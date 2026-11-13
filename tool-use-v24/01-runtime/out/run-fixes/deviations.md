# 运行偏离

## instrumentation_wrapper.py / [1, 2, 3, 4, 5, 6, 7]
同步 task builder 中的 span 宏没有 enter，逐 BB event 证明未复用既有 span 白名单、bool Not 与闭合 storage connector 规则。
判断：bb134/171 与148/149/150 是完整 tracing-only；bb126/142/144/167/169/177 含非宏状态或源码字段读，应继续保留。现有 span 白名单 AST 未改变，反例测试拒绝业务写与错误身份。
修正：提取既有 span callee predicate 供逐 BB 证明复用；Not 额外约束唯一 tracing bool 来源和同宏使用；source-less connector 要求两侧已证明且仅宏临时 storage。独立检查及所有阈值不改。
证据：[{'path': '$OUTPUT_ROOT/01-runtime/out/work/raw-body.json', 'sha256': 'a055391183bd540542c7b8f187eb4b6ba78517b56b2dc2e83993c163a1dbc34b'}, {'path': '$OUTPUT_ROOT/01-runtime/out/run-fixes/repair-checks.json', 'sha256': '78a3a8043caceb6cd4af10faab5a140d5f875cef136aac780a584d2636bfc108'}]
脚本：$OUTPUT_ROOT/01-runtime/out/run-fixes/instrumentation_wrapper.py
SHA256：945d0ba25635c7293cfebccf2aff33e8e6fad150ab9abe9bafdd1f9d56aa3fe9

## classify.py / [1, 2, 3, 4, 5, 6, 7]
同步 task builder 中的 span 宏没有 enter，逐 BB event 证明未复用既有 span 白名单、bool Not 与闭合 storage connector 规则。
判断：bb134/171 与148/149/150 是完整 tracing-only；bb126/142/144/167/169/177 含非宏状态或源码字段读，应继续保留。现有 span 白名单 AST 未改变，反例测试拒绝业务写与错误身份。
修正：提取既有 span callee predicate 供逐 BB 证明复用；Not 额外约束唯一 tracing bool 来源和同宏使用；source-less connector 要求两侧已证明且仅宏临时 storage。独立检查及所有阈值不改。
证据：[{'path': '$OUTPUT_ROOT/01-runtime/out/work/raw-body.json', 'sha256': 'a055391183bd540542c7b8f187eb4b6ba78517b56b2dc2e83993c163a1dbc34b'}, {'path': '$OUTPUT_ROOT/01-runtime/out/run-fixes/repair-checks.json', 'sha256': '78a3a8043caceb6cd4af10faab5a140d5f875cef136aac780a584d2636bfc108'}]
脚本：$OUTPUT_ROOT/01-runtime/out/run-fixes/classify.py
SHA256：48a40b30339fade5046313a058f6dee432136fedc9ecb97205ac151040981b8e

## stage_engine.py / [7]
S7 独立 Python 子进程只添加原包 PYTHONPATH，不加载本次已登记的证明模块；新事实将被旧证明器误判。
判断：stage7 在 subprocess.run 前只替换检查器主脚本路径，分类依赖的 run-local 修复没有传播；需要让原检查器在加载同一 SHA 锁定证明模块后运行。
修正：原检查器正文、参数、阈值及执行超时不变；在独立新进程中先调用既有 run_fixes.apply(Context,7)，再 runpy 执行原检查器。
证据：[{'path': '$SKILL_ROOT/scripts/stage_engine.py', 'sha256': '2a17fbb0bbe1ac35293204a5ac0ae6f2447471468bb33d75008d81fadd5e9d04'}, {'path': '$OUTPUT_ROOT/01-runtime/out/run-fixes/repair-checks.json', 'sha256': '78a3a8043caceb6cd4af10faab5a140d5f875cef136aac780a584d2636bfc108'}]
脚本：$OUTPUT_ROOT/01-runtime/out/run-fixes/stage_engine.py
SHA256：03c8489f05010025545381598fbadae84a061b8c232d96732dba6ac4fc812e08

## event_macro_verifier.py / [7]
独立 event verifier 与生成证明器一样未复用既有 span 证明规则，漏验合法的 Not、Span::record_all 和闭合 storage connector。
判断：从原始 MIR 独立重算，不读取生成器的证明结果；白名单来自原有独立 span verifier，未修改该表。突变反例仍被拒绝。
修正：保持独立实现与全部错误检查；增加同宏唯一 bool 来源、局部输出封闭和已证明邻居条件，以原始 MIR 再证明相同 witness。
证据：[{'path': '$OUTPUT_ROOT/01-runtime/out/work/raw-body.json', 'sha256': 'a055391183bd540542c7b8f187eb4b6ba78517b56b2dc2e83993c163a1dbc34b'}, {'path': '$OUTPUT_ROOT/01-runtime/out/run-fixes/independent-repair-checks.json', 'sha256': 'e16ba9d01fd098e190c3a7edd4a6183fcebd176729cfe1bc84df73d09fd18658'}, {'path': '$SKILL_ROOT/scripts/span_wrapper_extension_verifier.py', 'sha256': 'fa3fb8b77147f382941cd1011eb2dc1b451c5561b0b6be502500fed75089985f'}]
脚本：$OUTPUT_ROOT/01-runtime/out/run-fixes/event_macro_verifier.py
SHA256：f2c3dae274cc2e39db2147e509edb0feddfe03cad217daffb31bfbdaaaac3767
