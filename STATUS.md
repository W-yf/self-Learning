# 当前状态

本文件维护当前计划的总进度、课程索引和接续入口。详细范围见 [学习计划](LEARNING_PLAN.md)，资料见 [RESOURCES](RESOURCES.md)。

```yaml
last_updated: 2026-11-13
current_day: 1
completed_learning_days: 0
progress_scope: current_learning_plan
current_stage: core_programming_foundations
current_stage_status: planned_not_started
plan_revision: minimal_cs_core_and_cam_exploration
plan_review_status: approved
plan_approved_at: 2026-11-13
repository_role: learning_overview
course_repository_strategy: single_repository_course_directories
weekly_hours_stage_1: 7
weekly_hours_stage_2: 9-11
weekly_hours_stage_2_confirmed: 2026-11-09
weekly_hours_stage_3_proposed: 6-8
next_task: fill_c_gaps_with_cs50x_exercises_and_create_course_directory
sync_verification: compare_HEAD_origin_main_and_remote_main
repository_url: https://github.com/W-yf/self-Learning
remote_pulled_at: 2026-11-13
```

## 当前安排

2026-11-09 确认计算机基础共同核心，以 C++ 为主要实践语言。2026-11-13 确认方向探索的优先级。先立足当前 CAM 研发，持续研究 OCCT、加工工艺和接口语义。再把几何处理、数值验证与系统能力用于 CAD、CAM、CAE 之间的迁移。随后按兴趣向机器人运动规划、工业可视化与渲染或 CUDA 高性能计算与算子开发延伸。具体范围和工时见[学习计划](LEARNING_PLAN.md)。

新计划尚未开课。学习日从本计划第 1 天起计算，已完成 0 天；这表示当前计划的进度，不否认过去的学习经历。当前掌握情况由后续课程习题和实验确认。

## 课程目录索引

当前尚无已启动课程。实际开课时创建 `courses/<course>/`，在此登记课程版本、README、成果入口和下一步；独立项目或受限作业才另设仓库。

## 下一学习会话

1. 检查本地分支和修改、同步远程，再读本 STATUS 与已确认计划。
2. 从 CS50x 2026 的 C 相关原题按缺口接续，实际启动时创建 `courses/cs50x/` 并登记课程版本、题目与成果入口；Week 0 作背景，优先 Week 1–5，能独立完成的内容加快通过。
3. 起步每周约 7 小时，其中核心 5–6 小时、方向探索 1–2 小时。完成首个课程单元后用实际耗时校准安排。需要探索时，先确认工作所用 OCCT 版本，可用纯平移样例区分轨迹点与方向，或用一条五轴轨迹核对参考点、坐标系和补偿分工。核心深化阶段的探索计入每周已有的 2–3 小时预算。
4. 只配置当前作业必要工具。CSAPP/xv6/CUDA 环境留到对应阶段验证。

## 同步与跨电脑接续

首次克隆、学前同步、学后提交核验和两类新对话接手提示词，统一见 [README：两台电脑同步与接续学习](README.md#两台电脑同步与接续学习)。当前课程与下一步以本 STATUS 为准。

2026-11-10 按用户要求清理旧学习记录及对应入口；历史记录仍可通过 Git 查阅。跨电脑接续时，以本地 HEAD、origin/main 和远程 main 是否一致核对同步结果。

既有未跟踪 `CppProperties.json` 未改动。若文件长度元数据异常造成假截断，应核对完整字节流与 Git 对象，不据异常 diff 覆盖文件。
