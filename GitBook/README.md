# **2.GitBook 终端基础**
Gitbook 其实是一个终端命令工具。  
无论使用在线编辑器还是本地编辑器，还是使用文本编辑器（如Sublime Text）再推送到仓库，都是使用gitbook.com服务端生成的电子书。这样一来就无法在本地生成电子书籍预览查看或发布到别的平台（如将HTML格式发布到web服务上），而解决这个问题的工具，就是gitbook终端命令工具了。  
使用gitbook命令的前提，必须已经安装好`Node`、`Npm`,在准备工作中，我们已经将它们安装并配置好了，现在来查看下版本。  

      $node --version
      v4.2.3
---
      $npm -version
      2.14.7
##**安装gitbook-cli**
gitbook 终端命令工具，真正使用的是gitbook-cli命令。  

      npm install -g gitbook-cli  
