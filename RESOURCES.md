# 学习资源

当前范围以 [LEARNING_PLAN](LEARNING_PLAN.md) 为准。每个主题选一套主要讲解，书籍/官方文档用于查证和习题；不因列出资源而增加必修课程。2026-11-09 核查了下列核心官方入口，未下载课程实验包、运行测试或核验本机学习环境。

## 阶段 1

| 资源 | 用法 |
|---|---|
| [CS50x 2026](https://cs50.harvard.edu/x/2026/) · [大纲](https://cs50.harvard.edu/x/2026/syllabus/) | 主课；按每周 problem set 与 final project 验证。完整课包含 C、Python、SQL、Web，不把 C 部分等同于全课 |
| [3Blue1Brown 线代](https://www.3blue1brown.com/topics/linear-algebra) | 建立向量、线性变换、矩阵和基的直觉，计算练习配合虎书 |
| C Programming: A Modern Approach，K. N. King | C 问题的文字参考，不通读，不要求购买 |
| Crash Course Computer Science | 可选科普，不是开课前置 |

CS50x 的年份入口本次重定向到官方当前页面；正式开课以当时题目和工具命令为准，跨年先查官方衔接政策。采用课程提供的检查反馈，不代填完成记录或生成作业答案。公开记录只保存可公开的笔记、进度与独立练习；作业提交及展示遵循课程规则。

## 阶段 2：系统

| 资源 | 用法 |
|---|---|
| CSAPP 第 3 版 · [官方站点](https://csapp.cs.cmu.edu/3e/) | 重点第 6/7/9/12 章及其习题，必要前置按计划补齐 |
| [CMU 15-213 Spring 2025 课表](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/schedule.html) | 按主题取讲义、代码、工具导读；视频可访问性开课时核对 |
| [CSAPP 自学实验入口](https://csapp.cs.cmu.edu/3e/labs.html) | Cache Lab 按需选做，只使用 Self-Study Handout；不恢复旧四实验必修清单 |
| [OSTEP 作者官网](https://pages.cs.wisc.edu/~remzi/OSTEP/) | 虚拟化、并发的书籍与对应作业/模拟器；持久化按需查阅 |
| [IIT Bombay OS 讲授](https://www.cse.iitb.ac.in/~mythili/os/) | Part A–D 基于 OSTEP，Part X 用 xv6 **x86** 举例；不能照搬其代码到 RISC-V |
| [MIT 6.1810 2025 课表](https://pdos.csail.mit.edu/6.1810/2025/schedule.html) · [工具](https://pdos.csail.mit.edu/6.1810/2025/tools.html) | xv6 的匹配教材、RISC-V/QEMU 与环境说明 |
| [page tables](https://pdos.csail.mit.edu/6.1810/2025/labs/pgtbl.html) · [thread](https://pdos.csail.mit.edu/6.1810/2025/labs/thread.html) | 两个选定 lab；配套代码分支和测试不可混用其他年份。先读页表、Scheduling 及指定源文件；按章节名查找，旧页面章号可能与新版书不同 |
| [Compiler Explorer](https://godbolt.org/) · Inside the C++ Object Model，Stanley B. Lippman | 对象布局、虚函数的实现观察与历史机制参考，按需选读，不外推为 C++ 标准保证 |

保留先前用户提供的 [Dr.Dng CSAPP 中文带学](https://www.bilibili.com/video/BV1hf4y1P7qW/) 作为可选解释入口；此前只核对过目录，未逐集审校。本轮范围以书籍和官方资料为准，同主题不重复观看整套课程。

## 阶段 2：图形学

- [GAMES101 官方课程主页](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html)：第 2 讲线代，第 3/4 讲变换，第 5/6 讲光栅化；页面有讲义与视频入口。官方先修涉及线代、微积分、算法和数据结构，本计划按选学内容补缺，不宣称只看线代视频就满足整课前置。
- 官方作业入口：[作业 0](https://games-cn.org/forums/topic/graphics-intro-hw0/) · [作业 1](https://games-cn.org/forums/topic/graphics-intro-hw1/) · [作业 2](https://games-cn.org/forums/topic/graphics-intro-hw2/)。[作业 0 说明](https://games-cn.org/wp-content/uploads/2023/10/pa0.pdf) 涉及 C++、Eigen、CMake 及齐次变换。已核对发布入口，未运行或完整审阅压缩包内的实现和测试。
- Fundamentals of Computer Graphics，第 4 版（虎书）：对应数学、变换、光栅化章节及习题。先完成原作业，再按实际需要扩展；不额外重写另一套光栅器。

## 阶段 3

| 资源 | 用法 |
|---|---|
| [PMPP 第 5 版出版社目录](https://www.inspectioncopy.elsevier.com/book/details/9780443439001) | 2026-06-03 出版；Wen-mei W. Hwu、David B. Kirk、Izzat El Hajj。基础第 1–6 章，归约第 10 章；高级矩乘第 23 章按需，不能声称前六章覆盖归约 |
| [CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/index.html) | 执行模型、内存、同步及当前 API 的官方依据；使用与实际 Toolkit 相符的文档 |
| [Nsight Compute Profiling Guide](https://docs.nvidia.com/nsight-compute/ProfilingGuide/index.html) | 报告、指标意义、采集方式与工具开销；先正确，再分析和优化 |
| [NVIDIA Floating Point and IEEE 754](https://docs.nvidia.com/cuda/floating-point/index.html) | 舍入、FMA、CPU/GPU 差异与编译选项的首选免费资料 |
| [Floating Point Numerics for Games and Simulations](https://www.routledge.com/Floating-Point-Numerics-for-Games-and-Simulations/Badizadegan/p/book/9781003565543) | Nima Badizadegan，CRC Press，2025；选查数值误差与性能，不必为几小时回顾购买或通读 |
| CUDA by Example | 轻量历史示例，API/构建以当前官方文档为准，不直接承诺旧代码可运行 |
| Computational Geometry in C，Joseph O'Rourke | CAM 几何问题按需参考，不新增计算几何整课 |

PMPP 相关 Applied Parallel Programming / Heterogeneous Parallel Programming 视频可按同一主题辅助，具体授课年份、播放列表和作业版次在开课时匹配。GPU MODE / GPU Puzzles 是可选练习来源，本轮未逐项核验，不纳入三个 kernel 的强制验收。

## 历史成果与资料边界

[foundations](https://github.com/W-yf/foundations) 保留旧 R0 Testing 笔记和来源；其课程范围已退出当前主线。旧离散/算法、网络、数据库及其他候选资源可从 Git 历史查询，不作为待补清单。

课程资料可阅读不等于可公开复制或公布答案。使用实验时按当前课程规则处理框架、测试和解答；公开仓库只保存允许公开的内容，不复制公司代码或客户数据。CAM 收束采用独立实现和合成数据。
