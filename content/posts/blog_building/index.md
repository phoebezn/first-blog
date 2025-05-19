---
title: "用Hugo建博客"
date: 2025-04-13
categories: [技术]
tags:
  - Hugo
  - 建站
  - PaperMod
---

## 博客搭建的第一个周末

离职不代表不写代码，未来的路，代码也许还会在生命里时常出现。

通过这个[Hugo新手教程](https://gohugo.io/getting-started/quick-start/)搭建了第一个博客。
theme 虽然很想用 `PaperMod`，但是在安装过程中卡住了，所以选择了`ananke`，确实更加简单。之后或许会继续更改吧。
[Hugo Themes](https://themes.gohugo.io/)

因为Hugo 0.146.3版本更新导致PaperMod调用partials时出现问题，所以暂时没有必要更换主题。更新至0.146.4之后，成功换成`PaperMod`主题。很多过去的教程都在用`config.yml`，所以尽管初始设置文件是`hugo.toml`，我还是改成了用`config.yml`。目前在根据[PaperMod Repo](https://github.com/adityatelange/hugo-PaperMod)做一些更新。

## 目前博客的设置
Hugo version
```
hugo version
hugo v0.146.4+extended+withdeploy darwin/arm64 BuildDate=2025-04-14T13:10:30Z VendorInfo=brew
```
Directory Tree
```
.(site root)
├── hugo.yaml
├── content
│   ├── posts
│   │   ├── first_post
│   │   │   ├── index.md
│   │   │   ├── image.jpg
└── themes
    └── PaperMod
```

## Basic usage

To view your site while developing layouts or creating content, cd into your project directory and run:
```
hugo server
```

[Hugo - Basic usage](https://gohugo.io/getting-started/usage/)



## Host on GitHub Pages
[Hugo - Host on GitHub Pages](https://gohugo.io/host-and-deploy/host-on-github-pages/)