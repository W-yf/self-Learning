# 当前状态

本文件是唯一总进度、课程索引与接续入口。详细范围见 [学习计划](LEARNING_PLAN.md)，资料见 [RESOURCES](RESOURCES.md)。

```yaml
last_updated: 2026-11-16
current_day: 1
completed_learning_days: 0
progress_scope: current_learning_plan
current_stage: core_programming_foundations
current_stage_status: planned_not_started
plan_revision: cpp_systematic_math_occt_qt_graphics_threadpool_optional_coroutines_spsc_cuda
plan_review_status: approved
plan_approved_at: 2026-11-16
repository_role: learning_overview
course_repository_strategy: single_repository_course_directories
weekly_hours_stage_1: 7
weekly_hours_stage_2: 9-11
weekly_hours_stage_2_confirmed: 2026-11-09
occt_work_version: 7.9.x
next_task: c_gap_exercises_analytic_geometry_and_occt_overview
sync_verification: compare_HEAD_origin_main_and_remote_main
repository_url: https://github.com/W-yf/self-Learning
remote_fetched_at: 2026-11-16
```

## 当前安排与审核状态

**以计算机基础知识构成最小、连贯的共同核心。** C++ 为主要实践语言，按程序、数据结构、机器执行、内存、操作系统和基本并发推进。软件设计与工程基础分段融入。

本版完整方案已于 **2026-11-16 审核通过并定稿**：

- 共同核心必修含 CS149 Assignment 2 Part A 线程池；Part B 任务图与 Taskflow 阅读为选修。
- 数学系统学习解析几何基础、18.06 主干（含 3Blue1Brown 辅助）、18.01SC 基础，连贯选学必要 18.02SC 和曲线曲面。
- OCCT 7.9.x 先通识再专题，用 Qt 辅助可视化；CAM 概念持续结合工作。
- GAMES101 原作业 0–2、3 基础及 LearnOpenGL 安排入门；CUDA 第一轮选修，均满足局部先修后提前进入。
- 协程在 RAII、移动语义、泛型和异常基础之后选修；SPSC 在同步与原子内存模型之后选修，不同时开多个项目。深入几何内核不是其他方向的前置。

起步 **7 小时/周**：核心 4、数学 2、OCCT 通识或观察 1。后续 **9–11 小时/周**：核心 4–5、数学 3、一个应用主题 2–3。核心工程基础与线程池不另加周投入，选修替换当期选修时段。

共同核心 **385–585 小时**（含工程基础 35–55、线程池 Part A 20–35）；基础与已安排的数学、OCCT、Qt、图形学/OpenGL、CAM 合计 **925–1415 小时**。含 CUDA 第一轮 40–70 小时，共 **965–1485 小时，约 30–50 个月**，以每年约 40 个有效学习周估算并按实际耗时校准。Part B 15–30、Taskflow 8–12、协程 15–25、SPSC 20–35 小时另计。

当前计划尚未开课，已完成学习日为 0。此次仅定稿文档，不提升掌握层级；以原有习题和实验事实记录进度，不把阅读、AI 产出和独立完成混为一谈。

## 课程目录索引

当前尚无已启动课程。实际开课才在 courses 下创建课程目录，在此登记范围、版本、课程 README、成果入口与下一步；课程内保存笔记、练习和验证证据。

## 下一学习会话

1. 检查本地修改、分支与上游，保留未同步内容；条件允许时快进同步本仓库，再读本 STATUS 与适用规则。
2. 核心每周 4 小时：用 CS50x Week 1–5 的 C 原题按缺口确认起点；能独立完成并解释的部分加快通过，随后接 CS106L，必要语言缺口查 PPP3。需求、边界与任务拆分从核心时段少量穿插。
3. 数学每周 2 小时：先连贯启动《解析几何》第 5 版的向量与坐标基础，衔接 MIT 18.06 和 3Blue1Brown；保持一个主要数学单元，不同时重开多门完整数学课。
4. 应用每周 1 小时：OCCT 官方 Introduction 与概览视频建立模块关系，随后进入同版本 Bottle。开课登记工作实际 7.9 补丁版本，使用对应资料，不复制公司代码或客户数据。
5. 掌握基本 C++ 后进入 Qt 官方教程及 OCCT 示例；向量、矩阵和变换具备后进入 GAMES101；OpenGL 在对应图形概念后开始。CUDA 按其局部先修轮换探索，无需等全部数学和 OCCT 学完。
6. C++ 生命周期、线程、互斥锁、条件变量具备后进入 CS149 Part A。Part B、Taskflow、协程和 SPSC 只在选定时启动；不要现在配置所有项目环境。
7. 实际开课才创建目录并登记原题与版本。小节结束整理精简笔记、课程接续任务和本 STATUS 摘要；完成前几个单元后校准时间。

## 同步与跨电脑接续

操作步骤与新对话提示词见 [README](README.md#两台电脑同步与接续学习)。总计划与本 STATUS 决定安排，课程文件提供事实证据。

本机既有未跟踪 CppProperties.json 保留，不纳入本轮文档提交，也不作为跨电脑依赖。每次接续以实际 Git 状态检查未同步事项。
