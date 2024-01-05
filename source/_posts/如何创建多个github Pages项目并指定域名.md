---
title: 如何创建多个github Pages项目并指定域名
date: 2024-01-05 17:24:58
tags: [github,github pages,博客]
---

在这篇文章中，我将讲述如何为你的多个GitHub项目生成GitHub Pages，并指定一个域名。这将是一个简单的步骤，只需要一点点GitHub知识就可以完成。

GitHub Pages提供了两种类型的网页：用户页和项目页。

- **用户页**是基于你的用户名的，一般格式为`username.github.io`，在这种情况下，我的GitHub Pages用户页就是`tdoly.github.io`。这种格式的页面存储在仓库的主分支上。

- **项目页**，它们是基于你的项目的，格式通常为`username.github.io/repository`。这种类型的页面存储在该仓库的`gh-pages`分支或者主分支上。

### 步骤一：为你的项目创建GitHub Pages

在你的GitHub仓库中，
1. 选择`Settings`选项
2. 滚动到`GitHub Pages`区域
3. 选择你的页面来源分支，一般是主分支或者`gh-pages`分支。

### 步骤二：为你的项目指定一个域名

可以在你的仓库中创建一个`CNAME`文件，文件中需要包含你希望绑定的域名。

> **注意**：尽管你可以为同一个用户下的多个项目设置 GitHub Pages，但你只能向一个用户页绑定一个域名。如果你试图为其他项目页绑定域名，那你的用户页的域名可能会失效。

总的来说，为你的多个GitHub项目生成GitHub Pages并指定域名是一个强大的功能，它允许你轻松快速地部署并公开你的项目。你可以使用这个功能来展示你的项目，或者作为一个个人或项目博客使用。
