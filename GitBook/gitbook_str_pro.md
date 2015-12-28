# 2.1. GitBook 图书结构介绍

在书籍文件夹中输入`gitbook init`终端命令，会在当前目录下新增两个文件：`README.md`和`SUMMARY.md`,这是除了实际内容文件外，GitBook 制作电子书的必要文件，除此还有可选文件`LANGS.md`和`GLOSSARY.md`，对应含义如下：
* `README.md`:书的介绍文字，如前言、简介，在章节中也可做为章节的简介。
* `SUMMARY.md`:定制书籍的章节结构和顺序。
* `LANGS.md`:多种语言设置。
* `GLOSSARY.md`:词量表和定义描述。  

README.md和SUMMARY.md是书籍必不可少的文件，可用`gitbook init`命令自动生成，其余文件如有需要，可手动添加。