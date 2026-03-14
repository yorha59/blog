# Simon 的技术博客

使用 Hugo + PaperMod 主题搭建的个人技术博客，部署在 GitHub Pages 上。

## 🚀 快速开始

### 本地预览

```bash
# 进入项目目录
cd my-blog

# 启动开发服务器
hugo server -D

# 访问 http://localhost:1313
```

### 创建新文章

```bash
hugo new content posts/文章标题.md
```

### 构建站点

```bash
hugo --minify
```

## 📁 项目结构

```
my-blog/
├── archetypes/      # 内容模板
├── assets/          # 资源文件
├── content/         # 网站内容
│   ├── archives.md  # 归档页面
│   ├── search.md    # 搜索页面
│   └── posts/       # 博客文章
├── data/            # 数据文件
├── layouts/         # HTML 模板
├── static/          # 静态文件
├── themes/          # 主题
│   └── PaperMod/    # PaperMod 主题
├── hugo.toml        # 站点配置
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions 部署配置
```

## 📝 写作指南

### 文章 Front Matter

```yaml
---
title: "文章标题"
date: 2026-03-14T12:00:00+08:00
draft: false
tags: ["tag1", "tag2"]
categories: ["分类"]
author: "Simon"
description: "文章描述"
ShowToc: true      # 显示目录
TocOpen: false     # 目录默认折叠
---
```

### 常用 Shortcodes

PaperMod 主题提供了丰富的 shortcodes，详见[官方文档](https://github.com/adityatelange/hugo-PaperMod/wiki)。

## 🌐 部署

项目配置了 GitHub Actions，推送代码到 `main` 分支会自动构建并部署到 GitHub Pages。

## 🔧 配置说明

站点配置在 `hugo.toml` 中，主要配置项：

- `baseURL` - 网站地址（部署前需要修改为你的 GitHub Pages 地址）
- `title` - 网站标题
- `params` - 主题参数
- `menu` - 导航菜单

## 📄 许可证

MIT License
