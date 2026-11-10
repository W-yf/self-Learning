# 学习资源

当前范围以已确认的 [LEARNING_PLAN](LEARNING_PLAN.md) 为准。每个主题选一套主要讲解，书籍/官方文档用于查证和习题；不因列出资源而增加必修课程。2026-11-09 核查课程入口、下列招聘证据及 GitHub 项目；未下载实验包、运行样例或核验本机学习环境。

## 最小核心：编程启动

规划主要依据 [CS 自学指南学习规划](https://csdiy.wiki/CS学习规划/) 与 [Teach Yourself CS 中文版](https://github.com/izackwu/TeachYourselfCS-CN/blob/master/TeachYourselfCS-CN.md)，本轮已核对原文。前者用于课程地图和先修选择，后者用于学科联系与系统基础取舍；下列范围是本计划的选择，不是两份指南共同规定的必修组合。

| 资源 | 用法 |
|---|---|
| [CS50x 2026](https://cs50.harvard.edu/x/2026/) · [大纲](https://cs50.harvard.edu/x/2026/syllabus/) | 按 Week 1–5 的 C 相关原题补缺，Week 0 作背景；已有能力通过练习确认。Python 服务算法与脚本，SQL/Web/final project 按完整修课意愿续学，部分完成不等于整课完成 |
| C Programming: A Modern Approach，K. N. King | C 问题的文字参考，不通读，不要求购买 |
| Crash Course Computer Science | 可选科普，不是开课前置 |

CS50x 的年份入口本次重定向到官方当前页面；正式开课以当时题目和工具命令为准，跨年先查官方衔接政策。采用课程提供的检查反馈，不代填完成记录或生成作业答案。公开记录只保存可公开的笔记、进度与独立练习；作业提交及展示遵循课程规则。

## 最小核心：C++、算法与系统

| 资源 | 用法 |
|---|---|
| [CS106L Spring 2025](https://web.stanford.edu/class/archive/cs/cs106l/cs106l.1256/) | 现代 C++ 主来源；选择类型/引用、类、容器、泛型、特殊成员、移动、RAII 与智能指针的讲次和原有作业；基础函数与类知识先补齐 |
| [Programming: Principles and Practice Using C++，第 3 版](https://www.stroustrup.com/programming.html) | 补 CS106L 所需的语言缺口，按需选原题；不额外完整修读，不另学整套 GUI |
| [C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines) | 资源管理、接口、类与并发的查阅材料；不是按条背诵的课程 |
| [CS106B Spring 2025](https://web.stanford.edu/class/archive/cs/cs106b/cs106b.1256/) · [讲次索引](https://web.stanford.edu/class/archive/cs/cs106b/cs106b.1256/lecture_index) | 数据结构与基础算法主来源；第二门编程课，包含递归、容器、树/堆、哈希、图与路径算法；按该学期框架完成原题，Stanford 教学库与 STL 分别理解 |
| [MIT 6.006 Spring 2020](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/) · The Algorithm Design Manual，Steven Skiena | 6.006 是替代课程，Skiena 是问题参考；不与 CS106B 重复完整修读 |
| [MIT 6.042J / Mathematics for Computer Science](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/) | 随算法选逻辑、归纳、不变量、图、计数与基本概率的原有章节和习题 |
| CSAPP 第 3 版 · [官方站点](https://csapp.cs.cmu.edu/3e/) | 第 2/3 章建立表示与机器程序基础，第 4/5 章选学执行模型与优化，再接缓存、链接、进程、虚拟内存和并发；范围见计划 |
| [CMU 15-213 Spring 2025 课表](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/schedule.html) | 按主题取讲义、代码、工具导读；视频可访问性开课时核对 |
| [CSAPP 自学实验入口](https://csapp.cs.cmu.edu/3e/labs.html) | Cache Lab 按需选做，使用允许自学的 Self-Study Handout，遵守其公开范围 |
| [OSTEP 作者官网](https://pages.cs.wisc.edu/~remzi/OSTEP/) | 虚拟化、并发和持久化基础；选对应作业/模拟器，文件、I/O、缓存与崩溃恢复的基本问题纳入核心 |
| [Missing Semester：Debugging and Profiling](https://missing.csail.mit.edu/2020/debugging-profiling/) | 随当前练习短查调试、日志、分析和测量工具；不新增完整工具必修课 |
| [IIT Bombay OS 讲授](https://www.cse.iitb.ac.in/~mythili/os/) | Part A–D 基于 OSTEP，Part X 用 xv6 **x86** 举例；不能照搬其代码到 RISC-V |
| [MIT 6.1810 2025 课表](https://pdos.csail.mit.edu/6.1810/2025/schedule.html) · [工具](https://pdos.csail.mit.edu/6.1810/2025/tools.html) | xv6 的匹配教材、RISC-V/QEMU 与环境说明 |
| [page tables](https://pdos.csail.mit.edu/6.1810/2025/labs/pgtbl.html) · [thread](https://pdos.csail.mit.edu/6.1810/2025/labs/thread.html) | 系统实现选做；先完成 OSTEP 习题，需要深入时选择一个。配套代码分支和测试不可混用其他年份；先读指定章节 |
| [Compiler Explorer](https://godbolt.org/) · Inside the C++ Object Model，Stanley B. Lippman | 对象布局、虚函数的实现观察与历史机制参考，按需选读，不外推为 C++ 标准保证 |

保留先前用户提供的 [Dr.Dng CSAPP 中文带学](https://www.bilibili.com/video/BV1hf4y1P7qW/) 作为可选解释入口；此前只核对过目录，未逐集审校。本轮范围以书籍和官方资料为准，同主题不重复观看整套课程。

## 优先探索：OCCT

当前工作基于 OCCT，因此将其作为持续研究对象；研究深度由当前基础和实际问题决定。工作使用版本尚未确认，先在本地确认版本，再匹配源码标签与文档。下列 master 链接用于定位材料，不能直接当作工作版本的 API 依据。

| 官方资料 | 使用方式 |
|---|---|
| [文档总入口](https://dev.opencascade.org/doc/overview) | 按版本查阅概览、用户手册和 API Reference |
| [Bottle Tutorial](https://github.com/Open-Cascade-SAS/OCCT/blob/master/dox/tutorial/tutorial.md) | 初学从 Profile 小段开始，将点/曲线、拓扑构造与 C++ 值对象/handle 联系起来 |
| [User Guides](https://github.com/Open-Cascade-SAS/OCCT/blob/master/dox/user_guides/user_guides.md) | Foundation Classes、Modeling Data/Algorithms、Shape Healing、Mesh、Visualization、STEP/XDE 等按专题深入 |
| [Debugging tools and hints](https://github.com/Open-Cascade-SAS/OCCT/blob/master/dox/debug/debug.md) | 源码断点、形状检查与 DRAW 调试；需要回归时再使用匹配版本的测试体系 |

研究顺序与成果要求见 LEARNING_PLAN：基础接口与对象语义 → B-rep 数据模型 → 算法诊断与源码 → 专题研究。示例使用独立合成模型；FreeCAD 作为上层集成对照，libigl 作为网格处理对照。

## 细分探索：图形学

- [3Blue1Brown 线代](https://www.3blue1brown.com/topics/linear-algebra)：几何直觉，配合虎书原有计算练习；也可用于理解 OCCT 中的坐标与变换。
- [GAMES101 官方课程主页](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html)：第 2 讲线代，第 3/4 讲变换，第 5/6 讲光栅化；页面有讲义与视频入口。官方先修涉及线代、微积分、算法和数据结构，本计划按选学内容补缺，不宣称只看线代视频就满足整课前置。
- 官方作业入口：[作业 0](https://games-cn.org/forums/topic/graphics-intro-hw0/) · [作业 1](https://games-cn.org/forums/topic/graphics-intro-hw1/) · [作业 2](https://games-cn.org/forums/topic/graphics-intro-hw2/)。[作业 0 说明](https://games-cn.org/wp-content/uploads/2023/10/pa0.pdf) 涉及 C++、Eigen、CMake 及齐次变换。已核对发布入口，未运行或完整审阅压缩包内的实现和测试。
- Fundamentals of Computer Graphics，第 4 版（虎书）：对应数学、变换、光栅化章节及习题。先完成原作业，再按实际需要扩展；不额外重写另一套光栅器。

## 细分探索：CUDA 与高性能计算

CUDA 可作为独立深入方向。按计划中的执行与正确性、GPU 架构与性能、并行算法与算子、系统应用四层推进；资料按层使用，不要求一次读完。硬件和工具环境在实际启动时核验，不默认支持全部新架构特性。

浮点资料也适用于 CPU 几何与数值计算；单 GPU 基础先于多 GPU 和分布式。几何、渲染及 CUDA 的局部先修分别满足，不要求先完成全部图形学或 OCCT 才能学习 CUDA。

| 资源 | 用法 |
|---|---|
| [PMPP 第 5 版出版社目录](https://www.inspectioncopy.elsevier.com/book/details/9780443439001) | 2026-06-03 出版；Wen-mei W. Hwu、David B. Kirk、Izzat El Hajj。基础第 1–6 章，归约第 10 章；高级矩乘第 23 章按需，不能声称前六章覆盖归约 |
| [CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/index.html) | 执行模型、内存、同步及当前 API 的官方依据；使用与实际 Toolkit 相符的文档 |
| [CUDA Best Practices Guide](https://docs.nvidia.com/cuda/cuda-c-best-practices-guide/index.html) | 从并行化判断、数据传输到性能优化，配合当前练习理解带宽、资源与整体开销 |
| [Compute Sanitizer](https://docs.nvidia.com/compute-sanitizer/ComputeSanitizer/index.html) | memcheck、racecheck、initcheck、synccheck 按适用范围检查内存与同步；不替代算法和数值验证 |
| [Nsight Systems](https://docs.nvidia.com/nsight-systems/UserGuide/index.html) | CPU/GPU 时间线、启动、等待与传输，先定位应用整体问题 |
| [Nsight Compute Profiling Guide](https://docs.nvidia.com/nsight-compute/ProfilingGuide/index.html) | 报告、指标意义、采集方式与工具开销；先正确，再分析和优化 |
| [CCCL](https://nvidia.github.io/cccl/) | CUB/Thrust 等并行原语；作为扫描/归约等练习的语义和性能比较对象 |
| [cuBLAS/cuBLASLt](https://docs.nvidia.com/cuda/cublas/index.html) | 矩乘与相关线性代数库基线；匹配布局、精度和计时范围后比较 |
| [CUTLASS 官方文档](https://docs.nvidia.com/cutlass/latest/overview.html) | 分块 GEMM 之后研究局部实现、布局、CuTe 与架构相关优化 |
| [PyTorch 自定义 C++/CUDA 算子](https://docs.pytorch.org/tutorials/advanced/cpp_custom_ops.html) | 选择机器学习算子方向后使用；先具备张量与算子语义，分别验证注册行为和数值结果 |
| [NVIDIA Floating Point and IEEE 754](https://docs.nvidia.com/cuda/floating-point/index.html) | 舍入、FMA、CPU/GPU 差异与编译选项的首选免费资料 |
| [Floating Point Numerics for Games and Simulations](https://www.routledge.com/Floating-Point-Numerics-for-Games-and-Simulations/Badizadegan/p/book/9781003565543) | Nima Badizadegan，CRC Press，2025；选查数值误差与性能，不必为几小时回顾购买或通读 |
| CUDA by Example | 轻量历史示例，API/构建以当前官方文档为准，不直接承诺旧代码可运行 |
| Computational Geometry in C，Joseph O'Rourke | 几何处理问题按需参考，不新增计算几何整课 |

PMPP 相关 Applied Parallel Programming / Heterogeneous Parallel Programming 视频可按同一主题辅助，具体授课年份、播放列表和作业版次在开课时匹配。GPU MODE / GPU Puzzles 是可选练习来源，本轮未逐项核验。

### 进一步认识领域：暂不确定为职业目标

- 几何、渲染、仿真可视化：按所选问题继续使用 OCCT、libigl、GAMES101/虎书、Filament；需要时补微积分、微分方程和数值方法。
- 金融量化系统：[QuantLib](https://www.quantlib.org/) 用于认识 C++ 数值建模、定价与风险计算这一类软件；它不是完整行情、回测和交易系统。先了解职责与小例子，再决定是否增加金融、统计或网络系统课程。
- 模型量化与推理：[TensorRT 量化文档](https://docs.nvidia.com/deeplearning/tensorrt/latest/inference-library/work-with-quantized-types.html) 用于认识低精度类型、缩放与量化工作流，后续再连接算子和推理优化。

用户尚未确定“量化系统研发”所指领域，上述两项仅作区分与探索入口，不把其中任一项写成已选职业路线。GPU 是否适用须按具体计算与整体开销判断。

## GitHub 项目与知识入口

2026-11-09 通过 GitHub REST API 核对以下星数，六个仓库均未归档。星数仅作关注度快照；优先级由与当前工作及所选问题的关系决定，不据此推断岗位数量。以下是建议的局部学习入口，未执行或计入学习进度。

| 项目与星数 | 对应知识与用途 | 最小入口 |
|---|---|---|
| [FreeCAD](https://github.com/FreeCAD/FreeCAD) · 35,274 | 参数化 CAD 产品；连接文档/属性、几何内核、界面与重算机制 | [FeaturePartBox.cpp](https://github.com/FreeCAD/FreeCAD/blob/main/src/Mod/Part/App/FeaturePartBox.cpp)：追踪尺寸属性→重算→OCCT 建模→结果更新，无需先编译整个工程 |
| [OCCT](https://github.com/Open-Cascade-SAS/OCCT) · 3,144 | CAD/CAM/CAE 几何平台；几何与拓扑、精度、数据交换及可视化 | [Bottle Tutorial](https://github.com/Open-Cascade-SAS/OCCT/blob/master/dox/tutorial/tutorial.md) 的 Profile 部分：点/曲线→Edge/Wire，观察构造状态和失败处理 |
| [libigl](https://github.com/libigl/libigl) · 5,121 | 三角网格与几何处理；线代、稀疏矩阵、离散算子 | 先看[网格表示与法线教程](https://libigl.github.io/tutorial/)；具备稀疏线性系统基础后再看 [205_Laplacian](https://github.com/libigl/libigl/blob/main/tutorial/205_Laplacian/main.cpp)，分析算子和误差 |
| [Filament](https://github.com/google/filament) · 20,714 | 实时渲染；顶点数据、材质、相机、渲染流程与资源生命周期 | [hellotriangle.cpp](https://github.com/google/filament/blob/main/samples/hellotriangle.cpp)：修改顶点/颜色，解释 buffer→renderable→scene/view/camera 的关系及释放顺序 |
| [CUDA Samples](https://github.com/NVIDIA/cuda-samples) · 9,748 | 可选的 GPU 通用计算实践；执行映射、数据移动、同步 | [vectorAdd.cu](https://github.com/NVIDIA/cuda-samples/blob/master/cpp/0_Introduction/vectorAdd/vectorAdd.cu)：核对索引、非整块输入和 CPU 参考；本次所读版本使用 Unified Memory，不能当作显式拷贝示例 |
| [CUTLASS](https://github.com/NVIDIA/cutlass) · 10,713 | 后续专门的高性能矩乘/张量计算；布局、分块与数据复用 | 仅在已学 CUDA 且选定算子性能方向后看 [basic_gemm.cu](https://github.com/NVIDIA/cutlass/blob/main/examples/00_basic_gemm/basic_gemm.cu)，解释矩阵布局并对照参考结果 |

OCCT 是当前工作的优先研究对象，FreeCAD 提供产品集成对照，libigl/Filament 提供几何与渲染探索入口；CUDA Samples 到 CUTLASS 对应 CUDA 分支从入门到算子性能的不同层次。以上是本计划的使用建议，不是项目作者规定的学习路线。

## 招聘岗位：辅助观察知识如何用于工作

调研日期：2026-11-09。只考虑江苏、浙江、上海、北京、广州、合肥；来源限定 BOSS直聘、前程无忧、猎聘和公司官网。下表不是求职清单或市场统计，也不要求覆盖每个地区。岗位负责说明能力在不同工作中的用途，课程范围与先修关系由学习计划决定。

| 样本与来源 | 地点与资历 | 可核对的能力要求及用途 | 证据边界 |
|---|---|---|---|
| 浩辰 [C++中高级软件工程师](https://www.gstarcad.com/joinus/) | 北京；本科，3年以上，至少2年 C++ 经验 | 需求分析、方案设计与评审、关键模块实现、代码审核；说明工业软件研发需要语言与工程能力共同支撑 | 官网正文可读；该岗位另列的非目标城市不纳入；未见明确发布日期 |
| 柏楚 [27校招-几何算法工程师 J10838](https://fscut.zhiye.com/campus/jobs) | 上海；校招，理工科本科及以上 | 数据结构与算法、面向对象语言、计算几何/数值计算；偏置、求交、裁剪、布尔等用于刀路和工艺计算 | 官方招聘页搜索索引文本；直接打开无可读正文；索引列发布日期 2026-09-02 |
| Cadence [Lead Software Engineer (Graphics), R56789](https://cadence.wd1.myworkdayjobs.com/en-US/External_Careers/job/Lead-Software-Engineer--Graphics-_R56789-1) | 上海；10年以上 | 工程软件模型显示、选择与交互、渲染及可视化；C++、内存/线程/图形性能诊断 | 官方招聘页索引文本；资深职责只作深入方向参照，不作为当前学习门槛 |
| NVIDIA [Graphics Tools Software Engineer, JR2017973](https://nvidia.wd5.myworkdayjobs.com/en-US/NVIDIAExternalCareerSite/job/Graphics-Tools-Software-Engineer_JR2017973) | 上海；相关学位及3年以上经验为优先 | C++、图形 API、Linux 进程线程/IPC/内存/系统调用、调试与性能诊断；连接图形工具与底层系统知识 | 官方招聘页索引文本；直接打开无可读正文；GPU 架构与调优属加分项 |
| 数码大方 [三维CAD算法工程师（应届生方向）](https://www.zhipin.com/job_detail/eb2819810b4bfd5f03F_2NW4FFBT.html) · BOSS直聘 | 北京海淀；在校/应届，硕士 | 布尔运算、曲面构造、拓扑维护、特征识别与编辑，提示几何算法方向需要进一步的数学与几何知识 | 仅取得 [BOSS列表摘要](https://www.zhipin.com/zhaopin/fca1b10be8156cb10HB52tg~/)；详情页受安全验证限制，不补写缺失任职条件 |

上述页面或索引的存在不表示岗位现时仍开放；不同资历样本仅用于区分知识应用的深度。前程无忧、猎聘也已检索，但未取得满足本轮地区范围且足以支持能力分析的具体岗位正文，因此未纳入主表；未绕过登录或验证码。

结合样本的辅助判断：C++、算法、工程实现可直接联系 CAM/CAD；几何岗位更关注表示、拓扑与鲁棒性，图形工具岗位更强调操作系统、内存、并发与诊断。CUDA/HPC、量化相关系统及仿真方向的深入安排主要基于知识关系与用户兴趣，本轮岗位样本不足以判断这些方向在目标地区的具体需求。

## 资料与成果管理

课程资料和成果统一放在本仓库的 `courses/<course>/`，总进度见 [STATUS](STATUS.md)；CS50x 目录待实际启动时创建。独立项目或需隔离的受限作业才另设仓库。

课程资料可阅读不等于可公开复制或公布答案。使用实验时按当前课程规则处理框架、测试和解答；公开仓库只保存允许公开的内容，不复制公司代码或客户数据。综合实践采用独立实现和合成数据。
