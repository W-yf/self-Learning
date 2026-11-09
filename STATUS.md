# 当前状态

本文件维护总进度、已有证据、课程目录索引和接续入口。详细范围见 [学习计划](LEARNING_PLAN.md)，资料见 [RESOURCES](RESOURCES.md)。

```yaml
last_updated: 2026-11-09
current_day: 2
completed_learning_days: 1
current_stage: stage_1_cs50x_linear_algebra
current_stage_status: planned_not_started
plan_revision: graphics_cuda_course_exercises
scope_confirmed: 2026-11-09
review_schedule: disabled
repository_role: learning_overview
course_repository_strategy: single_repository_course_directories
weekly_hours_stage_1: 7
weekly_hours_stage_2: 9-11
weekly_hours_stage_2_confirmed: 2026-11-09
weekly_hours_stage_3_proposed: 6-8
next_task: start_cs50x_week_0_and_create_course_directory
sync_status: migration_pending_publish
legacy_repository_deletion: manual_github_deletion_required
foundations_import_commit: a7d4ea2d0e2780650567f157de2c165828e9b34b
repository_url: https://github.com/W-yf/self-Learning
remote_pulled_at: 2026-11-09
published_main_baseline: 75ae3622d079c591b173c42e266f05d3de02532a
```

## 本次调整

- 用户取消独立复习排程，改用课程或书籍布置的习题、作业和实验检验成果；不再学前抽题、不更新间隔、不追加独立口述考试。
- 当前路线：CS50x/线代 → CSAPP/OSTEP 与 CPU 图形学 → PMPP/CUDA 与 CAM。第 2 阶段周投入 **9–11 小时已确认**；其余投入和阶段估时见计划。
- 旧 R0 不再作为主线前置；新路线尚未开课、未创建 CS50x 课程目录。本文更新不推进学习日或掌握层级，不表示任何旧任务已经完成。

## 已有成果与起点

- Day 1（2026-08-12）：安全路径经 MSVC 编译运行，退出码 0；有新字符串 Lambda 场景的独立迁移解释。保留 [笔记](notes/day-01-lifetime.md) 与 [练习](exercises/day-01-lifetime/README.md)。
- foundations（2026-09-16）：Test-first programming 与 Systematic testing 已有独立解释证据，包括 Spec → Test → Implement、预期结果来源及测试套件 correct/thorough/small；相应局部内容为 **2. 能够解释**。未完成课程整体验收，环境验证和实验没有完成证据。
- 旧返回流程题仍有未独立验证的问题；停用调度不等于掌握。旧题目与当时结果在 [历史题库](reviews/question-bank.md)，不再生成当前任务。

| 范围 | 保留证据 |
|---|---|
| 对象生命周期、作用域与悬空 | **2. 能够解释**，限定 Day 1 已验证范围，不外推完整语言细则 |
| 线性代数 | **1. 看过**，仅代表历史接触；仍需从基础重建 |
| C++、Python、调试、容器/BFS | 有自述使用经验，不替代新课程作业的独立实现与验证 |
| 缓存/局部性、并发/同步 | 旧诊断为 **1. 看过**，不视作已完成系统课 |
| CUDA | 未学习，GPU/Toolkit/profiling 环境未核验 |

## 课程目录索引

| 课程/阶段 | 入口 | 当前证据与状态 |
|---|---|---|
| 历史 R0 / foundations | [课程 README](courses/foundations/README.md) · [Testing 笔记](courses/foundations/notes/testing.md) | 保留独立解释证据；退出当前主线，实验和整体验收未完成 |

foundations 的已跟踪文件与原提交历史已整体迁入本仓库；来源提交为 a7d4ea2d0e2780650567f157de2c165828e9b34b。CS50x 等课程在实际启动时创建 courses/<course>/ 目录，登记版本、成果入口和下一步；独立项目或受限作业才另设仓库。

## 下一学习会话

1. 先读本 STATUS 与当前计划，**不启动旧复习或继续旧 R0 待办**。
2. 启动 CS50x 2026，创建 courses/cs50x/ 课程目录并登记版本；从 Week 0 课程和对应 problem set 开始，既有知识允许加快讲解，不跳过完成证据。
3. 线代副线从向量与线性变换开始，结合教材相关原有习题，不建立额外题卡。
4. 只配置当前作业必要工具。CSAPP/xv6/CUDA 环境留到对应阶段验证，不因本次规划重开初始化、安全检查或完整环境流程。

如果以后主动恢复 foundations，旧断点为 Testing 的 Choosing test cases by partitioning；这只是历史位置，不是当前待执行任务。

## 同步与跨电脑接续

日常只拉取、提交与推送 self-Learning；先读本 STATUS，再读课程 README，学后在同一提交中更新成果与必要进度。旧双仓发布流程已取消。

2026-11-09 用户授权合并 foundations 并在迁移验证后删除旧仓库。本轮迁移包含尚未推送的课程提交及完整原历史；先核对迁入文件、相对链接与 Git 对象，再提交并推送主仓库，最后处理旧仓库。发布及旧仓库处置结果见 [当日日志](logs/2026-11-09.md)。

现有 origin 使用旧名称 cuda-selfLearning 地址，可访问同一主仓库，本轮不修改远程配置。既有未跟踪 CppProperties.json 未改动、不提交。文件长度元数据异常仍用完整字节流与 Git 对象比对规避，不据工作区 diff 的假截断覆盖历史文件。
