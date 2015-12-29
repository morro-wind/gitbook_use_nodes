# **2.4. Git 更新**

本节只简单的介绍几个 `git` 命令

每一本书籍都对应一个Git HTTPS网址， GitBook的 git 主机还不接受 ssh 传输协议。

网址看起来像这样：

    https://git.gitbook.com/{{UserName}}/{{Book}}.git

**授权认证**

主机需要认证你的 GitBook 帐号，跳出提示时输入你的 GitBook 账户名称和密码即可（可以使用专属的 API token）

**存储你的认证许可 (credentials)**

为了省去每次推送内容时都得输入帐号密码的麻烦，可以把 GitBook 的认证许可写到 `~/.netrc` 文件里。
新建或添加下面的内容到 `~/.netrc` 文件：

    machine git.gitbook.com
      login USERNAME-or-EMAIL
      password API-TOKEN-or-PASSWORD

建议使用 **API TOKEN** ,因为安全性更高些；可以从[网站后台](https://www.gitbook.com/settings#api)的“API”选项中找到属于你的相信息。

建立新的书籍项目

    touch README.md SUMMARY.md
    git init
    git add README.md SUMMARY.md
    git commit -m "first commit"
    git remote add gitbook https://git.gitbook.com/{{UserName}}/{{Book}}.git
    git push -u gitbook master

推送到已有书籍项目

    git remote add gitbook https://git.gitbook.com/{{UserName}}/{{Book}}.git
    git push -u gitbook master