[中文](README.zh.md) | [English](README.md)

# Hugo 版本 NexT 主题快速启动器

# 1. 更新主题模块

在根目录中使用如下的 `Git` 子模块更新命令拉取 `hugo-theme-next` 主题的最新版本。

```
# 首次初始化操作
git submodule update --init --recursive
# 后续更新操作
git submodule update --remote --merge
```

> 注意：当你在中国境内，建议先将 `.gitmodules` 的仓库指向 `Gitee` 地址，再执行上述的命令速度会更快。

# 2. 发布和浏览

在根目录中使用如下 `Hugo` 命令启动服务生成静态站点，打开浏览器输入默认地址[http://localhost:1313/](http://localhost:1313/)访问浏览效果。

```
hugo server
```

# 3. 预览

![my-hugo-blog](https://lisenhui.gitee.io/imgs/blog/my-hugo-blog.png)

# 4. 许可证

[MIT 许可证](LICENSE).