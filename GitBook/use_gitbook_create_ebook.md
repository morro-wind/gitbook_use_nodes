# **2.3. 使用 GitBook 制作电子书**

通过前面的学习，我们已经大概了解了 GitBook 电子书籍的结构，并且也了解了 Markdown 标记语法的基本使用。下面我们使用 GitBook 来实际制作一本电子书。

建存放电子书的目录

    $mkdir mybook

进入图书目录，并生成 `README.md` 和 `SUMMARY.md` 两个必要文件。

    $cd mybook
    $gitbook init

编写图书简介 `README.md` 文件输入如下内容：

    #Introduction
    这是一本使用 gitbook 制作电子书籍的快速上手指南。
    分为两个章节：
    第一章介绍 gitbook.com 在线平台
    第二章介绍 gitbook 基础知识

创建章节目录：

    $mkdir part1
    $mkdir part2

进入第一章目录，编写第一章内容：

    #README.md
    GitBook除了是一个命令行工具，它同时也是间书籍发布平台和电子书店。桌面版本同时支持Mac、Windows、Linux三种平台。

    #register.md
    访问gitbook.com，如有GitHub帐号，直接使用GitHub帐号进行授权注册，这里使用GitHub帐号，是因为与GitHub进行关联时无需再次做GitHub授权操作。当然，你也可以注册一个GitBook帐号。

进入第二章目录，并编写其内容：

    #README.md
    
    