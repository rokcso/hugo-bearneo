# Hugo ʕ•ᴥ•ʔ Bear Blog ✨ Neo

> 免费、简洁、超快速的博客。

[English](../README.md) | [简体中文](./README_zh.md)

基于 [Bear Blog](https://bearblog.dev/) 的 [Hugo](https://gohugo.io/) 主题。

从 [Hugo Bear Blog][hugo-bearblog] 移植而来，由于原作者选择与原版 [Bear Blog](https://bearblog.dev) 保持一致，因此我选择创建一个更具扩展性和功能丰富的 [Hugo Bear Blog][hugo-bearblog]。

准则：

1. 继续坚持 [Bear Blog](https://bearblog.dev) 的理念
2. 保证能通过配置还原到和 [Hugo Bear Blog][hugo-bearblog] 甚至是和 [Bear Blog](https://bearblog.dev) 一致

## ✨ 功能

> 在 [Hugo Bear Blog][hugo-bearblog] 的基础上，增加了以下功能：

- [x] Upvote 文章（亮点功能 👍，复刻自 Bear Blog）
- [x] Follow App Claim
- [x] 文章列表页按年份分组
- [x] 文章页显示目录

## 🐻 示例

要查看此主题的最新状态和实际演示，请访问 [https://rokcso.com/][rokcso-blog] 🎯。

## 📑 使用手册

### Upvote

首先参考 Post Upvote API 的 [README](https://github.com/rokcso/post-upvote-api) 文档，完成后端服务部署。

> 使用 Cloudflare Workers + KV，部署简便且免费。

然后在 Hugo 博客配置文件 `hugo.toml` 中添加如下配置:

```toml
[params]
    upvote = true
    upvoteURL = "刚刚部署的 Worker 的域名/" 
```

注意：URL 末尾的 `/` 一定要加上！

## 🎁 鸣谢

特别感谢 [Herman](https://herman.bearblog.dev)，他创建了最初的 [ʕ•ᴥ•ʔ Bear Blog](https://bearblog.dev/)。

特别感谢 janraasch，没有他的 [hugo-bearblog][hugo-bearblog]，就不会有 [hugo-bearblog-neo][hugo-bearblog-neo]。

## ©️ License

[MIT License](http://en.wikipedia.org/wiki/MIT_License) © [Rokcso][rokcso-blog]

[hugo-bearblog]: https://github.com/janraasch/hugo-bearblog
[hugo-bearblog-neo]: https://github.com/rokcso/hugo-bearblog-neo
[rokcso-blog]: https://rokcso.com/