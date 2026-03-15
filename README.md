# Simon taking a breather

A personal blog built with Hugo + PaperMod theme, deployed on GitHub Pages.

## 🚀 Quick Start

### Local Preview

```bash
# Enter project directory
cd my-blog

# Start development server
hugo server -D

# Visit http://localhost:1313
```

### Create New Post

```bash
hugo new content posts/article-title.md
```

### Build Site

```bash
hugo --minify
```

## 📁 Project Structure

```
my-blog/
├── archetypes/      # Content templates
├── assets/          # Asset files
├── content/         # Site content
│   ├── archives.md  # Archives page
│   ├── search.md    # Search page
│   └── posts/       # Blog posts
├── data/            # Data files
├── layouts/         # HTML templates
├── static/          # Static files
├── themes/          # Themes
│   └── PaperMod/    # PaperMod theme
├── hugo.toml        # Site configuration
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions deployment config
```

## 📝 Writing Guide

### Post Front Matter

```yaml
---
title: "Article Title"
date: 2026-03-14T12:00:00+08:00
draft: false
tags: ["tag1", "tag2"]
categories: ["Category"]
author: "Simon"
description: "Article description"
ShowToc: true      # Show table of contents
TocOpen: false     # TOC collapsed by default
---
```

### Common Shortcodes

PaperMod theme provides rich shortcodes, see [official documentation](https://github.com/adityatelange/hugo-PaperMod/wiki) for details.

## 🌐 Deployment

GitHub Actions is configured. Pushing code to `main` branch will automatically build and deploy to GitHub Pages.

## 🔧 Configuration

Site configuration is in `hugo.toml`, main options:

- `baseURL` - Site URL (modify to your GitHub Pages URL before deployment)
- `title` - Site title
- `params` - Theme parameters
- `menu` - Navigation menu

## 📄 License

MIT License
