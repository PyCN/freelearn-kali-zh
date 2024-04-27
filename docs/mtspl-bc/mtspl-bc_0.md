# 前言

渗透测试是当今商业中无处不在的必需品。随着过去几年网络犯罪和基于计算机的犯罪的增加，渗透测试已成为网络安全的核心方面之一，并有助于使企业免受内部和外部威胁的侵害。使渗透测试成为必需的原因是它有助于发现网络、系统或应用程序中的潜在缺陷。此外，它有助于从攻击者的角度识别弱点和威胁。利用系统中的各种潜在缺陷来发现它们对组织可能造成的影响以及对资产的风险因素。然而，渗透测试的成功率主要取决于对测试目标的了解。因此，我们使用两种不同的方法来进行渗透测试：黑盒测试和白盒测试。黑盒测试是指在测试目标没有先验知识的情况下进行测试。因此，渗透测试人员通过系统地收集有关目标的信息来开始测试。而在白盒渗透测试的情况下，渗透测试人员对测试目标有足够的了解，并通过识别目标的已知和未知弱点来开始测试。渗透测试分为七个不同的阶段，如下所示：

1.  **前期交互**：这一步定义了所有前期交互活动和范围定义，基本上是在测试开始之前与客户讨论的一切。

1.  **情报收集**：这个阶段完全是关于收集有关测试目标的信息，通过直接连接到目标或被动地，完全不连接到目标。

1.  **威胁建模**：这个阶段涉及将发现的信息与资产进行匹配，以找到威胁水平最高的领域。

1.  **漏洞分析**：这涉及查找和识别已知和未知的漏洞并对其进行验证。

1.  **利用**：这个阶段致力于利用前一阶段发现的漏洞。通常意味着我们试图访问目标。

1.  **后期利用**：在目标上执行的实际任务，包括下载文件、关闭系统、在目标上创建新用户账户等，都是这个阶段的一部分。这个阶段描述了在利用后需要做什么。

1.  **报告**：这个阶段包括总结测试结果并提出可能的建议和推荐，以修复目标中当前的弱点。

刚刚提到的七个阶段在只有一个测试目标时可能看起来更容易。然而，当需要测试包含数百个系统的庞大网络时，情况完全改变。因此，在这种情况下，手动工作被自动化方法取代。考虑这样一个情景，测试的系统数量恰好是 100 个，所有系统都运行相同的操作系统和服务。手动测试每个系统将消耗大量时间和精力。这种情况需要使用渗透测试框架。渗透测试框架的使用不仅可以节省时间，还可以在改变攻击向量和覆盖更广泛的测试目标方面提供更大的灵活性。渗透测试框架将消除额外的时间消耗，并有助于自动化大部分攻击向量；扫描过程；识别漏洞，最重要的是利用漏洞；从而节省时间并加快渗透测试的步伐。这就是 Metasploit 发挥作用的地方。

Metasploit 被认为是最好的和最广泛使用的渗透测试框架之一。在 IT 安全社区中享有很高的声誉，Metasploit 不仅满足了作为优秀渗透测试框架的需求，还提供了创新功能，使渗透测试人员的工作变得更加轻松。

Metasploit Bootcamp 旨在为读者提供对最流行的渗透测试框架 Metasploit 的深入了解。本书专注于使用 Metasploit 进行渗透测试，同时揭示 Metasploit 相对于传统渗透测试的许多出色功能。本书以集训营的方式深入讲解扫描技术、对各种现实软件的利用、后渗透测试、SCADA、VOIP、MSSQL、MySQL、Android 利用、AV 逃避技术等内容。在完成具有挑战性的自主练习时，您也会发现自己不断思考。

# 本书涵盖的内容

第一章《使用 Metasploit 入门》带领我们了解使用 Metasploit 进行渗透测试的绝对基础知识。它有助于制定计划并设置测试环境。此外，它系统地介绍了渗透测试的各个阶段，同时涵盖了一些尖端的后渗透模块。它进一步讨论了使用 Metasploit 相对于传统和手动测试的优势。

第二章《识别和扫描目标》涵盖了使用 Metasploit 进行情报收集和扫描。该章节重点介绍了对各种不同服务进行扫描，如 FTP、MSSQL、SNMP、HTTP、SSL、NetBIOS 等。该章节还拆解了扫描模块的格式、内部工作原理，并阐明了用于构建模块的库。

第三章《利用和获取访问权限》将我们的讨论转移到利用现实软件。该章混合了关键和中低熵漏洞的组合，并将它们作为一个挑战呈现。该章还讨论了提升和更好的访问质量，同时讨论了 Android 和浏览器利用等具有挑战性的主题。最后，该章讨论了将非 Metasploit 利用转换为与 Metasploit 兼容的利用模块的技术。

第四章《使用 Metasploit 进行后渗透》讨论了 Metasploit 的基本和高级后渗透功能。该章节讨论了 meterpreter 负载上可用的基本后渗透功能，以及高级和强大的后渗透功能，同时介绍了 Windows 和 Linux 操作系统的权限提升。

第五章《使用 Metasploit 测试服务》将讨论使用各种服务进行渗透测试。本章涵盖了 Metasploit 中一些重要的模块，帮助测试 SCADA、MySQL 数据库和 VOIP 服务。

第六章《使用 Metasploit 进行快速利用》将讨论重点转移到构建策略和脚本，以加快渗透测试过程。这一章不仅帮助了解如何改进渗透测试过程的重要知识，还揭示了许多 Metasploit 的功能，可以节省编写利用脚本的时间。最后，该章还讨论了自动化后渗透过程。

第七章，*使用 Metasploit 利用真实世界的挑战*，将行动转移到模拟真实世界问题的环境中。本章重点介绍了渗透测试人员日常生活中使用的技术，这也意味着利用并非易事；您将不得不努力获取利用这些场景的手段。本章将学习诸如暴力破解、识别应用程序、转向内部网络、破解哈希、在明文中找到密码、规避杀毒软件检测、形成复杂的 SQL 查询以及从数据库中枚举数据等技术。

# 你需要为这本书做什么

要跟随并重现本书中的示例，您将需要六到七个系统。一个可以是您的渗透测试系统-安装了 Kali Linux 的计算机-而其他可以是测试系统。或者，您可以在单个系统上工作，并设置一个具有仅主机或桥接网络的虚拟环境。

除了系统或虚拟化，您还需要 Kali Linux 的最新 ISO，该系统默认已经打包了 Metasploit，并包含了本书中示例所需的所有其他工具。

您还需要在虚拟机或实际系统上安装 Ubuntu 14.04 LTS、Windows XP、Windows 7 Home Basic、Windows Server 2008 R2、Windows Server 2012 R1、Metasploitable 2、Metasploitable 3 和 Windows 10，因为所有这些操作系统都将作为 Metasploit 的测试平台。

此外，章节中还提供了所有其他所需工具和易受攻击软件的链接。

# 这本书是为谁准备的

如果您是渗透测试人员、道德黑客或安全顾问，希望快速掌握 Metasploit 框架，并在高度安全的环境中进行高级渗透测试，那么这本书适合您。

# 约定

在这本书中，您将找到许多文本样式，用于区分不同类型的信息。以下是一些样式的示例及其含义的解释。

文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 用户名显示如下：“我们可以看到，从`/tools/exploit/`目录运行`pattern_create.rb`脚本，生成 1000 字节的模式，将生成前面的输出。”

代码块设置如下：

```
def exploit
    connect
    weapon = "HEAD "
    weapon << make_nops(target['Offset'])
    weapon << generate_seh_record(target.ret)
    weapon << make_nops(19)
    weapon << payload.encoded
    weapon << " HTTP/1.0\r\n\r\n"
    sock.put(weapon)
    handler
    disconnect
  end
end

```

当我们希望引起您对代码块的特定部分的注意时，相关的行或项目将以粗体显示：

```
    weapon << make_nops(target['Offset'])
    weapon << generate_seh_record(target.ret)
    weapon << make_nops(19)
    weapon << payload.encoded

```

任何命令行输入或输出都以以下方式编写：

```
irb(main):003:1> res = a ^ b
irb(main):004:1> return res

```

**新术语**和**重要单词**以粗体显示。您在屏幕上看到的单词，例如菜单或对话框中的单词，会在文本中以这种方式出现：“我们可以看到我们已经扫描了整个网络，并发现了两台运行 FTP 服务的主机，分别是 TP-LINK FTP 服务器和 FTP 实用程序 FTP 服务器。”

警告或重要说明会以这样的方式出现。

提示和技巧会以这种方式出现。