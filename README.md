# Hugo ʕ•ᴥ•ʔ Bear Blog ✨ Neo

> Free, no-nonsense, super-fast blogging.

[English](./README.md) | [简体中文](./doc/README_zh.md)

🧸 A [Hugo](https://gohugo.io/) theme based on [Bear Blog](https://bearblog.dev).

Transplanted from [Hugo Bear Blog][hugo-bearblog], because the original author chose to maintain consistency with the root original [Bear Blog](https://bearblog.dev), so I chose to create a more extensible and feature-rich [Hugo Bear Blog][hugo-bearblog].

**TOC**

- [Hugo ʕ•ᴥ•ʔ Bear Blog ✨ Neo](#hugo-ʕᴥʔ-bear-blog--neo)
  - [✨ Features](#-features)
  - [🐻 Demo](#-demo)
  - [📑 User Manual](#-user-manual)
    - [Upvote](#upvote)
  - [🎁 Acknowledgments](#-acknowledgments)
  - [©️ License](#️-license)

## ✨ Features

> Based on [Hugo Bear Blog][hugo-bearblog], the following features have been added:

- [x] Upvote post (Highlight feature 👍, Replicated from Bear Blog)
- [x] Follow App Claim
- [x] Post list page grouped by year
- [x] Post page displays table of contents

## 🐻 Demo

For a current & working demo of this theme, please check out [https://rokcso.com/][rokcso-blog] 🎯.

## 📑 User Manual

### Upvote

First, refer to the [README](https://github.com/rokcso/post-upvote-api) documentation of the Post Upvote API to complete the deployment of the backend service.

> Using Cloudflare Workers + KV, deployment is simple and free.

Then add the following configuration to the Hugo blog configuration file `hugo.toml`:

```toml
[params]
    upvote = true
    upvoteURL = "The domain name of the Worker that was just deployed/" 
```

Note: The `/` at the end of the URL must be included!

## 🎁 Acknowledgments

A special thank you goes out to [Herman](https://herman.bearblog.dev), for creating the original [ʕ•ᴥ•ʔ Bear Blog](https://bearblog.dev/).

Another special thanks to janraasch, without his [hugo-bearblog][hugo-bearblog], there would not be [hugo-bearblog-neo][hugo-bearblog-neo].

## ©️ License
[MIT License](http://en.wikipedia.org/wiki/MIT_License) © [Rokcso][rokcso-blog]

[hugo-bearblog]: https://github.com/janraasch/hugo-bearblog
[hugo-bearblog-neo]: https://github.com/rokcso/hugo-bearblog-neo
[rokcso-blog]: https://rokcso.com/