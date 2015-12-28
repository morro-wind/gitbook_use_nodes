#**准备工作和所具备知识**

如果您只是使用gitbook.com的在线编辑器或客户端，那您只需学会如何使用gitbook工具即可。而如果您想脱离gitbook.com的编辑器去创建一部电子书籍的话，就会涉及到Node.js和Markdown。

gitbook是Node.js代码库的命令工具，使用GitHub/Git与Markdown(或AsciiDoc)就能制作漂亮的电子书籍。

上面所涉及到的知识不会也没关系，我会介绍些简单知识，为了达到独立制作电子书的目的。

##**需要安装的软件**
除了使用gitbook.com的在线编辑器外，还需安装一下软件。
* **GitBook Editor 客户端编辑器**

  GitBook Editor 是一个适合任何平台的客户端，下载地址：https://www.gitbook.com/editor

* **Node.js**

  Node.js是一个基于Chrome V8引擎的JavaScript运行环境。Node.js使用了一个事件驱动、非阻塞式I/O的模型，使其轻量又高校。Node.js的包管理器npm，是全球最大的开源库生态系统。下载地址:https://wwww.nodejs.org/en/download/ 或http://nodejs.cn/download/  
 >node.js有多种安装方式，可以下载编译好的二进制包解压后直接使用，也可通过包管理器安装，还可通过下载源码包编译安装。  

 > 通过包管理器的安装方式请参照[官方文档](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)  
 这里我简单介绍下使用源码编译安装。  
 1.下载node.js源码  
      $wget https://nodejs.org/dist/v4.2.4/node-v4.2.4.tar.gz
      $tar zxf node-v4.2.4.tar.gz && cd node-v4.2.4
      $
* **npm**  

  NPM的全称是Node Package Manager,是Node.js包管理和分发工具。通过此工具安装gitbook-client
  
* **Markdown**

  Markdown是一种轻量级标记语言，创始人为约翰 格鲁伯(John Gruber)。它允许人们“使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML(或HTML)文档”。
  这种语言吸收了很多在电子邮件中已有的纯文本标记的特性。
  ——维基百科
  
####**说明**
本笔记所有操作均是基于ubuntu 14.04 x86_64平台  

## **常见错误**
