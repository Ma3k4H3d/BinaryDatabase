## 论文目录

---
### 2019年

#### 综述

* ##### **Fuzzing-Art-Science-and-Engineering**

> **Abstract**
> ​		在当今可用的众多软件漏洞发现技术中，模糊测试由于其概念简单，部署的低屏障以及发现现实世界软件漏洞的大量经验证据而一直非常受欢迎。虽然近年来研究人员和从业人员都为改进模糊测试投入了大量不同的努力，但这项工作的激增也使得难以获得全面和一致的模糊测试观点。为了帮助保存并使大量的模糊测量文献保持连贯性，本文提出了一种统一的，通用的模糊测试模型以及当前模糊文献的分类。我们通过调查相关文献和艺术，科学和工程方面的创新，有条不紊地探索模型模糊器的每个阶段的设计决策，使现代模糊器有效。

#### 研究性工作

* ##### **SoK-Security-Evaluation-of-Home-Based-IoT-Deployments-S&P**

> **Abstract**
> ​		智能家居在安全方面一直表现得不尽人意，究其原因，在于IoT系统相对于传统的嵌入式系统，还引入了智能终端和网络，这就导致了其本身暴露了更多的攻击面。本文通过总结大量论文来帮助研究人员和从业者更好的理解针对智能家居的攻击技术，缓解措施，以及利益相关者应该如何解决这些问题。最后作者利用这些方法评估了45款智能家居设备，并将实验数据公布在https://yourthings.info%E3%80%82

---
### 2018年

#### 综述

#### 研究性工作

* ##### **Check-It-Again-Detecting-Lacking-Recheck-Bugs-in-OS-Kernels-CCS**

> **Abstract**
> ​		论文中，作者主要介绍分析操作系统内核中的LRC（lacking-recheck）类型bug。并介绍了自己设计的一个静态分析系统LRSan（在Linux上实现），用于检测操作系统内核中的LRC bug。***本文的主要贡献： 1. 定义了LRC bugs，并第一次展示了关于LRC bug的深入研究。 2. 实现一个自动化的LRC bug检测系统（LRSan），基于LLVM，使用在Linux内核上，可以检测内核中的LRC bug。LRSan运用了很多新的程序静态分析技术。结果显示LRSan在Linux内核发现了2808个LRC case，检测耗时为4小时。并且作者会将它开源。 3. 识别Security check（SC）和相关Critical variable（CV）的方法。 4. 发现了Linux内核中的19个新的LRC bug。***

* ##### **Automated-Detection-Exploitation-and-Elimination-of-Double-Fetch-Bugs-Using-Modern-CPU-Features**

> **Abstract**
> ​		Double-fetch bugs 是一种特殊的条件竞争，在高权限线程的time-of-check和time-of-use之间，低权限线程能够修改共享的内存，导致高权限线程访问的内存产生不一致。本文作者提出了一种检测，利用并消除double-fetch bugs的技术DECAF和Dropit。总体来说，***贡献如下：1. 把cache attack与kernel fuzzing结合起来。2. 首个自动化的挖掘double-fetch bugs的方法。3. 利用的成功率高达97%。4.利用Hardware Transactional Memory的特性，消除double-fetch bugs。5.方法对fuzz TEE也有效。***

* ##### **Towards-Paving-the-Way-for-Large-Scale-Windows-Malware-Analysis-Generic-Binary-Unpacking-With-Orders-of-Magnitude-Performance-Boost-CCS**

> **Abstract**
> ​		windows的软件脱壳本来已经在多年前已经被讨论得非常多了，目前安全学术会议上关于脱壳的论文非常少，然而这篇关于脱壳的论文还能在2018年被CCS所录取，足见他的方法之高效。此前关于脱壳的方法大多是跟踪脱壳时期的内存代码写入执行的变化，从而跟踪被加密代码的解密流程从而追溯到OEP。这也是对于分析脱壳的一个最为直观的方法，***在这篇论文里作者提出来通过跟踪IAT(函数导入表)被恢复和引用的情况来追溯OEP，并且达到很理想的效果。作者将这款工具称为BinUnpack。***

* ##### **Using-Logic-Programming-to-Recover-C-Classes-and-Methods-From-Compiled-Executables-CCS**

> **Abstract**
> ​		随着计算机硬件的发展，计算机软件也变得越来越庞大、越来越复杂。而为了开发这些复杂的计算机软件，软件工程师们逐渐把方向转向了面向对象 OO（Object Oriented）的编程语言，例如 C++ 等高级开发语言。这些高级的编程语言，对于开发庞大、复杂的应用程序，它可以提供一种高级抽象的框架（Natural Framework），使得面向对象的编程语言更加适用于构造复杂的数据结构 — Class。类可以把相关的数据成员和一组对数据成员进行操作的方法绑定在一起，这样的绑定方式极大的方便了 C++ 代码的维护与管理，使得开发者更容易、更高效地开发复杂的应用程序。虽然类可以给开发者带来极大的便利，但是，万事万物总有两面性，类也一样，它给开发者带来便利的同时，也给软件逆向分析工程师带来了不便，使得分析师在分析 C++ 开发的程序的难度有所提高，特别是在分析恶意程序的时候，分析 C++ 开发的恶意程序变成了一项更高难度的挑战。因此，如何从恶意程序中恢复出代码的高级抽象特性（例如类等），成为了一项值得深究的工作。

* ##### **Enforcing-Unique-Code-Target-Property-for-Control-Flow-Integrity-CCS**

> **Abstract**
> ​		在这篇文章中，作者主要介绍了一种准确率更高的确保CFI的应用方式：Unique Code Target（UCT）。对于每次间接跳转（ICT），作者们设计了一个叫μUCT的系统来确保这一特性的实施。在编译时，μCFI就识别那些可能影响ICT的指令并让程序去记录一些必要的执行环境；在运行时，μCFI在另一个进程中监视程序的运行，并且在一些关键性的指令上使用内存安全地记录着地运行环境来做一些对点分析，判断这些指令的跳转是否符合预期。作者将μCFI这套系统布置到SPEC benchmark和2个服务器程序（nginx和vsftpd）上测试性能和overhead。同时它们还用它来测试了5个真实世界中的案例、1个[COOP](https://csdl.computer.org/csdl/proceedings/sp/2015/6949/00/6949a745.pdf)的poc进行攻击的案例。μCFI在这些测试上表现得都非常好，展现了100%的检测率和仅不到10%的overhead

* ##### **Angora-Efficient-Fuzzing-by-Principled-Search-S&P**

> **Abstract**
> ​		Fuzzing是一种用于查找软件错误的流行技术。然而，最先进的模糊器的性能还有很多不足之处。基于符号执行的模糊器产生高质量输入但运行缓慢，而基于随机变异的模糊器运行速度快但难以产生高质量输入。我们提出了一种新的基于突变的模糊器Angora，它的性能远远超过了最先进的模糊器。Angora的主要目标是通过解决路径约束来增加分支覆盖率而无需符号执行。**为了有效地解决路径约束，我们引入了几个关键技术：可扩展的字节级污点跟踪，上下文敏感的分支计数，基于梯度下降的搜索和输入长度探索**。在LAVA-M数据集上，Angora发现了几乎所有注入的错误，发现了比我们比较的任何其他模糊器更多的错误，并且发现错误是程序中第二好的模糊器的8倍。Angora还发现了LAVA作者注射但却无法触发的103个错误。我们还在八个流行的，成熟的开源程序上测试了Angora。Angora分别在file，jhead，nm，objdump和size中发现了6,52,29,40和48个新错误。我们测量了Angora的覆盖范围，并评估了其关键技术如何促成其令人印象深刻的性能。

* ##### **NAR-Miner-Discovering-Negative-Association-Rules-from-Code-ESEC/FSE**

> **Abstract**
> ​		从基于数据挖掘技术的源代码推断编程规则已被证明对检测软件错误是有效的。现有研究侧重于以A⇒B的形式发现积极规则，表明当操作A出现时，操作B也应该在这里。不幸的是，负面规则（A⇒¬B），表明程序元素之间的相互抑制或冲突关系，没有得到应有的重视。事实上，违反这些负面规则也会导致严重的错误。在本文中，我们提出了一种名为NAR-Miner的新方法，可以从大规模系统中自动提取负关联编程规则，并检测它们的违规行为来发现bug。然而，挖掘负面规则面临着比挖掘正面规则更严重的规则爆炸问题。大多数获得的负面规则都是无趣的，并且可能导致不可接受的错误警报。**为了解决这个问题，我们设计了一个语义约束的挖掘算法，将规则挖掘集中在具有强语义关系的元素上。此外，我们引入信息熵来排列候选负面规则并突出有趣的规则**。因此，我们有效地缓解了规则爆炸问题。我们实现NAR-Miner并将其应用于Linux内核（v4.12-rc6）。实验表明，不感兴趣的规则大大减少，检测到的17个违规行为已被确认为真正的错误并被内核社区修补。我们还将NAR-Miner应用于PostgreSQL，OpenSSL和FFmpeg，并发现了六个真正的错误。

---
### 2017年

#### 综述

#### 研究性工作
* ##### **VUzzer-Application-aware-Evolutionary-Fuzzing-NDSS**

> **Abstract**
> ​		Fuzzing是一种有效的软件测试技术，用于查找错误。考虑到实际应用程序的大小和复杂性，现代模糊器往往是可扩展的，但在探索执行更深层次的错误或者能够在应用程序中深入渗透但不具有可扩展性方面无效。在本文中，我们提出了一种应用程序感知的进化模糊测试策略，它不需要任何有关应用程序或输入格式的先验知识。**为了最大化覆盖范围并探索更深入的路径，我们利用基于静态和动态分析的控制和数据流特征来推断应用程序的基本属性。**与应用程序无关的方法相比，这可以更快地生成有趣的输入。我们在VUzzer中实现我们的模糊测试策略并在三个不同的数据集上进行评估：DARPA Grand Challenge二进制文件（CGC），一组实际应用程序（二进制输入解析器）和最近发布的LAVA数据集。在所有这些数据集中，通过快速查找几个现有和新的错误，VUzzer产生的结果明显优于最先进的模糊器。

* ##### **Digtool-A-Virtualization-Based-Framework-for-Detecting-Kernel-Vulnerabilities-USENIX**

>  **Abstract**
> ​		发现操作系统（OS）内核中的漏洞并对其进行修补对于操作系统安全至关重要。但是，缺乏有效的内核漏洞检测工具，尤其是对于Microsoft Windows等封闭源操作系统。在本文中，我们介绍了Digtool，一个有效的，仅二进制代码的内核漏洞检测框架。 Digtool构建于我们设计的虚拟化监视器之上，成功捕获内核执行的各种动态行为，例如内核对象分配，内核内存访问，线程调度和函数调用。通过这些行为，Digtool已经确定了45个零日漏洞，例如最近版本的Microsoft Windows的内核代码和设备驱动程序中的out--bounds访问，free-after-free和check-time-of-use-of-use ，包括Windows 7和Windows 10。

---
### 2016年
#### 综述

#### 研究性工作

---
### 2015年
#### 综述

#### 研究性工作

---
