# 当前状态

本文件同时承担进度、能力起点、近期任务和跨环境交接。计划范围见 [LEARNING_PLAN](LEARNING_PLAN.md)。

```yaml
last_updated: 2026-09-09
current_day: 2
completed_learning_days: 1
current_stage: goal_and_route_rebaseline
current_stage_status: systems_first_plan_updated
plan_revision: systems_first_with_required_labs
scope_confirmed: 2026-09-09
foundation_diagnostics: not_started
course_environment_verification: not_started
next_task: review_then_r0_design_and_csapp_setup
weekly_hours_assumption: 7
weekly_main_course_hours_proposed: 5
weekly_foundation_math_hours_proposed: 1
weekly_review_buffer_hours_proposed: 1
weekly_budget_confirmed: false
total_route_budget: to_be_reestimated
document_structure: simplified
sync_status: local_uncommitted
remote_verified_at: 2026-09-09
remote_verified_branch: main
remote_verified_commit: c463696e6c9db21dba4a8a514e7ed9b2a8b0c246
```

## 已有成果与起点

- 初始化、旧 Stage 1–3 已完成并经用户确认，详见 [历史日志](logs/2026-08-12.md)。
- Day 1 于 2026-08-12 完成并确认巩固：安全路径通过 MSVC 编译、运行退出码为 0；新字符串 Lambda 场景的独立迁移解释通过。保留 [笔记](notes/day-01-lifetime.md) 和 [练习](exercises/day-01-lifetime/README.md)。
- Day 2 和新 R0 未开始。本次只调整文档，没有新学习、诊断或复习作答。

| 范围 | 当前证据 |
|---|---|
| 对象生命周期、作用域与悬空 | **2. 能够解释**，有 Day 1 证据；不外推到全部 RAII 或语言细则 |
| 线性代数 | **1. 看过**，仅代表历史接触；已确认需要从基础重建 |
| C++ 编程、调试、容器与 BFS | 有使用经验，自述支持局部解释能力，尚无完整独立验证 |
| 所有权/view、移动与容器失效 | 旧诊断为 **1. 看过** 或尚未分配层级；按当前练习需要补缺 |
| 缓存/局部性、并发与同步 | 旧诊断为 **1. 看过**；机制和正确性仍需验证 |
| CMake、性能工具、CUDA | 旧起点保留于 Git 历史；CMake/性能工具曾接触，CUDA 未学习，均不是当前必补清单 |
| Python 与其余数学、算法、组成、OS、网络、数据库 | Python 有既往经历，其余范围在对应入口诊断；不按缺少证据判定全部零基础 |

旧 B1–B7 细节可从 Git 历史查阅。Day 1 文档中旧 CMake 学习日、完整 Lambda 等后续安排已失效；历史证据与当前任务分开使用。

## 下一学习会话

主线编号现为 R0 短准备、R1 CSAPP、R2 OS、R3 离散/算法、R4 网络、R5 数据库，另有 M 基础数学支线。下表均未开始，不把文档更新算作学习。

| 近期任务 | 产出 |
|---|---|
| 检查到期复习 | 按 [REVIEW](REVIEW.md) 一次一题；当前 3 张 active 到期、3 张 suspended、2 个 parked，实际开课日重新筛选 |
| R0-01 最小环境与起点 | 检查 C/C++ 编译、GDB 与 Python 测试；只诊断当前任务所需知识，记录环境可用性 |
| R0-02 规格与测试 | 读 Testing/Specifications，写非负权有向图的接口边界和契约测试 |
| R0-03 抽象与实现 | 读 ADT/表示不变量，完成邻接表与边列表两种小实现，共用测试 |
| R1-01 开始 CSAPP | R0 完成后读数据表示并启动 Data Lab，核对 btest/dlc 与第一组边界题；随后按计划进入 Bomb/Cache/Malloc |

准备阶段沿用原稿约 12 小时的预算基线，完成即进入 CSAPP；OS 紧随其后，完整算法课不作为 OS 开课条件。R0 以外的课内任务与验收只在 LEARNING_PLAN 维护。

每周约 7 小时仍是假设，本轮暂分主课 5 小时、基础数学 1 小时、复习/缓冲 1 小时。六阶段原稿工时参考合计 552 小时，新增数学完整工时与最终周期尚待估算。恢复既定实验与优先级已经写入计划，不代表确认全部工时或已完成课程环境验证。

## 同步说明

本轮在既有未提交修改上恢复原稿的明确实验与验收，并提高 CSAPP/OS 优先级；保持精简后的文件结构。远程 main 仍是上述提交，新路线和本次重构只在本地；未暂存、提交或推送。其他环境以已推送提交为准，同步后再据新文件继续。重构记录见 [本日日志](logs/2026-09-09.md)。
