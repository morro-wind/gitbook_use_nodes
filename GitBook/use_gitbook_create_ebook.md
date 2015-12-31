# **2.3. 使用 GitBook 制作电子书**

通过前面的学习，我们已经大概了解了 GitBook 电子书籍的结构，并且也了解了 Markdown 标记语法的基本使用。下面我们使用 GitBook 来实际制作一本电子书。

1.创建存放电子书的目录

    $mkdir mybook

2.进入图书目录，并生成 `README.md` 和 `SUMMARY.md` 两个必要文件。

    $cd mybook
    $gitbook init

3.编写图书简介 `README.md` 文件输入如下内容：

    #Introduction
    这是一本使用 gitbook 制作电子书籍的快速上手指南。
    分为两个章节：
    第一章介绍 gitbook.com 在线平台
    第二章介绍 gitbook 基础知识

4.创建章节目录：

    $mkdir part1
    $mkdir part2

5.编写实际内容

进入第一章目录，编写第一章内容：

    #README.md
    GitBook除了是一个命令行工具，它同时也是间书籍发布平台和电子书店。桌面版本同时支持Mac、Windows、Linux三种平台。

    #register.md
    访问gitbook.com，如有GitHub帐号，直接使用GitHub帐号进行授权注册，这里使用GitHub帐号，是因为与GitHub进行关联时无需再次做GitHub授权操作。当然，你也可以注册一个GitBook帐号。

进入第二章目录，并编写其内容：

    #README.md
    使用 `gitbook` 命令的前提，必须已经安装好`Node`、`Npm`,在准备工作中，我们已经将它们安装并配置好了，现在来查看下版本。  

    #markdown.md
    本节仅简要介绍 Markdown 的基本语法与展现......

> <font size=3> 以上都只是截取了章节目录的部分文件和内容.</font>

6.配置SUMMARY.md文件

每完成一个章节内容，即可在图书目录内进行连接，当然也可全部完成后在进行连接。

    #SUMMARY.md
    * [Introduction](README.md)
    * [前言](qian_yan.md)
    * [准备工作和所具备知识](zhun_bei_gong_zuo.md)
    * [1.gitbook](part1/README.md)
       * [1.1.gitbook.com账户注册](part1/register.md)
    * [2.GitBook 基础](part2/README.md)
       * [2.1.Markdown 语法](part2/markdown.md)

SUMMARY.md 结构说明

    * 无序列表
    []章节名称
    ()章节对应的实际文件，包含相对路径

> ***<font size="3" color="#A60000">注：</font>*** 
> *<font size=3>另一种创建图书的方式是：先定义好 `SUMMARY.md` 内的图书结构，然后使用 `gitbook init` 命令生成图书目录和文件。这样的好处是有助于一本书的整体构思，坏处就是写作过程中很难变更图书结构(除非你不会有思维定式)。</font>*

**在线查看**

输入 `gitbook serve` ，在浏览器中输入 `http://localhost:4000` ，就可以看到和 GitBook 网站一样的网页版电子书。修改内容、保存，会看到网页自动重载并更新了内容。

现在已经拥有了一个可在本地离线编辑，并能立即展现最终效果的编写环境。