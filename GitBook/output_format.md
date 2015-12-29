# **2.4. 生成格式**

完成书籍撰写，就可以生成需要的格式进行发布了。

## **HTML网页版本**

在书籍项目目录的跟目录输入 `gitbook install` ，会自动安装必要的插件与书籍项目指定的插件。

指定插件是由 `book.json` 这个文件控制，这里没有用到，因此GitBook只会预先安装一个 **high light** 插件，用来显示书中插入程序代码区段。(使用 `gitbook serve` 还会自动启用另一个 **livereload** 插件，用于自动重载更新后的页面。)

整个静态格式书籍会放在 `_book` 目录下，若是不需要通过浏览器查看，也可使用 `gitbook build` 构建。

可以把整个html目录上传到自己的网站空间，就连GitHub Pages 空间都可以用。

## **制作电子书文件**

从书籍项目更目录执行：

* `gitbook epub` 制作 ePub 电子书
* `gitbook mobi` 制作 Kindle 电子书
* `gitbook pdf` 制作PDF电子书

## **完整命令**

也可以从书籍项目外部执行，完整命令是：

    gitbook epub [book] [output]

例如 `gitbook mobi ~/ebook/mybook ~/Desktop/mybook.mobi` 。制作电子书制定 `output` 时需包含完整的路径和文件名称。

想要将静态网站建立到指定目录，可以这样输入：

    gitbook build --output=/site/mybook

输入 `gitbook help` 可以看到帮助信息。

## **结论**

GitBook 可以说是未来出版的一个发展趋势，而且还在持续进化之中。

一般使用桌面客户端编辑器，或在线编辑器即可，只要注意草稿分支的使用技巧，完全不懂技术也能制作各种电子书籍。不怕终端命令、略懂 Node 和 NPM 的，可搭配 `gitbook-cli` 和 Calibre 则可以使用 GitBook 的所有功能。

下一步进阶，就是“使用模板、插件”等，可参考 GitBook 的[中文繁体说明](https://www.gitbook.com/book/wastemobile/gitbook-chinese/details)

此指南到此就全部结束。

谢谢！