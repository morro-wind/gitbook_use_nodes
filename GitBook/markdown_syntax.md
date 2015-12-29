# 2.2 Markdown 标记语法
GitBook 使用Markdown 标记语法。  
本节仅简要介绍 Markdown 的基本语法与展现，若要详细了解，英文资源可以看其发明人的说明：[Jon Gruber's original spec](http://daringfireball.net/projects/markdown/) 以及GitHub 的扩展版 [Github-flavored Markdown infoj](http://github.github.com/github-flavored-markdown/) page。[Markdown.cn](http://markdown.cn)有其中文详解；想看看俗称 GFM-GitHub 风格的 Markdown 语法，也找得到[中文翻译](https://github.com/cssmagic/blog/issues/13)。  

# **标题**
     # H1
     ## H2
     ### H3
     #### H4
     ##### H5
     ###### H6
     
     最常使用的是 H1 和 H2 标题，还有更明显的另一种写法：
     
     Alt-H1
     ======
     
     Alt-H2
     ------
> 此处`-`是负号，不是`_`下横号，`_`下横号，显示的是双横线

# H1
## H2
### H3
#### H4
##### H5
###### H6

最常使用的是 H1 和 H2 标题，还有更明显的另一种写法：

Alt-H1
======

Alt-H2  
------

# **强调语法**
     强调，例如意大利斜体，可以使用 *asterisks* 或 _underscores_。  
     加重语气强调，例如粗体，可以用 **asterisks** 或 __underscores__ 。
     可以混用这两种 **asterisks and _underscores_**。
     给文字加上删除线，是这样 ~~Scratch this.~~
# **清单**
下面的示例为了清楚展示缩排时需要的空格，使用了点号，实际撰写时只需要相同数量的空格。  
     1. 第一则列表项目
     2. 另一个项目
     ..* 无序的次清单
     1. 数字本身是否排序并不重要，统统使用相同的数字也可以
     ..1. 排序的次清单
     4. 另一个项目
     
     ...可以在一则项目中使用缩进的段落格式。注意上面的**空行**，还有本段前的**空格**(至少一个，我们使用了三个，展示的更清楚)
     
     ...在一个段落中**强制换行**，在语句后方加入两个**空格**。..
     ...这个被强制设置的独立行，依旧在同一个段落中。..
     ...（有些人觉得使用空格强制换行太麻烦，例如 GFM 就不需要）。
     
     * 可以使用星号建立无序清单
     - 或是短横线（负号）
     + 使用半形加号也可以

# **连接设置**
有两种方式可以建立文中的链接。  
     [这是一个行内链接](https://www.gitbook.com)  
     
     [这是一个带有标题的行内链接](https://www.gitbook.com "GitBook's Homepage")  
     
     [这是一个参考链接][Arbitrary
     case-insensitive reference text]  
     
     [这是一个对应到 Git 仓库文件的相对参考链接](../blob/master/LICENSE)  
     
     [参考标的物也可以使用数字][1]  
     
     直接使用文字对应也可以 [这段文字链接到参考项目]
     
     参考项目可以写在文档的最后，有点像书内的注解（注脚）。
     
     [arbitrary case-insensitive reference text]: https://www.mozilla.org
     [1]: http://slashdot.org
     [这段文件链接到参考项目]: http://www.reddit.com

# **图片**
     这是我们的 logo （将鼠标移动到图片上会显示图片标题）：  
     行内格式：  
     ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo 标题文字示例一")
     
     参考链接结构：
     ![alt text][logo]
     
     [logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo 标题文字示例二"
     
# **程序代码与语法高亮标示**
     行内 `code` 必须使用 `back-ticks` 将文字包起来(一般在键盘左上方的地一个键)。