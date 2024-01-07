---
title: 使用Hexo+Github搭建个人博客
date: 2024-01-05 16:35:17
tags: [hexo,博客,github]
---

个人网站可以方便地展示你的思想、成果，甚至更好地进行个人品牌设计。[Hexo](https://hexo.io/)和[GitHub](https://github.com/)是搭建个人网站非常优秀的技术组合。现在让我们开始详细的搭建教程：

<img src="https://res.mounui.com/2024/d4c1239e75c02e8482c22017a6c8d407cd63b1.png" alt="5bb7J7NT"  />

## 准备工作

首先，在你的电脑上需要安装以下环境：

- [Node.js](https://nodejs.org/en/download/)：Hexo是基于Node.js开发的。
- [Git](https://git-scm.com/download/win)：版本管理工具，也是我们部署到Github的必备工具。

你可以通过访问官方网站下载安装包，也可以通过命令行工具来进行安装。按照官方教程步骤安装好后，可以在命令行使用`node -v`和`git --version`命令检查是否安装成功。

![Snipaste_2024-01-06_20-26-40](https://res.mounui.com/2024/2bbb03f9c0cd04c63d896191c276452eef626d.png)

## 安装Hexo

通过npm（Node.js的包管理器）全局安装Hexo。打开终端，运行以下命令：

```bash
$ npm install -g hexo-cli
```

如果出现权限错误，请确保你有管理员权限，或者使用`sudo`命令。

## 创建并初始化网站

选择一个目录作为你的博客文件要存放的地方，然后在终端执行下面的命令，`myblog`是你博客的文件夹名，你可以自由地更换：

```bash
$ hexo init myblog
$ cd myblog
```

以上命令执行后，Hexo将会在myblog文件夹中创建必要的文件，并自动进行初始化。

## 安装依赖

在你的博客文件夹下，执行下面的命令来安装必要的依赖包：

```bash
$ npm install
```

## 生成静态网页

在你的博客文件夹下，通过执行下面的命令，Hexo将会在public文件夹中生成博客的静态网页，这些都是用来部署到Github的：

```bash
$ hexo generate
```

## 创建Github Pages仓库

在Github上创建新的仓库，注意仓库名的格式应为`yourusername.github.io`。然后在仓库的Settings页面，找到GitHub Pages选项，更改Source为main branch。

## 配置Hexo部署选项

回到你的博客根目录下，找到并打开文件_config.yml，找到deploy选项，并按以下格式更改：

```bash
deploy:
  type: git
  repository: git@github.com:yourname/yourname.github.io.git
  branch: main
```

## 部署到Github

在终端，执行如下命令来进行部署：

```bash
$ npm install hexo-deployer-git
$ hexo deploy
```

根据网络情况，等待一段时间，你的博客就会自动部署到github的pages服务上。

## 查看你的博客

最后，只需在浏览器中键入 `yourname.github.io`，你就能看到你自己的博客啦！

这只是基础的博客搭建，以后你还可以根据自己的需求来个性化你的博客，比如更换主题，添加评论系统等。尽情享受你的博客旅程吧！