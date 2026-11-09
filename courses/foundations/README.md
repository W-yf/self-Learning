# foundations：历史 R0 成果

本目录保存原 foundations 仓库的短准备与软件设计成果，已于 2026-11-09 合并到 self-Learning。原主分支截至 a7d4ea2d0e2780650567f157de2c165828e9b34b 的提交历史保留在本仓库合并历史中，不再维护独立仓库。

总计划见 [LEARNING_PLAN](../../LEARNING_PLAN.md)，唯一总进度和下一步见 [STATUS](../../STATUS.md)。R0 已退出当前主线；以下未完成内容只是历史断点，不是新课程的前置条件。

## 已有成果与入口

| 内容 | 状态 |
|---|---|
| [Testing 笔记](notes/testing.md) | 已记录测试的作用/边界、Test-first programming、Systematic testing |
| [schedule 导读 01](lessons/0001-schedule-registration.html) · [术语速查](reference/schedule-basics.html) | 备用 AI 教学材料；未开始阅读或项目作业 |
| [环境与学习记录](logs/2026-09-10.md) | 历史环境与学习记录 |

截至 2026-09-16，Test-first 与测试套件 correct/thorough/small 有独立解释证据，相关局部内容达到 **2. 能够解释**。C/C++ 编译运行、GDB、Python 测试与项目实验尚无完成证据，未完成 R0 整体验收。迁移不增加学习日或掌握层级。

## 历史课程范围（当前不执行）

参考 MIT 6.031 Spring 2022：[Testing](https://web.mit.edu/6.031/www/sp22/classes/03-testing/)、[Specifications](https://web.mit.edu/6.031/www/sp22/classes/06-specifications/)、[ADT](https://web.mit.edu/6.031/www/sp22/classes/10-abstract-data-types/)、[表示不变量](https://web.mit.edu/6.031/www/sp22/classes/11-abstraction-functions-rep-invariants/)。旧笔记实际采用的 2016 来源照原记录保留。

| 原任务 | 原验收范围 |
|---|---|
| R0-01 最小环境与起点 | C/C++ 编译运行、GDB 单步、Python 测试；C 指针、数组、结构体与分配释放 |
| R0-02 规格与测试 | Testing/Specifications；非负权有向图的接口约定与契约测试 |
| R0-03 抽象与实现 | ADT/抽象函数/表示不变量；邻接表与边列表实现同一接口、共用测试 |

原图练习涉及重复/缺失节点、自环、负权输入、返回值所有权，要求修改返回集合不影响内部状态；不扩展 GUI、持久化或图算法。练习使用 C/C++，Python 公开项目按需；不安排 Java 作业或语言补课。schedule 1.2.2 导读仍只是备用材料，未替代原项目或构成完成证据。

## 接续与维护

- 日常只在 self-Learning 根目录拉取、提交和推送，先读总 STATUS；本目录没有独立 Git 仓库或另一份总进度。
- 当前按新主线启动 CS50x。若用户明确恢复本主题，阅读断点为 Testing 的 Choosing test cases by partitioning；环境按实际任务核验。
- 笔记仅保存知识和个人理解，区分独立产出与 AI 帮助；小节结束整理，不保留问答流水。
- 教学页面的相对链接和本地资源随目录整体保留；页面准备不等于用户已阅读或完成实验。
