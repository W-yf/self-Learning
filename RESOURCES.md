# 学习资源

范围与顺序以 [LEARNING_PLAN](LEARNING_PLAN.md) 为准，总进度见 [STATUS](STATUS.md)，路线图见 [交互图](docs/learning-roadmap.html) / [SVG](docs/learning-roadmap.svg)。每个主题选一套主要讲解，配合原有习题、作业和官方文档；列出资料不等于增加必修课，也不代表已经学习。2026-11-16 按已确认计划整理。

## 共同核心：编程、系统与算法

主线依次为 C 内存补缺、现代 C++、CSAPP 第 1–9 章、OSTEP 与同步、CS106B 算法。系统原题需要的数组、结构体、栈/队列/树概念与复杂度随题先补，不等待算法整课；MCS 与软件工程分段嵌入。

| 主资源 | 使用范围 |
|---|---|
| [CS50x 2026](https://cs50.harvard.edu/x/2026/) · [大纲](https://cs50.harvard.edu/x/2026/syllabus/) | 从 Week 1–5 的 C 相关原题选取指针、数组、结构体、内存与调试补缺；已有能力通过练习确认。选学这些周不等于完成整课 |
| [CS106L Spring 2025](https://web.stanford.edu/class/archive/cs/cs106l/cs106l.1256/) | 现代 C++：类型与引用、容器、泛型、类、特殊成员、移动、RAII 和智能指针，配套原有作业 |
| [Programming: Principles and Practice Using C++，第 3 版](https://www.stroustrup.com/programming.html) | 补 CS106L 所需的函数、类等语言缺口，按需选原题；不额外完整修读或另学整套 GUI |
| [CSAPP 第 3 版官方站点](https://csapp.cs.cmu.edu/3e/) | 第 1–9 章按计划选择深度：系统概览、表示、机器程序、执行与优化、存储层次、链接、进程及虚拟内存 |
| [CMU 15-213 Spring 2025 课表](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/schedule.html) · [自学实验](https://csapp.cs.cmu.edu/3e/labs.html) | 对应讲义、代码和工具导读；Cache Lab 按需使用允许自学的 Self-Study Handout，遵守公开边界 |
| [OSTEP 作者官网](https://pages.cs.wisc.edu/~remzi/OSTEP/) | 虚拟化、并发、持久化选章及对应习题/模拟器；覆盖文件、I/O、缓存与崩溃恢复的基本问题 |
| [CS106B Spring 2025](https://web.stanford.edu/class/archive/cs/cs106b/cs106b.1256/) · [讲次索引](https://web.stanford.edu/class/archive/cs/cs106b/cs106b.1256/lecture_index) | 系统与 OS 主线后展开的数据结构与基础算法：递归、容器、树、堆、哈希、图与路径算法；系统题所需概念可提前查阅。使用该学期框架，区分 Stanford 教学库与 STL |
| [MIT 6.042J / Mathematics for Computer Science](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/) | 随共同核心选逻辑、证明、归纳、不变量、图、计数与基本概率的章节和原题，不另叠加完整课程 |

查阅材料：[C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines) 用于资源管理和接口判断；[Compiler Explorer](https://godbolt.org/) 用于观察编译结果；[Missing Semester 调试与性能分析](https://missing.csail.mit.edu/2020/debugging-profiling/) 随练习短查。中文讲解可选 [Dr.Dng CSAPP 带学](https://www.bilibili.com/video/BV1hf4y1P7qW/)，此前只核对过目录，关键结论仍回查教材和官方资料。

## 共同核心：软件设计与工程基础

本单元选读与原有练习分段嵌入共同核心；时机与范围以 LEARNING_PLAN 为准。

| 资源 | 使用范围与实践性质 |
|---|---|
| [Ian Sommerville《软件工程》第 10 版目录](https://www.pearson.com/en-us/pearsonplus/p/9780137503148) | 主教材：第 4 章需求、第 5 章基本建模、第 6 章架构、第 7 章对象与接口；第 22、23 章选风险、协作、任务依赖、估时与迭代。第 9、25 章维护、变更、构建与发布按需查阅。使用对应章节原有习题；译本按章名核对 |
| [作者配套资料](https://software-engineering-book.com/intro/) · [视频](https://software-engineering-book.com/videos/) | 案例、讲义、视频与部分习题解答。区分作者制作和推荐的他人视频；配套资料公开不等于整本书免费，教材须合法获取 |
| [《软件设计的哲学》作者课程讨论页](https://web.stanford.edu/~ouster/cs190-winter23/lectures/aposd/) | 设计补充：复杂性、接口与实现、信息隐藏、深浅模块、通用与专用设计、错误处理、命名及设计意图；按约束判断适用性 |
| [Stanford CS190，Winter 2023](https://web.stanford.edu/~ouster/cs190-winter23/) · [PrimeGenerator 原始练习](https://web.stanford.edu/~ouster/cs190-winter23/lectures/primes/) | 按需选用教师发布的代码审查练习，并非自动评分 lab；完整课程依赖实现、审查与修改反馈，Raft 等项目留作进阶选修 |
| [CMU 17-313](https://cmu-313.github.io/) | 项目规划、规格与设计文档讲义按需查阅；2026 年公开课程包含团队协作、需求访谈与开源项目，不作为本轮完整必修课 |

练习以主教材原有分析、建模和方案比较题为主；设计题可能存在多个合理方案。C++ 所有权、生命周期及既有 Git 内容与原单元衔接，不重复安排；不额外建立架构练习项目。

## CPU 并发：必修原实验与选修阅读

OSTEP 同步及 C++ 线程、锁、条件变量具备后即可进入 Part A，不等待 CS106B 整课。协程、SPSC、Part B 与 Taskflow 属于后续选修，不挤占本轮 CUDA 入门。

| 资源 | 使用范围与实践性质 |
|---|---|
| [Stanford CS149 Assignment 2](https://github.com/stanford-cs149/asst2) | 必修 Part A 原实验：每次创建线程 → 线程池 spinning → 线程池 sleeping，配套原测试；理解任务分配、同步与线程生命周期。Part B 的依赖任务图为选修，不将整门 CS149 列为必修 |
| [Taskflow 官方文档](https://taskflow.github.io/taskflow/) · [源码](https://github.com/taskflow/taskflow) | Part B 后选读成熟库的任务图、executor 与调度实现；属于库阅读，不是课程原题 |
| [David Mazières：My tutorial and take on C++20 coroutines](https://www.scs.stanford.edu/~dm/blog/c%2B%2B-coroutines.html) | C++20 协程选修：作者教程与示例，理解 handle、promise、挂起/恢复及对象生命周期；不是 Stanford 课程 lab |
| [rigtorp/SPSCQueue](https://github.com/rigtorp/SPSCQueue) | 选修阅读与验证：先理解 acquire/release，再读单生产者、单消费者有界队列的源码及原测试；成熟库不是原题，不扩展到 MPMC |

## 数学与曲线曲面

先学 18.06 完整主干，配合 3Blue1Brown 建立直觉，再依次学习解析几何、18.01SC、18.02SC 必要部分、Shene/Farin 曲线曲面。应用当前所需的叉积、直线与平面可提前查后续教材并做相应原题。

| 主资源 | 使用范围 |
|---|---|
| [MIT 18.06 Linear Algebra，Spring 2010](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/) | 完整主干与原有习题：线性方程、矩阵、向量空间、正交投影、行列式、特征值与特征向量、SVD 等；课程题号对应 Strang《Introduction to Linear Algebra》第 4 版，其他版本须按题意核对 |
| [3Blue1Brown 线性代数](https://www.3blue1brown.com/topics/linear-algebra) | 辅助建立直觉，配合 18.06 计算与推导；不代替习题验证 |
| [吕林根、许子道《解析几何》第 5 版，出版社入口](https://xuanshu.hep.com.cn/front/book/findBookDetails?bookId=5bc22e30f18f967ee7f37856) | 线代主干后的几何主教材：向量与坐标、轨迹与方程、平面与空间直线、常见二次曲线曲面及相应原题；一般理论按计划选择深度 |
| [MIT 18.01SC Single Variable Calculus，Fall 2010](https://ocw.mit.edu/courses/18-01sc-single-variable-calculus-fall-2010/) | 完整单变量微积分基础与原题：极限、导数、积分、积分方法和应用、序列与级数等 |
| [MIT 18.02SC Multivariable Calculus，Fall 2010](https://ocw.mit.edu/courses/18-02sc-multivariable-calculus-fall-2010/) | 必要部分及原题：向量与参数曲线、偏导、链式法则、梯度和切平面；参数曲面法向由 CAGD 内容衔接，不要求完整修读整课 |
| [Shene：Introduction to Computing with Geometry Notes](https://pages.mtu.edu/~shene/COURSES/cs3621/NOTES/) · [Bézier 原题](https://pages.mtu.edu/~shene/COURSES/cs3621/NOTES/spline/Bezier/problems.html) · [B-spline 原题](https://pages.mtu.edu/~shene/COURSES/cs3621/NOTES/spline/B-spline/problems.html) | 曲线曲面主要讲解与原题：参数曲线、连续性、Bézier、de Casteljau、B-spline、节点与 de Boor，延伸到有理曲线/NURBS 和曲面基本概念 |
| [Farin《Curves and Surfaces for CAGD》第 5 版目录](https://www.farinhansford.com/books/cagd/toc.html) | 曲线曲面参考教材，按 Shene 当前主题查阅推导、性质与原题；不再叠加完整修读 |

数学按计划分段推进，可在具备局部先修后穿插 OCCT 或图形入门；资源入口不代替计划中的完整基础范围。

## 当前工作：OCCT 7.9.x 与 CAM

工作版本已确认为 **OCCT 7.9.x**。以下官方文档固定到 `V7_9_0`，用于该系列的基础入口；具体 API、补丁差异和源码行为以工作实际版本核对。官网旧版链接可能跳到 8.x，不将跳转后的文档或 master 当作 7.9.x 的实践依据。

| 资源 | 使用范围 |
|---|---|
| [Quaoar 第 7 集](https://www.youtube.com/watch?v=ie7UCyg_b4Q) · [第 8 集](https://www.youtube.com/watch?v=qGPxaqyNMRE) | 全局概览辅助，结合官方文档辨认模块及关系；[第 4 集 AIS](https://www.youtube.com/watch?v=PXkv7fmURnI) 可按显示与拾取需求选看，视频不作为版本 API 依据 |
| [Introduction，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/introduction/introduction.md) | 先建立 Foundation、Modeling Data/Algorithms、Visualization、Data Exchange、Application Framework 的全局结构 |
| [Modeling Data，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/user_guides/modeling_data/modeling_data.md) | 几何与拓扑：gp、Geom、TopoDS，曲线/曲面参数，以及位置、方向、容差与 B-rep 的关系 |
| [Bottle Tutorial，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/tutorial/tutorial.md) | 官方教程示例：从 Profile 到完整 Bottle，联系几何对象、Edge/Wire/Face/Solid、建模操作与结果检查；与 Modeling Data 中的示例同属官方示例，不称课程作业 |
| [User Guides，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/user_guides/user_guides.md) | 按需定位 Visualization、数据交换与 OCAF 文档；入门先理解显示/选择、导入导出、文档/属性/撤销等职责 |

入门后回到当前 CAM 的轮廓提取、表面提取、孔相关功能、拾取与转换，核对坐标、参数、拓扑归属及几何含义。先能使用和解释相关接口，再按真实故障进入算法诊断和源码；不要求先深入整个内核。示例采用独立合成模型，工作中的非公开代码和数据不进入公开仓库。

### Qt Widgets 与显示集成

- [Qt Widgets Getting Started 原教程](https://doc.qt.io/qt-6/widgets-getting-started.html)：按官方 Notepad 教程学习窗口、布局、信号槽、菜单/动作和基本文件操作；属于官方教程，不是课程作业。使用与实际 Qt 版本匹配的文档。
- [官方 Hello GL2 示例](https://doc.qt.io/qt-6/qtopengl-hellogl2-example.html)：按显示集成需要理解 QOpenGLWidget 与 Qt/OpenGL 的衔接；不另加完整 GUI 或图形框架课程。
- [OCCT Qt samples，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/tree/V7_9_0/samples/qt)：固定版本的官方集成示例入口，含 Tutorial、OCCTOverview、Common 等目录；按 Qt/OCCT 窗口、显示和交互集成需要选读，属于官方示例。

### CAM 工艺与五轴接口

| 资源 | 使用范围 |
|---|---|
| [天津大学《机械制造技术基础》课程大纲](https://www.icourse163.org/course/detail.htm?cid=1003482003) | 选看 1.3–1.4、2.2–2.4、5.2–5.5：工艺过程、装夹定位、工艺路线、余量与公差，配套相关原题 |
| [《机械 CAD/CAM 技术》第 5 版目录](https://www.cmpedu.com/books/book/5606280.htm) | 选读 7.3 刀位点计算和 7.4.2 刀具轨迹生成，理解设计几何、刀位与路径的关系 |
| [LinuxCNC 五轴运动学](https://linuxcnc.org/docs/stable/html/motion/5-axis-kinematics.html) | 遇到轴名、坐标系或 RTCP 时选一种机床构型对照；实际接口以对应设备与系统文档为准 |

## 图形学：GAMES101 原作业与 LearnOpenGL

- [GAMES101 官方课程主页](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html)：对应线代、变换、光栅化、插值、着色与纹理的讲解，按作业补先修。
- 官方原作业：[作业 0](https://games-cn.org/forums/topic/graphics-intro-hw0/) · [作业 1](https://games-cn.org/forums/topic/graphics-intro-hw1/) · [作业 2](https://games-cn.org/forums/topic/graphics-intro-hw2/) · [作业 3](https://games-cn.org/forums/topic/graphics-intro-hw3/) 基础要求；[作业 4](https://games-cn.org/forums/topic/graphics-intro-hw4/) Bézier 可选。[作业 0 说明](https://games-cn.org/wp-content/uploads/2023/10/pa0.pdf) 涉及 C++、Eigen、CMake 和齐次变换。已核对发布入口，尚未运行作业包。
- [LearnOpenGL 作者教程](https://learnopengl.com/)：Getting started、Lighting、Model Loading，以及 Advanced OpenGL 的 Depth testing、Blending、Framebuffers；教程示例与练习用于掌握 OpenGL 实时渲染流程，不将整站设为必修。
- Fundamentals of Computer Graphics，第 4 版（虎书）：对应数学、变换和光栅化章节及习题，按需查阅。

具备相应 C++、向量矩阵与变换基础即可开始局部作业；不将选做范围写成完成整门课程。以原作业和教程为主，不额外重写另一套光栅器。

## CUDA：明确安排的第一轮与后续深入资源

第一轮按 A 执行与正确性 → B 分块与归约 → C profiling 推进；后续再按实际需要进入并行算子与系统应用。具备局部 C++、数组/指针、调试与 CPU 参考实现能力即可启动；默认在图形第一段后轮换，不等待数学、系统、图形或线程池全部完成。具体硬件、Toolkit 与工具兼容性在启动时核验。

| 资源 | 使用范围 |
|---|---|
| [PMPP 第 5 版出版社目录](https://www.inspectioncopy.elsevier.com/book/details/9780443439001) | 基础第 1–6 章，归约第 10 章；高级矩乘第 23 章后续按需，不把归约写成前六章内容 |
| [OLCF / NERSC CUDA Training Series 原实验](https://github.com/olcf/cuda-training-series/tree/master/exercises) | 第一轮 A：hw1 vector add / naive GEMM；B：hw2 tiled GEMM 与 hw5 reduction；C：hw3 profiling。hw5 原题即要求将给定 sum reduction 改成 max，不另冒称自拟练习。该实验来自 OLCF 培训，不是 PMPP 第 5 版配套作业 |
| [CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/index.html) · [Best Practices Guide](https://docs.nvidia.com/cuda/cuda-c-best-practices-guide/index.html) | 执行映射、内存、同步、传输和优化的官方依据；使用与实际 Toolkit 相符的文档 |
| [Compute Sanitizer](https://docs.nvidia.com/compute-sanitizer/ComputeSanitizer/index.html) | 按适用范围使用 memcheck、racecheck、initcheck、synccheck，并独立验证算法与数值结果 |
| [Nsight Systems](https://docs.nvidia.com/nsight-systems/UserGuide/index.html) · [Nsight Compute](https://docs.nvidia.com/nsight-compute/ProfilingGuide/index.html) | 先定位应用时间线、启动/等待/传输，再分析 kernel 指标及资源开销 |
| [NVIDIA 浮点与 IEEE 754](https://docs.nvidia.com/cuda/floating-point/index.html) | 舍入、FMA、CPU/GPU 差异与编译选项；同样辅助 CPU 几何数值判断 |
| [CCCL](https://nvidia.github.io/cccl/) | 后续扫描、归约等并行原语与性能比较 |
| [cuBLAS/cuBLASLt](https://docs.nvidia.com/cuda/cublas/index.html) | 矩乘和线性代数库基线，比较前匹配布局、精度与计时范围 |
| [CUTLASS](https://docs.nvidia.com/cutlass/latest/overview.html) | 分块 GEMM 之后研究布局、数据复用、CuTe 与架构相关优化 |
| [PyTorch 自定义 C++/CUDA 算子](https://docs.pytorch.org/tutorials/advanced/cpp_custom_ops.html) | 选择算子方向后使用，先理解张量语义，分别验证注册与数值结果 |

CS149 circle renderer 仅作为后续 CUDA 实践候选，启动时再核对原作业与公开边界；量化应用同属应用候选，不追加必修范围。

## 开源与岗位：辅助观察应用

开源入口按当前问题选读，不按星数排序，也不计入已完成的学习进度：

| 项目 | 局部用途 |
|---|---|
| [FreeCAD](https://github.com/FreeCAD/FreeCAD) · [Part Box 示例](https://github.com/FreeCAD/FreeCAD/blob/main/src/Mod/Part/App/FeaturePartBox.cpp) | 观察属性、重算、OCCT 建模和结果更新的上层集成；该项目的当前分支示例不代替工作版本 API 文档 |
| [CUDA Samples](https://github.com/NVIDIA/cuda-samples) | 按当前 Toolkit 选例子，核对索引、边界输入、数据移动和 CPU 参考结果 |
| [CUTLASS 示例](https://github.com/NVIDIA/cutlass/tree/main/examples) | CUDA 算子性能阶段再选用，理解布局并对照参考结果 |

岗位信息仅用于辅助理解实际应用与工程要求，不据此追加必修课程或推断市场规模。需要时从 BOSS、前程无忧（51job）、猎聘与企业官网核验，地区覆盖江苏、浙江、上海、北京、广州、合肥、深圳；月薪大于 17k 且不高于 30k 时优先双休、每天 8 小时，超过 30k 可放宽工时要求。岗位观察不以学历或项目 star 数作为筛选依据；具体岗位条件以当时原始招聘信息为准。

## 资料与成果管理

课程成果统一放在 `courses/<course>/`，实际开课后才创建目录并在总 STATUS 登记。默认通过本仓库同步文档接续；独立项目或需隔离的受限作业才另设仓库。

可阅读不等于可公开复制或公布答案。按课程规则处理框架、测试、实验包与解答；公开仓库只保存允许公开的内容，不复制公司代码或客户数据。综合实践采用独立实现和合成数据。
