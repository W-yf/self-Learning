# 当前状态

本文件是唯一总进度、课程索引和接续入口。范围见 [学习计划](LEARNING_PLAN.md)，资料见 [RESOURCES](RESOURCES.md)，路线见 [带学时流程图](docs/learning-roadmap.svg)与[可缩放版](docs/learning-roadmap.html)。

```yaml
last_updated: 2026-11-16
current_day: 1
completed_learning_days: 0
progress_scope: current_learning_plan
current_stage: core_programming_foundations
current_stage_status: planned_not_started
plan_revision: cpp_systems_os_before_algorithms_linear_algebra_first_flexible_3_2_2
plan_review_status: approved
plan_approved_at: 2026-11-16
repository_role: learning_overview
course_repository_strategy: single_repository_course_directories
ideal_weekly_hours_core: 3
ideal_weekly_hours_math: 2
ideal_weekly_hours_application: 2
ideal_weekly_hours_total: 7
weekly_hours_flexible: true
occt_work_version: 7.9.x
next_task: start_c_gap_exercises_linear_algebra_and_occt_overview
sync_verification: compare_HEAD_origin_main_and_remote_main
repository_url: https://github.com/W-yf/self-Learning
remote_fetched_at: 2026-11-16
```

## 当前安排与审核状态

**以计算机基础知识构成最小、连贯的共同核心。** 本版完整方案已于 **2026-11-16 审核通过并定稿**：

- 核心按 C 内存补缺与 C++ 基础 → CSAPP → OSTEP → 数据结构与算法；必要结构概念随系统原题补齐。线程池 Part A 在同步基础具备后进入，不等待完整算法。工程与离散数学嵌入核心时段。
- 数学从 MIT 18.06 线代与 3Blue1Brown 起步，之后解析几何、单变量微积分、必要多元微积分和曲线曲面；空间几何可按应用局部先修提前查阅。
- OCCT 7.9.x 先通识再专题，Qt 辅助可视化，CAM 概念持续补齐。GAMES101、LearnOpenGL 和 CUDA 第一轮明确安排入门，满足局部先修就进入。
- CUDA A/B/C 为 12–20、18–30、10–20h，合计 40–70h；在应用时段与图形学、OCCT 按阶段轮换，不等待整套数学、系统或线程池完成。
- Part B、Taskflow、协程、SPSC 及方向深化为选修；依据原题与实践体验选择一个主要深入方向。

每周理想投入为 **核心 3h、数学 2h、应用 2h，共 7h**。随事务弹性调整，不设逐周达标要求、欠时或固定工期；以先修和原有练习成果推进。

预计核心 385–585h、数学 335–505h、OCCT/Qt/CAM 115–185h、图形学/OpenGL 90–140h、CUDA 第一轮 40–70h，合计 **965–1485h**，后续选修另计。学时估计范围，实际耗时出来后再校准。

当前计划尚未开课，已完成学习日为 0。此次文档与流程图定稿不提升掌握层级。独立完成、提示后完成、AI 生成及示例运行分别记录。

## 课程目录索引

当前尚无已启动课程。实际开课才在 courses 下创建课程目录，在此登记范围、版本、课程 README、成果入口和下一步；课程内保存笔记、练习和验证证据。

## 下一学习会话

1. 检查本地修改、分支和上游，保留未同步内容；条件允许时快进同步本仓库，再读本 STATUS 与适用规则。
2. 核心理想 3h：使用 CS50x Week 1–5 的 C 原题按缺口确认起点，随后接 C++ 基础；能独立完成并解释的部分加快通过。具备指针、生命周期和调试后进入 CSAPP，再衔接 OSTEP。需求与边界从核心时段少量穿插。
3. 数学理想 2h：从 MIT 18.06 开始，配合 3Blue1Brown；原作业使用 Strang 第 4 版题号。应用需要叉积、直线平面时查解析几何对应内容，保持一个主要数学单元。
4. 应用理想 2h：先用 OCCT Introduction 与概览视频认识全貌，随后按基本 C++ 条件进入同版本 Bottle、Qt 教程与示例；开课登记实际 7.9 补丁版本。
5. 向量、矩阵和变换具备后做 GAMES101 原作业 0–2，再按段轮换 CUDA A 或后续图形/OpenGL。CUDA 以 C/C++、数组指针、调试和 CPU 参考实现为入口，不按月份启动；B/C 依各自先修和阶段成果衔接。
6. 学到 OSTEP 同步并具备 C++ 线程、锁、条件变量后，可在算法整课前完成线程池 Part A。数据结构算法整课安排在操作系统之后；其他项目选定后才配置环境。
7. 实际开课才创建目录、登记原题和版本。小节结束整理精简笔记、课程接续任务与本 STATUS 摘要；进度依据课程证据，不依据聊天或文档定稿。

## 同步与跨电脑接续

操作步骤和新对话提示词见 [README](README.md#两台电脑同步与接续学习)。审核状态与发布状态分开；同步以 HEAD、origin/main、远程 main 的实际提交为准。

既有未跟踪 CppProperties.json 为本机配置，不纳入本次提交或跨电脑依赖；每次接续以实际 Git 状态检查未同步事项。
