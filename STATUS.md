# 当前状态

本文件承担主仓库的总进度、能力起点、课程仓库索引、近期任务和跨环境交接入口。课程详细证据在对应独立仓库；计划范围见 [LEARNING_PLAN](LEARNING_PLAN.md)。

```yaml
last_updated: 2026-09-14
current_day: 2
completed_learning_days: 1
current_stage: foundations_r0
current_stage_status: testing_in_progress_r0_01_pending_personal_computer
plan_revision: systems_first_theory_lab_equal
repository_role: learning_overview
course_repository_strategy: separate_per_course_or_stage
scope_confirmed: 2026-09-10
foundation_diagnostics: not_started
course_environment_verification: pending_personal_computer
next_task: due_review_then_testing_test_first_programming
weekly_hours: 7
weekly_main_course_hours_proposed: 5
weekly_foundation_math_hours_proposed: 1
weekly_review_buffer_hours_proposed: 1
weekly_hours_confirmed: true
total_route_budget: to_be_reestimated
document_structure: simplified
sync_status: verify_head_against_origin_main
course_repository_sync_status: verified_published
handoff_document: https://github.com/W-yf/foundations/blob/main/README.md
handoff_status: tracked_repository_documents
management_session_role: course_repositories_plan_progress_and_handoff
next_management_task: maintain_overview_when_course_progress_changes
repository_name: self-Learning
repository_url: https://github.com/W-yf/self-Learning
remote_verified_at: 2026-09-14
remote_verified_branch: main
previous_verified_main_commit: 88ed5c2fc389cdcac717fa414cf4a456dbd4fb6f
```

## 已有成果与起点

- 初始化、旧 Stage 1–3 已完成并经用户确认，详见 [历史日志](logs/2026-08-12.md)。
- Day 1 于 2026-08-12 完成并确认巩固：安全路径通过 MSVC 编译、运行退出码为 0；新字符串 Lambda 场景的独立迁移解释通过。保留 [笔记](notes/day-01-lifetime.md) 和 [练习](exercises/day-01-lifetime/README.md)。
- 最近一次复习为 2026-09-11，三题均通过，下一最早复习日期为 2026-09-12，详见 [题库](reviews/question-bank.md)。2026-09-14 仅整理接续与同步，三题仍到期；学习仍在 Day 2，个人电脑环境与实验未推进，已完成学习日仍为 1，整体掌握层级不变。
- R0-01 已完成当前终端的环境初查，但编译、GDB 单步与 Python 测试均未通过验证。最新试行分工为理论学习端承担理论、视频和复习，个人电脑承担全部实验；个人电脑环境尚未核验，R0-01 留待该端完成，虚拟机或 WSL2 尚未选定。当前可先读 R0-02 Testing，理论与 lab 按主题接续并分别验收。详细记录见 [课程日志](https://github.com/W-yf/foundations/blob/main/logs/2026-09-10.md)。课程记录已发布，已核对版本见课程索引。
- 用户明确理论与 lab 同等重要，希望通过更有深度的实验弥补以往理论体会不足；工作经验作为起点信息，不替代独立学习证据。
- 课程笔记只保留课程知识和个人理解，必要时附权威来源与例子；小节结束整理，课程结束统一审校，不保存详细学习过程。Foundations 的 `notes/testing.md` 已整理测试的作用与边界，下一步阅读 Test-first Programming。笔记已随课程提交发布；无课程整体验收，掌握层级不变。
- RV-D1-001 此前包含题意理解偏差，2026-09-11 已用具体代码验证返回值取得、局部析构与调用方继续执行的顺序；后续沿用具体代码提问。

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

主仓库维护全局计划与必要进度，课程仓库保存知识笔记与实验。当前会话可以在已获授权范围内同步两仓库，不要求另切管理会话。

| 课程/阶段 | 远程地址 | 分支 | 状态与接续入口 | 已核对课程提交 | 当前状态 |
|---|---|---|---|---|---|
| R0 / foundations | [仓库](https://github.com/W-yf/foundations) | `main` | [README：个人电脑接续](https://github.com/W-yf/foundations/blob/main/README.md#个人电脑接续) | `ee6d54ae4ad5ab872985586be3533ac160ba2874` | 到期复习后继续 2022 版 Testing 的 Test-first Programming；schedule 导读为后续备用，项目作业未启动；R0-01 环境与实验未完成 |

上表课程提交于 2026-09-14 推送并核对本地 HEAD、origin/main 与远程 main 一致，包含精简笔记、环境记录、备用 teach 页面及最新接续入口。R0 主讲义采用 2022 版，旧 MITx 视频按主题配合；不学习 Java、不安排原版 Java 作业，四主题与自拟实验验收保留。材料准备与版本调整不代表已阅读、独立掌握或 R0 验收完成。

## 换电脑接续

1. 在已有的 `self-Learning` 和 `foundations` 本地仓库分别执行 `git pull --ff-only`；有未同步改动或分叉时先核对，不强制覆盖。
2. 读取本 STATUS 和课程 README，按其中“个人电脑接续”继续。必要的阅读位置、复习要求和实验入口均在 Git 中，无需复制聊天或旧临时 handoff。
3. 最近一次复习为 2026-09-11，三题下次日期均为 2026-09-12；截至 2026-09-14 已到期。学习前读 REVIEW 与题库，一次一道不同场景的具体代码题。学习日仍为 Day 2，已完成学习日仍为 1。
4. 个人电脑先核对已有 C/C++、GDB、Python 环境；理论阅读可继续，实验完成情况另验。工具安装不随 Git 同步。

## 可选分支计划

用户于 2026-09-10 确认小型 Python Agent Harness 为可选分支，拟独立完成后在个人 GitHub 展示。当前状态为尚未启动，未创建项目仓库、未分配工时、无实现或验收证据；范围与验收见 [LEARNING_PLAN](LEARNING_PLAN.md#可选分支小型-python-agent-harness)。R0 完成后可评估启动时机，当前主线保持不变，Testing 按近期任务接续。计划随本轮主仓库同步发布。

## 下一学习会话

主线编号现为 R0 短准备、R1 CSAPP、R2 OS、R3 离散/算法、R4 网络、R5 数据库，另有 M 基础数学支线。R0 环境初查及 Testing 理论学习已开展，其余任务按下表状态接续，不把文档更新算作学习完成。

| 近期任务 | 产出 |
|---|---|
| 检查到期复习 | 2026-09-11 三题均通过，下一最早复习日期为 2026-09-12；按实际学习日和 [REVIEW](REVIEW.md) 一次一题 |
| R0-01 最小环境与起点 | 转到个人电脑验证 C/C++、GDB 与 Python，用自拟小程序核对 C 指针/数组/结构体及分配释放；仍未完成 |
| R0-02 规格与测试 | 继续 2022 版 Testing 的 Test-first Programming，到 Systematic testing 标题前停止，配合视频 P21 对应部分与一道新题；链接见课程 README。再学系统测试、分区、边界与 Specifications，相关小练习验证后再进入项目作业 |
| R0-03 抽象与实现 | 读 ADT/表示不变量，完成邻接表与边列表两种小实现，共用测试 |
| R1-01 开始 CSAPP | R0 完成后读数据表示并启动 Data Lab，核对 btest/dlc 与第一组边界题；随后按计划进入 Bomb/Cache/Malloc |

准备阶段沿用原稿约 12 小时的预算基线，完成即进入 CSAPP；OS 紧随其后，完整算法课不作为 OS 开课条件。R0 以外的课内任务与验收只在 LEARNING_PLAN 维护。

用户于 2026-09-10 再次确认原稿为底稿，明确 CSAPP/OS 优先、网络/数据库后置，并确认每周约 7 小时。5 小时主课、1 小时基础数学、1 小时复习/缓冲仍为试行分配；六阶段 552 小时保留原稿基线，新增数学、前置补缺与最终周期尚待实际校准。

本轮已核对原稿与 CS 自学指南，将 CSAPP 章节/实验对应、进入 OS 前的 I/O 和体系结构衔接、xv6 实验所需理论写入 LEARNING_PLAN；来源见 RESOURCES。没有新增整门必修课或删减既定实验。首次在 R0 结束后按实际耗时调整，规划核查不代表课程环境验证通过。

随后按用户说明明确理论/实验分别验收，主课内两者各约一半作为试行起点。已读取所提供 Dr.Dng CSAPP 视频的简介和 23P 目录，记录按主题选集与缺口；尚未逐集试听或开始学习。视频与教材的使用分工见 RESOURCES，精选实验不缩减既定理论范围。

## 同步说明

2026-09-14 已先发布并核对课程仓库，提交见课程索引。本次主仓库发布范围为 2026-09-11 复习摘要、变式出题规则、2022 版阅读安排、资源与换电脑接续入口；不新增学习完成记录。

主仓库的本次完整版本以最新提交为准，避免在文件内记录它自身尚未生成的哈希。发布后核对 `git rev-parse HEAD`、`git rev-parse origin/main` 与 `git ls-remote origin refs/heads/main` 一致；同样核对课程仓库。`previous_verified_main_commit` 只标记此次发布前的基线。

主仓库既有未跟踪本机配置不属于学习资料，不纳入同步，也不是另一台电脑接续的依赖。旧临时开课快照已过时；当前交接依据为本 STATUS 与课程 README。历史发布记录见 [日志](logs/2026-09-10.md)。
