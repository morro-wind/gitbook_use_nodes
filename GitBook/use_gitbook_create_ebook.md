# **2.3. 使用 GitBook 制作电子书**

通过前面的学习，我们已经大概了解了 GitBook 电子书籍的结构，并且也了解了 Markdown 标记语法的基本使用。下面我们使用 GitBook 来实际制作一本电子书。

建存放电子书的目录

    $mkdir mybook

进入图书目录，并生成 `README.md` 和 `SUMMARY.md` 两个必要文件。

    $cd mybook
    $gitbook init

编写图书简介 `README.md` 文件输入如下内容：

    这是一本使用 gitbook 制作电子书籍的快速上手指南。
    分为两个章节：
    第一章介绍 gitbook.com 在线平台
    第二章介绍 gitbook 基础知识

创建章节目录：

    $mkdir part1
    $mkdir part2

进入第一章目录，编写第一章内容