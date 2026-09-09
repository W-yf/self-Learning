# 学习资源

以用户原稿的课程和实验版本为基础。视频优先，中英文按质量和完整度选择；任务与验收统一见 [LEARNING_PLAN](LEARNING_PLAN.md)。

## 固定入口

| 阶段 | 理论/讲义 | 实验/作业 |
|---|---|---|
| R0 设计准备 | [MIT 6.005 S16](https://ocw.mit.edu/ans7870/6/6.005/s16/) | 自拟 C++ 图的两种表示和契约测试；不用 Java 评分器 |
| R1 CSAPP | [CMU 15-213 S25](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s25/www/)、CSAPP 第 3 版 | [Self-Study Handout 入口](https://csapp.cs.cmu.edu/3e/labs.html)：Data、Bomb、Cache、Malloc |
| R2 操作系统 | [南大 OS 2025](https://jyywiki.cn/OS/2025/)、[MIT 6.1810 F25](https://pdos.csail.mit.edu/6.1810/2025/schedule.html) | [M2](https://jyywiki.cn/OS/2025/labs/M2.md)；[util](https://pdos.csail.mit.edu/6.1810/2025/labs/util.html)、[syscall](https://pdos.csail.mit.edu/6.1810/2025/labs/syscall.html)、[pgtbl](https://pdos.csail.mit.edu/6.1810/2025/labs/pgtbl.html)、[cow](https://pdos.csail.mit.edu/6.1810/2025/labs/cow.html)、[lock](https://pdos.csail.mit.edu/6.1810/2025/labs/lock.html) |
| R3 离散与算法 | [MIT 6.042J F10](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/)；[清华数据结构](https://dsa.cs.tsinghua.edu.cn/~deng/ds/dsacpp/) 补缺 | [MIT 6.006 S20 作业](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/pages/assignments/)：PS0、PS1–7 编程与代表性证明 |
| R4 网络 | [Kurose 公开讲解](https://gaia.cs.umass.edu/kurose_ross/online_lectures.htm)＋自顶向下教材 | [Wireshark 实验](https://gaia.cs.umass.edu/kurose_ross/wireshark.php)、[Proxy 说明](https://csapp.cs.cmu.edu/3e/proxylab.pdf) |
| R5 数据库 | [CMU 15-445 F24](https://15445.courses.cs.cmu.edu/fall2024/) | [固定 release](https://github.com/cmu-db/bustub/releases/tag/v20241207-2024fall)；[P0](https://15445.courses.cs.cmu.edu/fall2024/project0/)、[P1](https://15445.courses.cs.cmu.edu/fall2024/project1/)、[P2](https://15445.courses.cs.cmu.edu/fall2024/project2/)、[P3](https://15445.courses.cs.cmu.edu/fall2024/project3/) |
| M 基础数学 | [MIT 18.06SC F11](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/)；Strang 英文第 5 版辅书选择保留，购买未确认 | 线代手算与解释；微积分/概率统计的完整资料与工时待模块诊断后确定 |

R0 直达：[Testing](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/03-testing/)、[Specifications](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/06-specifications/)、[ADT](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/12-abstract-data-types/)、[表示不变量](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/13-abstraction-functions-rep-invariants/)。

## 版本与环境

2026-09-09 本轮重新查阅了 CSAPP 自学入口及 Data/Cache/Malloc README、南大 M2、xv6 2025 课表/pgtbl/cow/lock/工具页、6.006 作业入口和 15-445 F24 课程首页。其余入口沿用先前记录，不能据此声称全部网页重新核验。未下载实验包、安装环境或运行课程测试。

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

未来候选只保留入口：[CS149](https://github.com/stanford-cs149/asst2)、[MIT 6.5840](https://pdos.csail.mit.edu/6.5840/general.html)、[Go Tour](https://go.dev/tour/welcome/1)、[北大编译实践](https://pku-minic.github.io/online-doc/)、[Deep Learning Systems](https://dlsyscourse.org/)。不据此排课、安装或采购。
