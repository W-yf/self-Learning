# 学习资源

以用户原稿的课程和实验版本为基础。视频优先，中英文按质量和完整度选择；任务与验收统一见 [LEARNING_PLAN](LEARNING_PLAN.md)。

## 固定入口

| 阶段 | 理论/讲义 | 实验/作业 |
|---|---|---|
| R0 设计准备 | [MIT 6.005 S16](https://ocw.mit.edu/ans7870/6/6.005/s16/) | 自拟 C++ 图的两种表示和契约测试；不用 Java 评分器 |
| R1 CSAPP | CSAPP 第 3 版＋[CMU 15-213 S25](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/)；[Dr.Dng 中文带学](https://www.bilibili.com/video/BV1hf4y1P7qW/) 按下表选用 | [Self-Study Handout 入口](https://csapp.cs.cmu.edu/3e/labs.html)：Data、Bomb、Cache、Malloc |
| R2 操作系统 | [南大 OS 2025](https://jyywiki.cn/OS/2025/)、[MIT 6.1810 F25](https://pdos.csail.mit.edu/6.1810/2025/schedule.html) | [M2](https://jyywiki.cn/OS/2025/labs/M2.md)；[util](https://pdos.csail.mit.edu/6.1810/2025/labs/util.html)、[syscall](https://pdos.csail.mit.edu/6.1810/2025/labs/syscall.html)、[pgtbl](https://pdos.csail.mit.edu/6.1810/2025/labs/pgtbl.html)、[cow](https://pdos.csail.mit.edu/6.1810/2025/labs/cow.html)、[lock](https://pdos.csail.mit.edu/6.1810/2025/labs/lock.html) |
| R3 离散与算法 | [MIT 6.042J F10](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/)；[清华数据结构](https://dsa.cs.tsinghua.edu.cn/~deng/ds/dsacpp/) 补缺 | [MIT 6.006 S20 作业](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/pages/assignments/)：PS0、PS1–7 编程与代表性证明 |
| R4 网络 | [Kurose 公开讲解](https://gaia.cs.umass.edu/kurose_ross/online_lectures.htm)＋自顶向下教材 | [Wireshark 实验](https://gaia.cs.umass.edu/kurose_ross/wireshark.php)、[Proxy 说明](https://csapp.cs.cmu.edu/3e/proxylab.pdf) |
| R5 数据库 | [CMU 15-445 F24](https://15445.courses.cs.cmu.edu/fall2024/) | [固定 release](https://github.com/cmu-db/bustub/releases/tag/v20241207-2024fall)；[P0](https://15445.courses.cs.cmu.edu/fall2024/project0/)、[P1](https://15445.courses.cs.cmu.edu/fall2024/project1/)、[P2](https://15445.courses.cs.cmu.edu/fall2024/project2/)、[P3](https://15445.courses.cs.cmu.edu/fall2024/project3/) |
| M 基础数学 | [MIT 18.06SC F11](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/)；Strang 英文第 5 版辅书选择保留，购买未确认 | 线代手算与解释；微积分/概率统计的完整资料与工时待模块诊断后确定 |

R0 直达：[Testing](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/03-testing/)、[Specifications](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/06-specifications/)、[ADT](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/12-abstract-data-types/)、[表示不变量](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/13-abstraction-functions-rep-invariants/)。

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
