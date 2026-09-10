# 当前状态

本文件承担主仓库的总进度、能力起点、课程仓库索引、近期任务和跨环境交接入口。课程详细证据在对应独立仓库；计划范围见 [LEARNING_PLAN](LEARNING_PLAN.md)。

```yaml
last_updated: 2026-09-10
current_day: 2
completed_learning_days: 1
current_stage: goal_and_route_rebaseline
current_stage_status: published_ready_for_foundations_session
plan_revision: systems_first_theory_lab_equal
repository_role: learning_overview
course_repository_strategy: separate_per_course_or_stage
scope_confirmed: 2026-09-10
foundation_diagnostics: not_started
course_environment_verification: not_started
next_task: review_then_r0_design_and_csapp_setup
weekly_hours: 7
weekly_main_course_hours_proposed: 5
weekly_foundation_math_hours_proposed: 1
weekly_review_buffer_hours_proposed: 1
weekly_hours_confirmed: true
total_route_budget: to_be_reestimated
document_structure: simplified
sync_status: published_content_verified
course_repository_sync_status: initial_publication_verified_overview_recorded
handoff_skill_status: available
handoff_document: foundations-start-handoff-2026-09-10.md
handoff_status: generated_temp_file_requires_explicit_transfer
management_session_role: course_repositories_plan_progress_and_handoff
next_management_task: await_course_progress_and_maintain_overview
repository_name: self-Learning
repository_url: https://github.com/W-yf/self-Learning
remote_verified_at: 2026-09-10
remote_verified_branch: main
published_learning_commit: bbeae7510d662c5b0fc30a764131c6cbe309f6f6
```

## 已有成果与起点

- 初始化、旧 Stage 1–3 已完成并经用户确认，详见 [历史日志](logs/2026-08-12.md)。
- Day 1 于 2026-08-12 完成并确认巩固：安全路径通过 MSVC 编译、运行退出码为 0；新字符串 Lambda 场景的独立迁移解释通过。保留 [笔记](notes/day-01-lifetime.md) 和 [练习](exercises/day-01-lifetime/README.md)。
- Day 2 和新 R0 未开始。本次计划核对与仓库维护没有增加学习日、诊断或复习作答。
- 用户明确理论与 lab 同等重要，希望通过更有深度的实验弥补以往理论体会不足；工作经验作为起点信息，不替代独立学习证据。

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

## 课程仓库与交接索引

用户已确认采用“主仓库总览＋课程/阶段独立仓库”的方式。课程目录与主仓库分开放置，并已作为附加文件夹关联到同一个 Codex 项目；主仓库保留为主要文件夹。本 session 当前定位为课程仓库管理会话，负责开启与维护独立课程仓库、回写主仓库的宏观进度与计划摘要，并按需要生成 handoff；课程学习会话负责课程内实际学习。仓库初始化和文档发布不计入学习日或掌握证据。

本轮已核验课程仓库 `foundations` 使用远程地址 `https://github.com/W-yf/foundations`，分支为 `main`；本地 `main` 与远程 `main` 均为 `b435b1f2d508f9df96df5bf2c1aea08a26bf19ae`，工作区干净。课程 README 记录首次初始化提交 `94d2d4b3bf0b9cbe258db5e82bc84546fe04a345`；当前提交是后续筹备发布记录，不是学习成果。课程尚未开始，环境、代码、测试和学习证据均无。该版本课程 README 中“主仓库摘要待发布”和“handoff 未生成”保留的是本次发布前的快照；本次主仓库汇总已发布、交接已生成，课程文件尚未回写这些元数据，以本节较新的核验事实为准。

| 课程/阶段 | 远程地址 | 分支 | 状态入口 | handoff | 已核对成果提交 | 当前状态 |
|---|---|---|---|---|---|---|
| R0 / foundations | [仓库](https://github.com/W-yf/foundations) | `main` | [README.md](https://github.com/W-yf/foundations/blob/main/README.md)（课程状态入口） | 已生成开课交接；临时文件需显式传递，入口见下方 | `b435b1f2d508f9df96df5bf2c1aea08a26bf19ae`（筹备发布记录，非学习成果） | 首次同步已核验；课程未开始；环境、代码、测试和学习证据均无；主仓库汇总已发布 |

每次实际启用课程仓库，在此维护一条记录：课程/阶段、仓库地址与分支、详细状态文档、最新 handoff 入口、已核对的成果提交、理论/实验进度摘要与下一步。课程原始记录归课程仓库，本文件汇总并链接证据；课程已有新成果而这里尚未回写时，标记汇总待更新，再依据已发布证据同步。

新对话接手先拉取主仓库与当前课程仓库，再核对状态文件、交接日期和基线提交；学习结束先推送并核对课程成果，再回写并同步主仓库。统一复习队列继续由本仓库维护，课程仓库提供证据引用。现有 Day 1 文件保留原位。

已按用户指定的 handoff skill 生成 `foundations-start-handoff-2026-09-10.md`，用于新的 Foundations/R0 学习会话，包含基线提交、必读入口、接手事项和建议技能。文件位于生成机器的操作系统临时目录，具体文件通过管理会话交付，公开索引只记录文件名；换电脑或新会话时需显式传递，不会随 Git 自动同步。长期计划、进度和学习证据仍在各仓库，临时交接不可作为唯一状态载体。本次尚未创建课程学习会话。

## 下一学习会话

主线编号现为 R0 短准备、R1 CSAPP、R2 OS、R3 离散/算法、R4 网络、R5 数据库，另有 M 基础数学支线。下表均未开始，不把文档更新算作学习。

| 近期任务 | 产出 |
|---|---|
| 检查到期复习 | 按 [REVIEW](REVIEW.md) 一次一题；当前 3 张 active 到期、3 张 suspended、2 个 parked，实际开课日重新筛选 |
| R0-01 最小环境与起点 | 检查 C/C++ 编译、GDB 与 Python 测试，用自拟小程序核对 C 指针/数组/结构体及分配释放；记录当前缺口与环境可用性 |
| R0-02 规格与测试 | 读 Testing/Specifications，写非负权有向图的接口边界和契约测试 |
| R0-03 抽象与实现 | 读 ADT/表示不变量，完成邻接表与边列表两种小实现，共用测试 |
| R1-01 开始 CSAPP | R0 完成后读数据表示并启动 Data Lab，核对 btest/dlc 与第一组边界题；随后按计划进入 Bomb/Cache/Malloc |

准备阶段沿用原稿约 12 小时的预算基线，完成即进入 CSAPP；OS 紧随其后，完整算法课不作为 OS 开课条件。R0 以外的课内任务与验收只在 LEARNING_PLAN 维护。

用户于 2026-09-10 再次确认原稿为底稿，明确 CSAPP/OS 优先、网络/数据库后置，并确认每周约 7 小时。5 小时主课、1 小时基础数学、1 小时复习/缓冲仍为试行分配；六阶段 552 小时保留原稿基线，新增数学、前置补缺与最终周期尚待实际校准。

本轮已核对原稿与 CS 自学指南，将 CSAPP 章节/实验对应、进入 OS 前的 I/O 和体系结构衔接、xv6 实验所需理论写入 LEARNING_PLAN；来源见 RESOURCES。没有新增整门必修课或删减既定实验。首次在 R0 结束后按实际耗时调整，规划核查不代表课程环境验证通过。

随后按用户说明明确理论/实验分别验收，主课内两者各约一半作为试行起点。已读取所提供 Dr.Dng CSAPP 视频的简介和 23P 目录，记录按主题选集与缺口；尚未逐集试听或开始学习。视频与教材的使用分工见 RESOURCES，精选实验不缩减既定理论范围。

## 同步说明

此前学习计划调整、文件精简和文本清理已随提交 `88d50a9` 推送并完成远程核对；后续维护提交为 `72ab2bc`。本轮修改前只读核对远程 main 与本地 HEAD 均为 `72ab2bcd1ec2f61a0c9f178b9ca39a3910a2e2d9`。

仓库已更名为 [self-Learning](https://github.com/W-yf/self-Learning)。历史日志中的 origin 已更新描述属于当时环境；本次本地 origin 仍为旧名称地址，已能核对相同远程 main，本轮未修改远程配置。

本轮原稿/网页核对、理论与实验并重、视频使用、管理会话职责、多仓库分工与 foundations 索引已通过提交 `bbeae7510d662c5b0fc30a764131c6cbe309f6f6` 推送并核对远程 main。`published_learning_commit` 记录这次已核验的内容发布；本节和当日日志为发布后的维护记录，最新完整文档版本以远程 main 为准。

课程仓库仍保持已核验的 `b435b1f2d508f9df96df5bf2c1aea08a26bf19ae`，本次未修改课程文件。主仓库保留一个既有未跟踪的本机配置文件，未纳入提交，不属于学习材料或跨电脑接手依赖。发布和生成交接不推进学习日、掌握层级或复习结果。过程见 [当日日志](logs/2026-09-10.md)。
