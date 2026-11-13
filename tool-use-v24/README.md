# Tool use · v24 交互图

打开 [汇总入口](index.html)。六张图均使用已安装的 `codex-repo-blueprint` v24 流程，页面上的 `v6.4` 是冻结渲染器版本。

| 图 | 阅读重点 | 页面 |
|---|---|---|
| 01 调用入口 | 登记、router 配置、计时与 task / Future 移交 | [打开](01-runtime/out/deliverable/roundtrip/index.html) |
| 02 后台分派 | readiness、并发门、router dispatch、结果就绪 | [打开](02-dispatch-task/out/deliverable/roundtrip/index.html) |
| 03 等待与取消 | 完成竞态、abort、取消通知、全流程耗时 | [打开](03-wait-cancel/out/deliverable/roundtrip/index.html) |
| 04 Registry | handler 校验、PreToolUse / PostToolUse、生命周期与交付 | [打开](04-registry/out/deliverable/roundtrip/index.html) |
| 05 Orchestrator | 审批、sandbox、managed network、条件重试 | [打开](05-orchestrator/out/deliverable/roundtrip/index.html) |
| 06 exec_command | environment、cwd、shell、权限、apply_patch、进程模式与输出 | [打开](06-exec-command/out/deliverable/roundtrip/index.html) |

推荐先读 01，再分别展开 02 与 03；04、05、06 对应工具执行的不同职责。这个排列不是所有工具通用的直接调用链。

源码 commit：`c248f6d48b97eb4a2aa56147a0b11b7d763278b9`。每个页面支持阶段 / goal / action / 消息展开、参与者层级展开，以及 Rust 源码和 BB 证据联动。

## 验收与证据范围

每个输出保留 S0–S8 检查产物、作者账本、独立源码核验、浏览器检查和 `out/e2e-summary.md`。最新状态见 [delivery-status.json](delivery-status.json)。

Registry、Orchestrator、exec_command 分别有 4、11、12 项被调函数 MIR 不在原始抽取范围；这是按图统计，不代表 27 个互不重复的函数。各主 body 的 BB 全覆盖；缺失项在对应报告中保留，不能据此称为无缺失的干净通过。

01 入口图使用 4 个已登记的本次运行修补模块：复用原 span 白名单的证明逻辑、独立证明器的相应验证，以及把登记模块加载到独立检查进程的机制。修补只存在于本次输出的 `01-runtime/out/run-fixes/`，未修改安装的 skill、源码或冻结渲染器。白名单一致性与错误身份 / 非宏调用 / 非法状态写入等反例检查也在该目录中保留。

- [01 运行修补记录](01-runtime/out/run-fixes/deviations.md)
- [01 验收](01-runtime/out/e2e-summary.md)
- [02 验收](02-dispatch-task/out/e2e-summary.md)
- [03 验收](03-wait-cancel/out/e2e-summary.md)
- [04 验收](04-registry/out/e2e-summary.md)
- [05 验收](05-orchestrator/out/e2e-summary.md)
- [06 验收](06-exec-command/out/e2e-summary.md)

`inputs/ledgers/` 保存可复核语义账本；`out/deliverable/` 是各图正式交付；`out/work/` 保存阶段证据；`scratch/` 是运行临时数据。无需使用旧的 `v3-skill/output/` 页面。

公开副本将 Rust 依赖元数据中的本机 Cargo 目录规范化为 `$CARGO_HOME`；冻结渲染器、源码及图表语义保持不变。公开验收报告省略本机命令与日志路径。
