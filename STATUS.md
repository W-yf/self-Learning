# 当前状态

本文件维护总进度、已有证据、课程目录索引和接续入口。详细范围见 [学习计划](LEARNING_PLAN.md)，资料见 [RESOURCES](RESOURCES.md)。

```yaml
last_updated: 2026-11-09
current_day: 2
completed_learning_days: 1
current_stage: core_programming_foundations
current_stage_status: planned_not_started
plan_revision: guide_based_minimal_cs_core
plan_review_status: approved
plan_approved_at: 2026-11-09
scope_confirmed: 2026-11-09
repository_role: learning_overview
course_repository_strategy: single_repository_course_directories
weekly_hours_stage_1: 7
weekly_hours_stage_2: 9-11
weekly_hours_stage_2_confirmed: 2026-11-09
weekly_hours_stage_3_proposed: 6-8
next_task: fill_c_gaps_with_cs50x_exercises_and_create_course_directory
sync_verification: compare_HEAD_origin_main_and_remote_main
legacy_repository_deletion: deleted_by_user_verified_404
legacy_local_directory: removed
foundations_import_commit: a7d4ea2d0e2780650567f157de2c165828e9b34b
repository_url: https://github.com/W-yf/self-Learning
remote_pulled_at: 2026-11-09
published_main_baseline_before_plan: 8a024670acb7b5d01d61a9d85b5598891ed63512
```

## 本次调整

2026-11-09 用户已审核通过完整计划，并授权提交与推送。下一学习会话直接按以下安排接续。

- 学习定位：以计算机基础知识为最小核心，按知识联系和先修推进；图形学、CAD/CAM、OCCT、CUDA/HPC 等为细分探索方向。工作与岗位仅提供应用场景和辅助参考。
- 核对 CS 自学指南和 Teach Yourself CS；共同核心选 CS50x 按需补 C、CS106L 现代 C++、CS106B 数据结构算法、MCS 配套数学、CSAPP 与 OSTEP。OSTEP 保留文件/I/O/持久化基础，MIT 6.006 为替代课程，不与 CS106B 重复完整修读。
- 排错作为编程基础，复杂度、局部性与测量随原有习题学习，专项优化留给方向深入。共同核心约 330–500 有效小时，初估 12–18 个月，待实际作业耗时校准。
- 当前工作基于 OCCT，将其作为优先、持续研究对象；实际使用版本尚未确认。CUDA 保留执行与正确性、GPU 架构与性能、并行算法与算子、系统应用的独立深入路线。
- “量化系统研发”含义与兴趣范围尚未明确，先区分金融量化系统和模型量化/推理，通过小案例认识，不预设已选方向。
- 招聘参考限定江苏、浙江、上海、北京、广州、合肥，来源为 BOSS直聘、前程无忧、猎聘或公司官网；资料与证据见 RESOURCES。
- 核心深化每周 **9–11 小时已确认**，探索计入预算；xv6 选做，总工期按实际耗时校准。CS50x C 基础完成后可进入 C++/系统，完整课程后半按修课意愿续学。
- 旧 R0 不再作为主线前置；新路线尚未开课、未创建 CS50x 课程目录。本文更新不推进学习日或掌握层级，不表示任何旧任务已经完成。

## 已有成果与起点

- Day 1（2026-08-12）：安全路径经 MSVC 编译运行，退出码 0；有新字符串 Lambda 场景的独立迁移解释。保留 [笔记](notes/day-01-lifetime.md) 与 [练习](exercises/day-01-lifetime/README.md)。
- foundations（2026-09-16）：Test-first programming 与 Systematic testing 已有独立解释证据，包括 Spec → Test → Implement、预期结果来源及测试套件 correct/thorough/small；相应局部内容为 **2. 能够解释**。未完成课程整体验收，环境验证和实验没有完成证据。

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

1. 检查本地分支和修改、同步远程，再读本 STATUS 与已确认计划；当前路线尚未开课。
2. 从 CS50x 2026 的 C 相关原题按缺口接续，实际启动时创建 courses/cs50x/ 并登记课程版本、题目与成果入口；Week 0 作背景，优先 Week 1–5，能独立完成的内容加快通过。
3. 起步每周约 7 小时：核心 5–6 小时，轻量 OCCT/领域数学探索 1–2 小时。先完成一个课程单元并记录实际耗时，再校准后续安排；探索时先确认工作所用 OCCT 版本，从点、向量与变换联系基础数学。
4. 只配置当前作业必要工具。CSAPP/xv6/CUDA 环境留到对应阶段验证，不因本次规划重开初始化、安全检查或完整环境流程。

如果以后主动恢复 foundations，旧断点为 Testing 的 Choosing test cases by partitioning；这只是历史位置，不是当前待执行任务。

## 同步与跨电脑接续

日常只拉取、提交与推送 self-Learning；先读本 STATUS，再读课程 README，学后在同一提交中更新成果与必要进度。

本轮定稿的同步结果以本地 HEAD、origin/main 和远程 main 是否一致为准；上方基线仅记录定稿前已发布提交，不代表当前远程最新版本。

2026-11-09 已发布迁移成果与文档简化，包含迁移提交 6fb5a8a 和全部课程历史。用户已删除旧 GitHub 仓库，复查旧地址返回 404；旧本地空目录也已移除。后续仅维护 self-Learning，详情见 [当日日志](logs/2026-11-09.md)。

现有 origin 使用旧名称 cuda-selfLearning 地址，可访问同一主仓库，本轮不修改远程配置。既有未跟踪 CppProperties.json 未改动、不提交。文件长度元数据异常仍用完整字节流与 Git 对象比对规避，不据工作区 diff 的假截断覆盖历史文件。
