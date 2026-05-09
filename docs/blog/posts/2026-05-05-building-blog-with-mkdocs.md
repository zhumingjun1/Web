---
date: 2026-05-05
categories:
  - 技术
  - web
tags:
  - mkdocs
  - github-pages
  - 教程
authors:
  - your-name
slug: building-blog-with-mkdocs
---

# 用 MkDocs 和 GitHub Pages 搭建博客

一份创建类似本博客的静态博客的分步指南。

<!-- more -->

## 准备工作

- Python 3.8 或更高版本
- Git
- 一个 GitHub 账户

## 第 1 步：安装 MkDocs Material

```bash
pip install mkdocs mkdocs-material mkdocs-rss-plugin
```

## 第 2 步：创建新项目

```bash
mkdocs new my-blog
cd my-blog
```

## 第 3 步：配置博客插件

在 `mkdocs.yml` 中添加博客插件：

```yaml
plugins:
  - blog:
      blog_dir: blog
      post_dir: blog/posts
```

## 第 4 步：写第一篇文章

在 `docs/blog/posts/` 中创建一个带 frontmatter 的 Markdown 文件：

```yaml
---
date: 2024-03-10
categories:
  - 技术
---
```

## 第 5 步：部署到 GitHub Pages

```bash
mkdocs gh-deploy --force
```

搞定！你的博客现在已经上线了，访问地址是 `https://<用户名>.github.io/<仓库名>/`。

---

搭建博客从未如此简单。祝你写作愉快！
