# foundations

计算机基础回顾的历史 **R0：短准备与软件设计** 成果仓库。2026-11-09 主仓库改用 CS50x → 系统与 CPU 图形学 → CUDA/CAM 路线，本阶段退出当前主线，未完成任务不再作为开课前置。

本仓库保存本阶段的详细笔记、独立练习、测试与成果记录；[self-Learning 主仓库](https://github.com/W-yf/self-Learning) 保存总计划与总进度。本 README 是本课程的状态入口。

## 历史范围与验收（当前不执行）

固定参考 **MIT 6.031 Spring 2022** 的四份讲义：[Testing](https://web.mit.edu/6.031/www/sp22/classes/03-testing/)、[Specifications](https://web.mit.edu/6.031/www/sp22/classes/06-specifications/)、[Abstract Data Types](https://web.mit.edu/6.031/www/sp22/classes/10-abstract-data-types/)、[Abstraction Functions & Rep Invariants](https://web.mit.edu/6.031/www/sp22/classes/11-abstraction-functions-rep-invariants/)。使用 C/C++ 自拟练习，并按主题采用 Python 公开项目。用户明确不学习 Java，不安排 Java 补课、原版 Java 编程作业或 Java 评分器；相应知识通过独立练习验证。旧 MITx 视频按主题辅助理解，定义与版本差异以 2022 讲义为准；TypeScript 只按阅读需要解释，不自动新增语言课程。既有笔记保留当时实际使用的 2016 来源。

| 任务 | 完成证据 |
|---|---|
| R0-01 最小环境与起点 | 验证 C/C++ 编译运行、GDB 单步与 Python 测试；用自拟 C 小程序核对指针、数组、结构体及分配/释放，记录缺口 |
| R0-02 规格与测试 | 读 Testing、Specifications；为非负权有向图写接口约定和契约测试，涵盖增删点、设置边权、查询邻居 |
| R0-03 抽象与实现 | 读 ADT、抽象函数与表示不变量；用邻接表和边列表实现同一接口，并通过同一套契约测试 |

图的边界需明确重复节点、缺失节点、自环、负权输入和返回值所有权。验证修改返回的邻居集合不会改变内部图状态，并说明两种表示的不变量及替换依据。这些设计决定留在学习过程中独立完成。

**理论与实验同等重要**：既记录独立解释、推导与边界分析，也记录实现、调试和测试证据；区分独立产出与 AI 提示后的产出。约 12 小时仅为主计划的估时基线，实际用时按证据校准。

不扩展 GUI、持久化、图算法、完整 C++ 复习或系统 CMake 课程。完成本阶段验收后，由主仓库确认进入 CSAPP。完整范围与资料由主仓库的 [LEARNING_PLAN](https://github.com/W-yf/self-Learning/blob/main/LEARNING_PLAN.md) 和 [RESOURCES](https://github.com/W-yf/self-Learning/blob/main/RESOURCES.md) 维护。

## 当前状态

```yaml
last_updated: 2026-11-09
course_id: R0
repository_name: foundations
repository_url: https://github.com/W-yf/foundations
repository_role: course
branch: main
setup_status: remote_repository_initialized
learning_status: inactive_after_plan_revision
environment_verification: pending_personal_computer
theory_evidence: testing_limits_test_first_and_suite_criteria_explained_independently
lab_evidence: none
remote_status: configured
sync_status: local_commit_pending_push
initial_published_commit: 94d2d4b3bf0b9cbe258db5e82bc84546fe04a345
initial_publish_verified_on: 2026-09-10
overview_sync_status: see_main_repository_status
handoff_status: repository_readme_is_current_entry
next_task: follow_main_repository_cs50x_plan
```

本阶段已退出当前主线；以下为历史学习断点，不是当前待办。原处于 Testing：2026-09-16 已完成 Test-first programming 与 Systematic testing 当前小节。用户能够独立说明 Spec → Test → Implement、预期结果来源和调试价值，也能解释测试套件的 correct、thorough、small 及其平衡；两部分核心内容达到 **2. 能够解释**。下一步阅读 Choosing test cases by partitioning。正式项目作业尚未启动。schedule（标签 1.2.2）的 teach 导读 01 已备好，留待相关理论与小练习完成后使用；未记录为已阅读或掌握。R0-01 环境验证和所有实验留待个人电脑完成；理论与实验分别验收，尚无完整 R0 验收。

本 README 是当前交接入口，旧临时开课快照已过时，无需携带。环境初查见 [日志](logs/2026-09-10.md)；主仓库 [STATUS](https://github.com/W-yf/self-Learning/blob/main/STATUS.md) 登记已核对的课程提交。两仓库是否同步，以本地 HEAD 和远程 main 的实际比较为准。

## 学习笔记与成果入口

`notes/` 只保存课程知识和个人理解，必要时附来源、边界与例子；`exercises/` 保存实现与验证。学习时不逐题改文件，小节结束后整理，课程结束时统一审校、去重和精简。问答流水、提示过程与教学评语不写入笔记或另存为学习日志。

后续学习成果通过当前计划选定的课程/书籍习题、作业和实验检验，不再强制小节口述、独立抽题或复习调度。保留实际完成证据，不把已阅读或 AI 讲解记作独立掌握。

| 主题 | 内容 |
|---|---|
| [Testing：测试的作用与边界](notes/testing.md) | 测试通过的含义、反例与相等输入示例 |
| [schedule 导读 01](lessons/0001-schedule-registration.html) · [术语速查](reference/schedule-basics.html) | 后续备用的 AI 教学材料；未启动阅读或项目作业 |

关键结论以课程原文或官方资料为依据；个人理解忠实于实际表达，不把 AI 补充写成独立产出。README 只保留接续所需的进度和下一步，主仓库维护进度摘要。文件整理不代表课程验收完成。

## 个人电脑接续

1. 拉取主仓库与本仓库，先检查本地修改，不强制覆盖；读取主仓库 STATUS 与当前学习计划。
2. 当前下一步是启动 CS50x，本仓库保留历史成果。不要自动继续 R0、创建旧项目或筛选到期题；独立复习机制已取消。
3. 仅在用户明确恢复 R0 后，才从 Testing 的 Choosing test cases by partitioning 继续；环境与实验仍无完成证据，按当时实际任务核验。

2026-11-09 已快进拉取核对，本仓库已发布基线仍为 ee504f6708e382110441f1de8e9c3271692ed5ee。本次本地提交包含 README 与 AGENTS 的路线衔接调整，尚未推送；没有新增课程成果或运行实验。主仓库的新计划也需推送后另一台电脑才能读取。完整文件内容与暂存 Git 对象已核对，不以异常的工作区 diff 判断内容截断。
