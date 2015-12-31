# **2.1. GitBook 图书结构介绍**

一本由 GitBook 创建的电子书籍，除了实际内容文件外，还应包含如下文件：

* `README.md`:书的介绍文字，如前言、简介，在章节中也可做为章节的简介。
* `SUMMARY.md`:定制书籍的章节结构和顺序。
* `LANGS.md`:多种语言设置。
* `GLOSSARY.md`:词量表和定义描述。  

> `README.md`和`SUMMARY.md`是GitBook 制作电子书的必要文件，可用`gitbook init`命令自动生成，其余文件如有需要，可手动添加。  


## **章节设置**

GitBook 使用`SUMMARY.md`文件作为书籍的目录结构，既多层次章节设置。它同时也被用来制作书籍目录（TOC-Tables Of Contents）。  

`SUMMARY.md`的格式只是简单的连接列表，连接的“名称”就是章节的“标题”，连接标的则是实际内容“文件”（包含路径）。  
章节的层级，就是根据清单的层级关系定义的。  

> 多层级可将书籍分为“部”、“章”、“节”或“小节”，而且不会自动赋予标号或固定名称，选择自己想要的结构即可。  
没有在`SUMMARY.md`中出现的文件，GitBook 在生成各种格式电子书的时候是不会将其包含在内的，因此可以自由撰写草稿、参考文件等，只要不将它们加入到`SUMMARY.md`文件中，就不会被发布。  

## **目录示例**

`Summary.md`

     #Summary
     * [第一章](chapter1.md)
     * [第二章](chapter2.md)
     * [第三章](chapter3.md)

## **多层结构目录示例**

`Summary.md`

     #Summary
     * [第一部](part1/README.md)
        * [写作是没好的](part1/writing.md)
        * [GitBook 也不错](part1/gitbook.md)
     * 第二部
        * [我们欢迎读者回馈](part2/feedback_please.md)
        * [对作者更好的工具](part2/better_tools.md)

ps. 可以看到“第一部”有连接到实际的文件，可以放一个简单的“章节简介”，或特殊的标题或引言，甚至是展现一张图片都可以。而“第二部”则没有连接任何文件，这样在发布书籍时，就有可能导致“第二部”解析错误，后面有连接实际文件的不会受此影响。  

> `README.md`文件默认会作为多层目录结构中的章节连接文件。

## **多语言**

GitBook 支持多种语言编写图书。每种语言必须是一个子目录，子目录结构与 GitBook 结构相同（拥有各自的README.md、SUMMARY.md以及实际内容文件）， `LANGS.md` 在外层父目录（书籍项目根目录），其内容格式如下：

`LANGS.md`

     * [English](en/)
     * [zh-hans](zh-hans/)
     * [zh-tw](zh-tw/)
     

例子 [学习 Git](https://github.com/GitbookIO/git).

## **忽略目录和文件**

GitBook 会读取 `.gitignore`,`.bookignore` 以及 `.ignore` 这三个档案，根据里面的内容，忽略特定的文件或子目录。（格式为一行一个文件或目录。）

`.gitignore`

    #忽略 test.md 文件
    test.md
    
    #忽略 "bin" 目录下所有文件
    bin/*

## **术语表**

在术语表中指定要显示的术语和各自的定义。基于这些条件 gitbook 会自动建立索引，并在页面中高亮显示这些术语。

`GLOSSARY.md`

    # term
    Definition for this term

    # Another term
    With it's definition, this can contain bold text and all other kinds of inline markup ...
