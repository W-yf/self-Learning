# 学习资源

以用户原稿的课程和实验版本为基础。视频优先，中英文按质量和完整度选择；任务与验收统一见 [LEARNING_PLAN](LEARNING_PLAN.md)。

## 固定入口

| 阶段 | 理论/讲义 | 实验/作业 |
|---|---|---|
| R0 设计准备 | [MIT 6.031 S22](https://web.mit.edu/6.031/www/sp22/) 主讲义；旧 MITx 视频按主题辅助 | 自拟 C++ 图的两种表示和契约测试；Python 项目候选见下文；不安排 Java 作业或评分器 |
| R1 CSAPP | CSAPP 第 3 版＋[CMU 15-213 S25](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/)；[Dr.Dng 中文带学](https://www.bilibili.com/video/BV1hf4y1P7qW/) 按下表选用 | [Self-Study Handout 入口](https://csapp.cs.cmu.edu/3e/labs.html)：Data、Bomb、Cache、Malloc |
| R2 操作系统 | [南大 OS 2025](https://jyywiki.cn/OS/2025/)、[MIT 6.1810 F25](https://pdos.csail.mit.edu/6.1810/2025/schedule.html) | [M2](https://jyywiki.cn/OS/2025/labs/M2.md)；[util](https://pdos.csail.mit.edu/6.1810/2025/labs/util.html)、[syscall](https://pdos.csail.mit.edu/6.1810/2025/labs/syscall.html)、[pgtbl](https://pdos.csail.mit.edu/6.1810/2025/labs/pgtbl.html)、[cow](https://pdos.csail.mit.edu/6.1810/2025/labs/cow.html)、[lock](https://pdos.csail.mit.edu/6.1810/2025/labs/lock.html) |
| R3 离散与算法 | [MIT 6.042J F10](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/)；[清华数据结构](https://dsa.cs.tsinghua.edu.cn/~deng/ds/dsacpp/) 补缺 | [MIT 6.006 S20 作业](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/pages/assignments/)：PS0、PS1–7 编程与代表性证明 |
| R4 网络 | [Kurose 公开讲解](https://gaia.cs.umass.edu/kurose_ross/online_lectures.htm)＋自顶向下教材 | [Wireshark 实验](https://gaia.cs.umass.edu/kurose_ross/wireshark.php)、[Proxy 说明](https://csapp.cs.cmu.edu/3e/proxylab.pdf) |
| R5 数据库 | [CMU 15-445 F24](https://15445.courses.cs.cmu.edu/fall2024/) | [固定 release](https://github.com/cmu-db/bustub/releases/tag/v20241207-2024fall)；[P0](https://15445.courses.cs.cmu.edu/fall2024/project0/)、[P1](https://15445.courses.cs.cmu.edu/fall2024/project1/)、[P2](https://15445.courses.cs.cmu.edu/fall2024/project2/)、[P3](https://15445.courses.cs.cmu.edu/fall2024/project3/) |
| M 基础数学 | [MIT 18.06SC F11](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/)；Strang 英文第 5 版辅书选择保留，购买未确认 | 线代手算与解释；微积分/概率统计的完整资料与工时待模块诊断后确定 |

R0 直达：[Testing](https://web.mit.edu/6.031/www/sp22/classes/03-testing/)、[Specifications](https://web.mit.edu/6.031/www/sp22/classes/06-specifications/)、[ADT](https://web.mit.edu/6.031/www/sp22/classes/10-abstract-data-types/)、[表示不变量](https://web.mit.edu/6.031/www/sp22/classes/11-abstraction-functions-rep-invariants/)。[2016 版](https://ocw.mit.edu/ans7870/6/6.005/s16/) 保留为旧笔记来源与版本对照。

## R0 视频配合

用户提供的 [MIT 6.005 软件构建视频选集](https://www.bilibili.com/video/BV1Tp4y197XX/)可作为 R0 的视频讲解入口。2026-09-11 核对页面简介及完整目录：共 74P，标题标注“中英字幕·机翻”，简介注明来源为 edX；章节顺序与 [MITx 6.005.1x 官方大纲](https://openlearninglibrary.mit.edu/assets/courseware/v1/3fa26a139145897cd0db436e0d2e2ce1/asset-v1%3AMITx%2B6.005.1x%2B3T2016%2Btype%40asset%2Bblock/6.005.1xSyllabus.pdf)一致。这支持按主题配用，但未逐集试听，不据此认定为 S16 校内整学期课堂录像或保证字幕准确。

| R0 主题 | 对应选集 | 配合方式 |
|---|---|---|
| Testing | P19–25 | 当前 Test-first Programming 从 P21 开始；该集也包含 Partitioning |
| Specifications | P26–31 | P26–29 讲规格；P30–31 的异常内容按讲义需要选看 |
| Abstract Data Types | P52–56 | 关注抽象、操作分类与表示独立；必要时用自拟 C++、Python 例子解释 |
| Abstraction Functions & Rep Invariants | P57–63 | 对照抽象函数、表示不变量与表示泄漏，迁移到自拟 C++ 图 |

先看对应视频，再针对性阅读 S22 官方讲义并做一道自拟应用题；不默认完整观看 74 集，也不再叠加 6.0001 的 Testing 视频。视频与新版讲义按主题匹配，跳过 Java 专属语言与工具教学；机器翻译中的 specification、representation invariant 等术语以官方原文为准。2022 课程使用 TypeScript，只按阅读需要解释语法；练习继续使用 C/C++、Python，不能直接套用其他语言的对象与生命周期规则。当前阅读位置由课程 README 维护。

更新版本参考：[MIT 6.102 Spring 2026](https://web.mit.edu/6.102/www/sp26/)，使用 TypeScript，仍保留上述四个主题。当前只作为更新内容的对照入口，主阅读固定 2022 版，R0 范围和自拟实验不变；将来若系统学习现代软件构建，再评估整门新版课程。

2022 原版作业的题目说明可公开阅读：[PS0](https://web.mit.edu/6.031/www/sp22/psets/ps0/)、[PS1](https://web.mit.edu/6.031/www/sp22/psets/ps1/)、[PS2](https://web.mit.edu/6.031/www/sp22/psets/ps2/)、[PS3](https://web.mit.edu/6.031/www/sp22/psets/ps3/)、[PS4](https://web.mit.edu/6.031/www/sp22/psets/ps4/)、[Star Battle](https://web.mit.edu/6.031/www/sp22/projects/starb/)。官方起始仓库经 Didit 和 MIT GitHub 分发；目前未核实可匿名取得完整起始代码及评分测试的途径，不能把说明页公开等同于整套作业可直接运行。本轮未获取作业包，也未启用原版作业。

## 软件构建的个人参考资料

[pengzhangzhi 的 Software Construction 目录](https://github.com/pengzhangzhi/self-taught-CS/tree/main/Software%20Construction)：2026-09-11 核对资源页、笔记与实验目录，并抽查 Specifications 笔记。资源页链接 Spring 2021，笔记采用 Java 体系，实验目录包含 ps0–ps4 和播放器相关文件；未运行或审核全部实现。中文提要可用于学后查漏，准确表述、适用条件与版本以官方讲义核对。作业实现不作为当前导读或答案来源；不因文件齐全推断正确或已通过评分。

用户明确不学习 Java，因此不安排该仓库中的 Java 原版实验。参考目录组织方式和软件构建的训练目标，实际笔记仍保持精简，练习由用户用 C/C++、Python 独立完成，不逐行移植他人的解答。

## R0 公开项目导读

[dbader/schedule](https://github.com/dbader/schedule) 是 Python 定时任务库，本次导读固定标签 **1.2.2**。作为相关理论与小练习之后的项目导读材料，沿创建、登记、执行的过程阅读；课程 README 登记 teach 材料入口，当前尚未启动阅读或作业。它是公开项目练习材料，不是 MIT 原版作业，既有 R0 验收尚未调整。

原始资料：[固定版本源码](https://github.com/dbader/schedule/blob/1.2.2/schedule/__init__.py)、[原项目测试](https://github.com/dbader/schedule/blob/1.2.2/test_schedule.py)、[MIT 许可证](https://github.com/dbader/schedule/blob/1.2.2/LICENSE.txt)。2026-09-11 已读取源码与许可；尚未克隆、安装或运行测试。若复制或分发原项目代码，保留相应版权和许可声明。

## CSAPP 中文带学的使用

用户提供的 [Dr.Dng陪跑CSAPP: bigONE《深入理解计算机系统》](https://www.bilibili.com/video/BV1hf4y1P7qW/)，页面作者为“清华邓博士”。2026-09-10 通过浏览器读取简介和完整选集：当前 23P，按分集时长合计 33:43:53。简介说明融合多门课程材料；目录包含 C、数据表示、机器级程序、链接、动态分配及 RISC-V。这里只核查了简介和目录，未逐集试听，不能据此保证全部讲解的准确性或覆盖深度。

可作为已覆盖主题的中文讲解入口，按下表配合当前路线使用。P 号为本次页面顺序，开课时同时核对标题；不将该视频认作 CMU S25 同版课程。

| 当前主题 | 本视频对应选集 | 使用方式 |
|---|---|---|
| 总览与 C 补缺 | P1；P8、P11–13 | 总览、语法、指针、结构体布局与内存错误，按诊断选用 |
| 数据表示 → Data | P9–10；P16–18 | 对照第 2 章；两组有重叠，按理解需要选择，独立做题与实验 |
| 机器级程序 → Bomb | P19–22 | 对照第 3 章，结合 GDB 与 x86-64 调用/数据访问分析 |
| 链接 | P3–7 | 对照第 7 章；专题与读书讲解按需要选择，不因没有单独大 lab 而跳过理论 |
| 动态分配 → Malloc | P14–15 | 对照第 9.9 节，先补第 9 章虚拟内存基础，再进入实验 |
| RISC-V 衔接 | P2、P23 | OS 前按需选读；与 Bomb 的 x86-64、教材第 4 章的 Y86-64 分清语境 |

当前目录未单列缓存/存储层次、完整虚拟内存、异常控制流、系统级 I/O、网络与并发等后续主题；这是目录层面的覆盖判断，不排除片内提及。相应理论按 CSAPP 和 CMU 官方资料补齐，网络仍在 R4 展开。视频中的拓展材料不自动新增整门课程或实验。

观看时间包含在主课理论投入中，不能等同于学会所需时间；暂停、推导、习题与实验另按实际记录。选择中文讲解后，同主题不默认再完整观看一套英文课。原有 108 小时是待校准基线，不为塞入全套视频压缩理论练习或 lab。

## 本轮规划参考与按需补缺

- [CS 自学指南：CS 学习规划](https://csdiy.wiki/CS学习规划/)：用于核对覆盖面和发现资料；其课程分类不规定全部先后次序。采用工具补缺、系统基础与内核实践的思路，具体版本、前置和实验要求以对应官方课程为准。
- [CMU 15-213 S25 课表](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/schedule.html)：有教材章节、讲义及 Linux/GDB/GCC/C 的 Bootcamp 入口，用于补当前实验所需内容；视频权限需开课核实。
- [MIT 6.1810 F25 课表](https://pdos.csail.mit.edu/6.1810/2025/schedule.html)：从该页进入匹配 xv6 教材与 C in xv6、OS organization、page faults、locking、coordination、文件系统/恢复资料；具体衔接见 LEARNING_PLAN。
- [MIT Missing Semester 2020](https://missing.csail.mit.edu/2020/)：仅按需选 Shell、命令行环境、调试与构建相关内容，与 CMU 工具材料择一补缺；不增加完整课程或专项工具训练。

保留已选 6.042J/6.006 和南大＋xv6 的组合。门户列出的其他语言入门、算法或内核课程只是备选资料，不据此更换语言、叠加另一套实验或滚动升级课程年份。

## 版本与环境

2026-09-09 本轮重新查阅了 CSAPP 自学入口及 Data/Cache/Malloc README、南大 M2、xv6 2025 课表/pgtbl/cow/lock/工具页、6.006 作业入口和 15-445 F24 课程首页。其余入口沿用先前记录，不能据此声称全部网页重新核验。未下载实验包、安装环境或运行课程测试。

2026-09-10 新查阅 CS 自学指南总规划、CMU S25 课表、MIT F25 课表/课程说明/lock 正文、Missing Semester 2020 目录，核对虚拟内存与 Malloc、系统 I/O 与 OS、页故障/同步与 xv6 实验的衔接。lock 正文第二部分现为读写锁，页首仍有 block cache 旧描述，计划按正文修正。其余固定实验入口沿用既有核查；网页可读不等于视频可看、实验已下载或环境验证通过。

| 课程 | 开始时需要验证 |
|---|---|
| CSAPP | Linux x86-64、自学包具体版本、编译与 GDB；Data 的 btest/dlc，Cache 的测试驱动/Valgrind lackey，Malloc 的 mdriver/trace。只取 Self-Study Handout，不照搬面向教师的发布包构建步骤 |
| xv6 | [2025 tools](https://pdos.csail.mit.edu/6.1810/2025/tools.html) 对应 RISC-V 工具链与 QEMU；Windows 可按说明用 WSL2。每个 lab 使用匹配分支的说明与 make grade，不能混用旧 pgaccess 教程 |
| 南大 M2 | 按 [南大实验说明](https://jyywiki.cn/OS/2025/labs/Labs.md) 与自身框架确认 Linux 环境；不把 xv6 环境验证当作自动兼容，不依赖校内 OJ |
| 6.006 | 保留对应 Python 模板与作业测试；以自测、穷举对照、独立证明验收 |
| 网络 | Wireshark 9.0 说明与 9e trace 匹配；Proxy 自学包、Tiny、curl 与 driver.sh 先跑通基线 |
| BusTub | 固定 v20241207-2024fall / 5705473；[固定 README](https://raw.githubusercontent.com/cmu-db/bustub/v20241207-2024fall/README.md) 先前记录推荐 Ubuntu 22.04、不支持 WSL，开课复核。不能直接沿用 xv6 的 WSL 建议 |

CSAPP 细则：[Data README](https://csapp.cs.cmu.edu/3e/README-datalab)、[Cache 说明](https://csapp.cs.cmu.edu/3e/cachelab.pdf)、[Cache README](https://csapp.cs.cmu.edu/3e/README-cachelab)、[Malloc 说明](https://csapp.cs.cmu.edu/3e/malloclab.pdf)、[Malloc README](https://csapp.cs.cmu.edu/3e/README-malloclab)。实际测试命令以获取的学生包为准；不因预期某条命令存在就记作验证通过。

## 资料使用与未来入口

沿用已记录的 [MIT 6.005 分享规则](https://ocw.mit.edu/ans7870/6/6.005/s16/general/collaboration.html) 和 BusTub 固定 README 的公开限制；启用时复核。课程框架、测试、trace、参考二进制和受限实现放在独立非公开学习空间，公开仓库保留合规状态、通用笔记与自拟练习。其他材料使用前核对许可。

上述使用边界同样适用于独立课程仓库与 handoff 文档。课程仓库管理完整的允许保存的学习成果，公开展示内容按资料许可选择；主仓库只汇总可公开的进度和证据引用，不复制受限实现。

未来候选只保留入口：[CS149](https://github.com/stanford-cs149/asst2)、[MIT 6.5840](https://pdos.csail.mit.edu/6.5840/general.html)、[Go Tour](https://go.dev/tour/welcome/1)、[北大编译实践](https://pku-minic.github.io/online-doc/)、[Deep Learning Systems](https://dlsyscourse.org/)。不据此排课、安装或采购。
