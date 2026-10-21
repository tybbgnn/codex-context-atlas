# Codex 函数图谱

按 G01 请求接入、G02 回合主循环、G03 Context 构造组织的静态网站。

共 13 个入口：12 个交互图，F01 process_request 待补充。

v24 更新：替换 run_turn 及环境展示路径块、采样请求块、采样输入块、采样后状态块。5 个页面均标注 G02 · 回合主循环 / v24；所提供最终验收记录均为通过。

入口为 index.html。每个已完成函数的页面位于 functions/<slug>/roundtrip/index.html。配套数据、脚本和样式随站点一起发布。

GitHub Pages 使用 main 分支根目录，.nojekyll 禁用 Jekyll 转换。

图表是源码静态投影，不是运行轨迹。非 OpenAI 官方网站。
