# 学习资源

范围与顺序以 [LEARNING_PLAN](LEARNING_PLAN.md) 为准，总进度见 [STATUS](STATUS.md)。每个主题选一套主要讲解，配合原有习题、作业和官方文档；列出资料不等于增加必修课，也不代表已经学习。2026-11-16 按已确认计划整理；历史岗位证据保留原核查日期，不作为当前招聘状态。

## 共同核心：编程、算法与系统

| 主资源 | 使用范围 |
|---|---|
| [CS50x 2026](https://cs50.harvard.edu/x/2026/) · [大纲](https://cs50.harvard.edu/x/2026/syllabus/) | Week 1–5 的 C 相关原题补缺；已有能力通过练习确认。选学这些周不等于完成整课 |
| [CS106L Spring 2025](https://web.stanford.edu/class/archive/cs/cs106l/cs106l.1256/) | 现代 C++：类型与引用、容器、泛型、类、特殊成员、移动、RAII 和智能指针，配套原有作业 |
| [Programming: Principles and Practice Using C++，第 3 版](https://www.stroustrup.com/programming.html) | 补 CS106L 所需的函数、类等语言缺口，按需选原题；不额外完整修读或另学整套 GUI |
| [CS106B Spring 2025](https://web.stanford.edu/class/archive/cs/cs106b/cs106b.1256/) · [讲次索引](https://web.stanford.edu/class/archive/cs/cs106b/cs106b.1256/lecture_index) | 数据结构与基础算法主来源：递归、容器、树、堆、哈希、图与路径算法；使用该学期框架，区分 Stanford 教学库与 STL |
| [MIT 6.042J / Mathematics for Computer Science](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/) | 随算法选逻辑、证明、归纳、不变量、图、计数与基本概率的章节和原题 |
| [CSAPP 第 3 版官方站点](https://csapp.cs.cmu.edu/3e/) | 第 1–9 章选章：系统概览、表示、机器程序、执行与优化、存储层次、链接、进程及虚拟内存；具体深度见计划 |
| [CMU 15-213 Spring 2025 课表](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/schedule.html) · [自学实验](https://csapp.cs.cmu.edu/3e/labs.html) | 对应讲义、代码和工具导读；Cache Lab 按需使用允许自学的 Self-Study Handout，遵守公开边界 |
| [OSTEP 作者官网](https://pages.cs.wisc.edu/~remzi/OSTEP/) | 虚拟化、并发、持久化选章及对应习题/模拟器；覆盖文件、I/O、缓存与崩溃恢复的基本问题 |

查阅材料：[C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines) 用于资源管理和接口判断；[Compiler Explorer](https://godbolt.org/) 用于观察编译结果；[Missing Semester 调试与性能分析](https://missing.csail.mit.edu/2020/debugging-profiling/) 随练习短查。中文讲解可选 [Dr.Dng CSAPP 带学](https://www.bilibili.com/video/BV1hf4y1P7qW/)，此前只核对过目录，关键结论仍回查教材和官方资料。

## 数学：按当前问题选题

| 主资源 | 使用范围 |
|---|---|
| [MIT 18.06 Linear Algebra，Spring 2010](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/) | 向量、点积叉积、矩阵、线性方程、基、坐标变换、正交与投影，结合原有习题支撑几何、图形与数值计算 |
| [MIT 18.01SC Single Variable Calculus，Fall 2010](https://ocw.mit.edu/courses/18-01sc-single-variable-calculus-fall-2010/) | 导数、积分、近似、参数曲线与弧长等按需选题 |
| [MIT 18.02SC Multivariable Calculus，Fall 2010](https://ocw.mit.edu/courses/18-02sc-multivariable-calculus-fall-2010/) | 偏导数、曲面切向量与法向等按当前主题选题 |
| [3Blue1Brown 线性代数](https://www.3blue1brown.com/topics/linear-algebra) | 辅助建立直觉，配合上述课程计算与推导；不代替习题验证 |

数学随局部任务推进，不要求先完整修完这些课程再开始 OCCT 或 GAMES101 的入门内容。

## 当前工作：OCCT 7.9.x 与 CAM

工作版本已确认为 **OCCT 7.9.x**。以下官方文档固定到 `V7_9_0`，用于该系列的基础入口；具体 API、补丁差异和源码行为以工作实际版本核对。官网旧版链接可能跳到 8.x，不将跳转后的文档或 master 当作 7.9.x 的实践依据。

| 资源 | 使用范围 |
|---|---|
| [Quaoar 第 7 集](https://www.youtube.com/watch?v=ie7UCyg_b4Q) · [第 8 集](https://www.youtube.com/watch?v=qGPxaqyNMRE) | 全局概览辅助，结合官方文档辨认模块及关系；[第 4 集 AIS](https://www.youtube.com/watch?v=PXkv7fmURnI) 可按显示与拾取需求选看，视频不作为版本 API 依据 |
| [Introduction，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/introduction/introduction.md) | 先建立 Foundation、Modeling Data/Algorithms、Visualization、Data Exchange、Application Framework 的全局结构 |
| [Modeling Data，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/user_guides/modeling_data/modeling_data.md) | 几何与拓扑：gp、Geom、TopoDS，曲线/曲面参数，以及位置、方向、容差与 B-rep 的关系 |
| [Bottle Tutorial，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/tutorial/tutorial.md) | 从 Profile 到完整 Bottle，联系几何对象、Edge/Wire/Face/Solid、建模操作与结果检查 |
| [User Guides，V7_9_0](https://github.com/Open-Cascade-SAS/OCCT/blob/V7_9_0/dox/user_guides/user_guides.md) | 按需定位 Visualization、数据交换与 OCAF 文档；入门先理解显示/选择、导入导出、文档/属性/撤销等职责 |

入门后回到当前 CAM 的轮廓提取、表面提取、孔相关功能、拾取与转换，核对坐标、参数、拓扑归属及几何含义。先能使用和解释相关接口，再按真实故障进入算法诊断和源码；不要求先深入整个内核。示例采用独立合成模型，工作中的非公开代码和数据不进入公开仓库。

### CAM 工艺与五轴接口

| 资源 | 使用范围 |
|---|---|
| [天津大学《机械制造技术基础》课程大纲](https://www.icourse163.org/course/detail.htm?cid=1003482003) | 选看 1.3–1.4、2.2–2.4、5.2–5.5：工艺过程、装夹定位、工艺路线、余量与公差，配套相关原题 |
| [《机械 CAD/CAM 技术》第 5 版目录](https://www.cmpedu.com/books/book/5606280.htm) | 选读 7.3 刀位点计算和 7.4.2 刀具轨迹生成，理解设计几何、刀位与路径的关系 |
| [LinuxCNC 五轴运动学](https://linuxcnc.org/docs/stable/html/motion/5-axis-kinematics.html) | 遇到轴名、坐标系或 RTCP 时选一种机床构型对照；实际接口以对应设备与系统文档为准 |

## 图形学：提前选学 GAMES101 原作业 0–2

- [GAMES101 官方课程主页](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html)：第 2 讲线代、第 3/4 讲变换、第 5/6 讲光栅化，按选学内容补局部先修。
- 官方原作业：[作业 0](https://games-cn.org/forums/topic/graphics-intro-hw0/) · [作业 1](https://games-cn.org/forums/topic/graphics-intro-hw1/) · [作业 2](https://games-cn.org/forums/topic/graphics-intro-hw2/)。[作业 0 说明](https://games-cn.org/wp-content/uploads/2023/10/pa0.pdf) 涉及 C++、Eigen、CMake 和齐次变换。此前核对过发布入口，尚未运行作业包。
- Fundamentals of Computer Graphics，第 4 版（虎书）：对应数学、变换和光栅化章节及习题，按需查阅。

具备相应 C++、向量矩阵与变换基础即可开始这些局部作业；这不表示满足整门课的全部先修或完成整课。先做原作业，不额外重写另一套光栅器。

## CUDA：提前入门与独立深入路线

单 GPU 执行与正确性 → 架构与性能 → 并行算法与算子 → 系统应用。无需先完成全部 OCCT 或图形学；具体硬件、Toolkit 与工具兼容性在启动时核验。

| 资源 | 使用范围 |
|---|---|
| [PMPP 第 5 版出版社目录](https://www.inspectioncopy.elsevier.com/book/details/9780443439001) | 基础第 1–6 章，归约第 10 章；高级矩乘第 23 章后续按需，不把归约写成前六章内容 |
| [CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/index.html) · [Best Practices Guide](https://docs.nvidia.com/cuda/cuda-c-best-practices-guide/index.html) | 执行映射、内存、同步、传输和优化的官方依据；使用与实际 Toolkit 相符的文档 |
| [Compute Sanitizer](https://docs.nvidia.com/compute-sanitizer/ComputeSanitizer/index.html) | 按适用范围使用 memcheck、racecheck、initcheck、synccheck，并独立验证算法与数值结果 |
| [Nsight Systems](https://docs.nvidia.com/nsight-systems/UserGuide/index.html) · [Nsight Compute](https://docs.nvidia.com/nsight-compute/ProfilingGuide/index.html) | 先定位应用时间线、启动/等待/传输，再分析 kernel 指标及资源开销 |
| [NVIDIA 浮点与 IEEE 754](https://docs.nvidia.com/cuda/floating-point/index.html) | 舍入、FMA、CPU/GPU 差异与编译选项；同样辅助 CPU 几何数值判断 |
| [CCCL](https://nvidia.github.io/cccl/) | 后续扫描、归约等并行原语与性能比较 |
| [cuBLAS/cuBLASLt](https://docs.nvidia.com/cuda/cublas/index.html) | 矩乘和线性代数库基线，比较前匹配布局、精度与计时范围 |
| [CUTLASS](https://docs.nvidia.com/cutlass/latest/overview.html) | 分块 GEMM 之后研究布局、数据复用、CuTe 与架构相关优化 |
| [PyTorch 自定义 C++/CUDA 算子](https://docs.pytorch.org/tutorials/advanced/cpp_custom_ops.html) | 选择算子方向后使用，先理解张量语义，分别验证注册与数值结果 |

## 开源与岗位：辅助观察应用

开源入口按当前问题选读，不按星数排序，也不计入已完成的学习进度：

| 项目 | 局部用途 |
|---|---|
| [FreeCAD](https://github.com/FreeCAD/FreeCAD) · [Part Box 示例](https://github.com/FreeCAD/FreeCAD/blob/main/src/Mod/Part/App/FeaturePartBox.cpp) | 观察属性、重算、OCCT 建模和结果更新的上层集成；该项目的当前分支示例不代替工作版本 API 文档 |
| [CUDA Samples](https://github.com/NVIDIA/cuda-samples) | 按当前 Toolkit 选例子，核对索引、边界输入、数据移动和 CPU 参考结果 |
| [CUTLASS 示例](https://github.com/NVIDIA/cutlass/tree/main/examples) | CUDA 算子性能阶段再选用，理解布局并对照参考结果 |

2026-11-09 的历史岗位样本仅辅助理解工作要求，未在本轮重新核验是否仍开放，不用于推断市场规模或新增课程：

- [浩辰招聘官网](https://www.gstarcad.com/joinus/)：历史 C++ 岗位涉及需求、设计、实现、调试与测试，可用于校准工程练习深度。
- [柏楚校招入口](https://fscut.zhiye.com/campus/jobs)：当时几何算法岗位索引涉及数据结构、几何/数值计算、偏置、求交与布尔；直接页面未取得可读正文，保留此证据边界。
- [NVIDIA Graphics Tools，JR2017973](https://nvidia.wd5.myworkdayjobs.com/en-US/NVIDIAExternalCareerSite/job/Graphics-Tools-Software-Engineer_JR2017973)：当时官方索引涉及 C++、图形 API、Linux 系统知识及调试性能诊断；直接页面未取得可读正文。

## 资料与成果管理

课程成果统一放在 `courses/<course>/`，实际开课后才创建目录并在总 STATUS 登记。默认通过本仓库同步文档接续；独立项目或需隔离的受限作业才另设仓库。

可阅读不等于可公开复制或公布答案。按课程规则处理框架、测试、实验包与解答；公开仓库只保存允许公开的内容，不复制公司代码或客户数据。综合实践采用独立实现和合成数据。
