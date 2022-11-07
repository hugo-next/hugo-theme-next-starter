[中文](https://github.com/hugo-next/hugo-theme-next-starter/blob/main/README.zh.md) | [English](#)

# Hugo NexT theme starter

It's usefully for people who are first time notice Hugo framework and want to create himself blog site. Following steps as below and good luck for you! :tada::tada::tada:

> **Note**
> Before that make sure your PC were installed [Git](https://git-scm.com/downloads) and [Hugo](https://github.com/gohugoio/hugo/releases/) software.

## Deploy on Vercel

Now you can deployment your site on Vercel paltform by this button: [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fhugo-next%2Fhugo-theme-next-starter&env=HUGO_VERSION&envDescription=Enter%20latest%20version%20of%20Hugo%20engine.&envLink=https%3A%2F%2Fgithub.com%2Fgohugoio%2Fhugo%2Freleases%2F&project-name=my-blog&repo-name=my-blog&demo-title=Hugo%20NexT%20Theme&demo-description=Easily%20%26%20powerful%20theme%20of%20Hugo%20engine.&demo-url=https%3A%2F%2Fhugo-next.eu.org%2F&demo-image=https%3A%2F%2Fimgs.lisenhui.cn%2Fhugo-next%2Fhugo-next-demo.png&install-command=git%20submodule%20add%20https%3A%2F%2Fgithub.com%2Fhugo-next%2Fhugo-theme-next.git%20themes%2Fhugo-theme-next)

### ➕ Create Github repository

Please login Vercel with your Github account, then enter your repsitory name and click `Create`, also need enter latest Hugo version at `HUGO_VERSION` parameter, after those action then deploy it.

![deploy-with-vercel-01.png](https://imgs.lisenhui.cn/hugo-next/deploy-with-vercel-01.png)

### 🏗 Change Framework

Because Vercel doesn't defined the framework the site not work at first time, you need change it to `Hugo` and save change.

![deploy-with-vercel-02.png](https://imgs.lisenhui.cn/hugo-next/deploy-with-vercel-02.png)

### 🚧 Redeployment

Switch to `Deployment` tag page, refer to the following snapshot for operation, after a while the site will visit success.

![deploy-with-vercel-03.png](https://imgs.lisenhui.cn/hugo-next/deploy-with-vercel-03.png)

## ⏬ Clone Theme

Click the green button which name call `Use this template` and upper right corner on the page. Full information such as below image:

![Use Template](https://imgs.lisenhui.cn/hugo-next/use-hugo-next-starter.png)

After do that click the green button which name call `Create repository from template`, then will create your site code automatic, and clone it on your PC environment.

Remember that need use `git submodule` command to pull all things from `hugo-theme-next` at first time.

```
# First time
git submodule update --init --recursive
# Next time
git submodule update --remote --merge
```

> **Note**
> When you are in China, recommend to use `Gitee` repository url replace the submodule url in `.gitmodules` file content and then execute the above `Git` command line to improve the speed.

## 💻 Local Preview

Execute the `startup.sh` boot start script file which is under site root directory, when see some words like `stop` that mean success, and open browser visit
 [http://localhost:1414/](http://localhost:1414/) will enjoy yourself.

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

## 🎨 Snapshot

![Hugo NexT Demo](https://imgs.lisenhui.cn/hugo-next/hugo-next-demo.png)

## 🎉 Deployment

Use `hugo` command to build site's static files, and deploy them into Web server just like `Nginx` and so on. Or you can enable `Github Page` function when you commit your local things there will build static files by automatic, more info:[Github Pages](https://pages.github.com/).


> **Note**
> Please relpace actual parameter's value in `config/_default/params.yaml` config file before deploy, such as comment, analytis, share and so on.

## 📜 License

[MIT License](LICENSE)

Copyright (c) 2022, hugo-next teams.