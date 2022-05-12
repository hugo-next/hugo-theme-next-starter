[中文](README.zh.md) | [English](README.md)

# Hugo NexT theme starter

# 1. Update the submodule

Check in the repository folder then use the below git command line check out latest `hugo-theme-next` theme version.

```
# First time
git submodule update --init --recursive
# Next time
git submodule update --remote --merge
```

> Notice: When you are in China, recommend to use `Gitee` repository url replace the submodule url in `.gitmodules` file content and then execute the above `Git` command line to improve the speed.

# 2. Deploy & Browser visit

Check in the repository folder then use the Hugo command line deploy in local & open browser input default url [http://localhost:1313/](http://localhost:1313/) to visit site.

```
hugo server
```

# 3. Preview

![my-hugo-blog](https://lisenhui.gitee.io/imgs/blog/my-hugo-blog.png)

# 4. License

[MIT License](LICENSE).