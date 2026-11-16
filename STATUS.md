# 当前状态

本文件维护总进度、课程索引和接续入口。详细范围见 [学习计划](LEARNING_PLAN.md)，资料入口见 [RESOURCES](RESOURCES.md)。

```yaml
last_updated: 2026-11-16
current_day: 1
completed_learning_days: 0
progress_scope: current_learning_plan
current_stage: core_programming_foundations
current_stage_status: planned_not_started
plan_revision: minimal_cs_core_cam_occt79_early_graphics_cuda
plan_review_status: approved
plan_approved_at: 2026-11-16
repository_role: learning_overview
course_repository_strategy: single_repository_course_directories
weekly_hours_stage_1: 7
weekly_hours_stage_2: 9-11
weekly_hours_stage_2_confirmed: 2026-11-09
occt_work_version: 7.9.x
next_task: start_cs50x_c_gap_exercises_and_occt79_overview
sync_verification: compare_HEAD_origin_main_and_remote_main
repository_url: https://github.com/W-yf/self-Learning
remote_fetched_at: 2026-11-16
```

## 当前安排

**以计算机基础知识构成最小、连贯的共同核心。** C++ 为主要实践语言，按程序、数据结构、机器执行、内存和操作系统推进。

当前 CAM 工作以 OCCT 7.9.x 为基础，先补整体概念，再结合轮廓、表面、孔、拾取和转换等任务研究几何与拓扑、空间数学和接口语义。目标是准确理解需求与约束，理解并独立修改代码，验证结果、定位错误并在需要时分析性能。图形学和 CUDA/HPC 满足局部先修后提前探索，后续按实践体验选择一项深入。

本版方案已于 **2026-11-16 审核通过并定稿**，范围与时间以 LEARNING_PLAN 为准：起步 7 小时/周（核心 5、工作基础及相关数学 2），后续 9–11 小时/周（核心与所需数学 6–7、工作基础与探索 3–4）。本轮预计 520–805 小时、18–30 个月，后续方向深化另行估时。

当前计划尚未开课，已完成学习日为 0。此次调整仅更新计划和资料，不推进学习日或掌握层级。实际掌握情况由课程习题和实验确认。

## 课程目录索引

当前尚无已启动课程。实际开课时创建 `courses/<course>/`，在此登记范围、课程版本、README、成果链接和下一步。课程内保存笔记、练习与验证证据。

## 下一学习会话

1. 检查本地修改、分支与上游，保留未同步内容；快进同步本仓库后，读取本 STATUS、适用规则和当前计划。
2. 核心时段从 CS50x 2026 Week 1–5 的 C 相关原题按缺口接续。能独立完成并解释的部分加快通过，遇到概念缺口再补讲解。实际开课时创建 `courses/cs50x/` 并登记题目、成果与接续任务。
3. 方向时段启动 OCCT 通识：Quaoar 第 7、8 讲结合 7.9 官方 Introduction，认识模块与几何/拓扑的关系，再进入对应版本 Bottle。实际开课时创建 `courses/occt/`，登记工作项目实际 7.9 补丁版本和学习环境；资料使用匹配版本，不复制工作项目代码或数据。
4. 按每周核心 5 小时、工作基础与相关数学 2 小时执行。完成前几个单元后，用练习与调试的实际耗时校准安排；图形学与 CUDA 在满足各自启动条件后，使用方向时段分阶段开始。
5. 只配置当前练习必要工具。小节结束整理课程笔记，更新课程 README 与本 STATUS 的成果入口、简短摘要和下一步。

## 同步与跨电脑接续

操作步骤与新对话接手提示词见 [README：两台电脑同步与接续学习](README.md#两台电脑同步与接续学习)。课程安排以本 STATUS 为入口，实际成果以课程文件为依据。

2026-11-16 更新前已获取远程引用，核对本地 main 与 origin/main 一致。每次提交和推送后仍需按 README 核对 HEAD、origin/main 与远程 main；发布结果以 Git 为准，不把审核通过等同于已推送。

本轮四份文档已完成检查并在本地提交；2026-11-16 推送因本机 Git 无法取得 GitHub HTTPS 凭据而失败，尚未发布。待本机认证恢复后执行 `git push origin main`，核对 HEAD、origin/main 与远程 main，再清除此待同步事项。当前远程仍是本轮更新前的版本。

既有未跟踪 `CppProperties.json` 为本地文件，本次保留且不纳入提交。换电脑后按实际 Git 状态检查未同步事项。
