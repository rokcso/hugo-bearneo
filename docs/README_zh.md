# Hugo ʕ•ᴥ•ʔ Bear Blog ✨ Neo

> 免费、简洁、超快速的博客。

[English](../README.md) | [简体中文](./README_zh.md)

基于 [Bear Blog](https://bearblog.dev/) 的 [Hugo](https://gohugo.io/) 主题。

从 [Hugo Bear Blog][hugo-bearblog] 移植而来，由于原作者选择与原版 [Bear Blog](https://bearblog.dev) 保持一致，因此我选择创建一个更具扩展性和功能丰富的 [Hugo Bear Blog][hugo-bearblog]。

**准则**

1. 继续坚持 [Bear Blog](https://bearblog.dev) 的理念
2. 保证能通过配置还原到和 [Hugo Bear Blog][hugo-bearblog] 甚至是和 [Bear Blog](https://bearblog.dev) 一致

**目录**

- [✨ 功能](#-功能)
- [🐻 示例](#-示例)
- [📑 使用手册](#-使用手册)
    - [点赞文章](#点赞文章)
    - [搜索文章](#搜索文章)
    - [文章列表页按年份分组](#文章列表页按年份分组)
    - [显示目录](#显示目录)
    - [图片缩放](#图片缩放)
    - [Follow App Claim](#follow-app-claim)
- [🎁 鸣谢](#-鸣谢)
- [©️ License](#️-license)

## ✨ 功能

在 [Hugo Bear Blog][hugo-bearblog] 的基础上，增加了以下功能：

- [x] 点赞文章（亮点功能 👍，复刻自 Bear Blog）
- [x] 搜索文章
- [x] 文章列表页按年份分组
- [x] 显示目录
- [x] 图片缩放
- [x] Follow App Claim

还有一些优化项：

- 添加 canonical 元数据，更好的 SEO
- 支持 RSS
- 更丰富的 Footer 内容
- ……

## 🐻 示例

要查看此主题的最新状态和实际演示，请访问 [https://rokcso.com/][rokcso-blog] 🎯。

## 📑 使用手册

### 点赞文章

首先参考 Post Upvote API 的 [README](https://github.com/rokcso/post-upvote-api) 文档，完成后端服务部署。

> 使用 Cloudflare Workers + KV，部署简便且免费。

然后在 Hugo 博客配置文件 `hugo.toml` 中添加如下配置:

```toml
[params]
    upvote = true
    upvoteURL = "刚刚部署的 Worker 的域名/"
```

注意：URL 末尾的 `/` 一定要加上！

### 搜索文章

在文章列表页面显示搜索框，输入文章标题关键词以搜索特定文章。

在 Hugo 博客配置文件 `hugo.toml` 中添加如下配置：

```toml
[params]
    postSearch = true
```

### 文章列表页按年份分组

在 Hugo 博客配置文件 `hugo.toml` 中添加如下配置:

```toml
[params]
    groupByYear = true
```

### 显示目录

在 Hugo 博客配置文件 `hugo.toml` 中添加如下配置:

```toml
[params]
    toc = true
```

### 图片缩放

在 Hugo 博客配置文件 `hugo.toml` 中添加如下配置:

```toml
[params]
    imageZoom = true
```

### Follow App Claim

[Follow](https://follow.is/) 是一个 RSS 订阅工具，作为博客创作者，在 Follow 中 Claim 自己的博客可以接收博客读者通过 Follow 提供的 $POWER 打赏。对此我曾经写过一篇 [文章](https://rokcso.com/p/follow-claim-feed/) 介绍如何在 Follow 中 Claim 自己的博客。

而 hugo-bearneo 原生支持了我文章中提到的「方案三：RSS Tag」，只需要在 Hugo 博客配置文件 `hugo.toml` 中添加如下配置：

```toml
[params]
    followFeedId = "00000000000000000"
    followUserId = "00000000000000000"
```

注意：请记得将配置中的 follow id 替换为你自己的！

## 🎁 鸣谢

特别感谢 [Herman](https://herman.bearblog.dev)，他创建了最初的 [ʕ•ᴥ•ʔ Bear Blog](https://bearblog.dev/)。

特别感谢 janraasch，没有他的 [hugo-bearblog][hugo-bearblog]，就不会有 [hugo-bearneo][hugo-bearneo]。

## ©️ License

[MIT License](http://en.wikipedia.org/wiki/MIT_License) © [Rokcso][rokcso-blog]

[hugo-bearblog]: https://github.com/janraasch/hugo-bearblog
[hugo-bearneo]: https://github.com/rokcso/hugo-bearneo
[rokcso-blog]: https://rokcso.com/
