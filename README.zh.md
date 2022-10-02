[中文](README.zh.md) | [English](README.md)

# Hugo NexT 主题启动器

本启动器是为初学者所准备的，如果你正在准备搭建个人博客站，那么参考如下步骤便可快速完成。加油，祝你好运！:tada::tada::tada:

> **Note**
> 请确认你的电脑上已经安装有 [Git](https://git-scm.com/downloads) 和 [Hugo](https://github.com/gohugoio/hugo/releases/) 两款软件。

## ⏬ 克隆主题

点击右上角的 `Use this template` 绿色按钮然后填写代码仓库的相关信息，参考如下：

![使用模板创建](https://imgs.lisenhui.cn/hugo-next/use-hugo-next-starter.png)

最后点击 `Create repository from template` 绿色按钮，会直接在你的空间中生成站点代码，再使用`git clone`命令把它克隆到本地进行创作。

记得首次完全克隆后，需要在根目录中使用如下的 `Git` 子模块更新命令拉取 `hugo-theme-next` 主题的最新版本。

```
# 首次初始化操作
$ git submodule update --init --recursive
# 后续更新操作
$ git submodule update --remote
```

> **Note**
> 注意：当你在中国境内，建议先将 `.gitmodules` 的仓库指向 `Gitee` 地址，再执行上述的命令速度会更快。

## 💻 本地预览

在站点根目录下，执行自带的 `startup.sh` 启动脚本，当看到输出信息中带有 `stop` 字样时便表示启动成功，此时打开浏览器输入默认地址[http://localhost:1414/](http://localhost:1414/)访问浏览效果。

```shell
$ sh startup.sh
========================================
  ███╗   ██╗███████╗██╗  ██╗████████╗
  ████╗  ██║██╔════╝╚██╗██╔╝╚══██╔══╝
  ██╔██╗ ██║█████╗   ╚███╔╝    ██║
  ██║╚██╗██║██╔══╝   ██╔██╗    ██║
  ██║ ╚████║███████╗██╔╝ ██╗   ██║
  ╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝   ╚═╝
========================================
Hugo NexT version 4.3.1
Documentation: https://hugo-next.eu.org
========================================
Start building sites …
hugo v0.102.3-b76146b129d7caa52417f8e914fc5b9271bf56fc+extended windows/amd64 BuildDate=2022-09-01T10:16:19Z VendorInfo=gohugoio

                   | ZH-CN
-------------------+--------
  Pages            |    71
  Paginator pages  |     0
  Non-page files   |     0
  Static files     |    43
  Processed images |     0
  Aliases          |    26
  Sitemaps         |     1
  Cleaned          |     0

Built in 233 ms
Watching for changes in C:\xxx\hugo-theme-next-starter\{content,data,themes}
Watching for config changes in C:\xxx\hugo-theme-next-starter\config\_default
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at //localhost:1414/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

## 🎨 效果预览

![Hugo NexT Demo](https://imgs.lisenhui.cn/hugo-next/hugo-next-demo.png)

## 🎉 发布

执行 `hugo` 命令生成全站静态文件，并把文件部署到类似 `Nginx` 的 Web 服务器即可。若如自己没有服务器的话，也可以直接开启 `Github Pages` 功能，会在你推送本地文件到服务器时，自动生成站点的静态文件，使用详情可关注：[Github Pages](https://pages.github.com/)。

## 📜 许可证

[MIT 许可证](LICENSE)

Copyright (c) 2022， hugo-next 团队