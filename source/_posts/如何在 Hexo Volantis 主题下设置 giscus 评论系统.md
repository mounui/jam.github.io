---
title: 如何在 Hexo Volantis 主题下设置 giscus 评论系统
date: 2024-01-08 16:18:39
categories: [Hexo]
tags: [Hexo,Volantis,博客,评论,giscus]
---

[giscus](https://giscus.app/) 是一个基于 GitHub Discussions 构建的评论插件。 它允许用户在任何系统、网站或博客上通过 GitHub 讨论进行交互和评论。以着简单的方式，你可以在你的网页上嵌入giscus，并把GitHub的讨论区的功能扩展到你的网页或者博客上。这个评论系统使用起来非常方便，并且有了GitHub的支持，你的数据都是安全且容易管理的。

##### 1、Github创建新仓库

![image-20240108162628918](https://res.mounui.com/2024/bd7a55de9657a9dd74d469a515ae93ec836b57.png)

##### 2、安装giscus

- 点击这个链接安装：**[GitHub Apps - giscus](https://github.com/apps/giscus)**
- 选择刚建立的仓库，点击install

![image-20240108162852612](https://res.mounui.com/2024/cd85bcfec7db6d039dfc7f002209d9ce265710.png)

##### 3、配置仓库

首先打开仓库的setting，将Discussions部分打上对号，然后建立一个Announcements的分类

![image-20240108163139368](https://res.mounui.com/2024/fb2bf4c52adeb49409054a412791d7faa23ea2.png)

##### 4、进入[giscus](https://giscus.app/)配置

![image-20240108163656333](https://res.mounui.com/2024/d33adb8fd4dffbf8f32f970e911304c2927d16.png)

配置完上述部分后，在启动giscus下边复制几个东西

![image-20240108163955170](https://res.mounui.com/2024/24ae95e000083608ad6e6414a46c28232cc240.png)

将上面复制的内容填到 Volantis 主题配置文件里

![image-20240108164258081](https://res.mounui.com/2024/f1f05f9504aa4b93d69f0416f9de9093ec8bfa.png)

##### 5、重建 Hexo 网站

保存你的修改并执行 `hexo clean && hexo generate && hexo server` 命令来重新生成你的网站。现在，你应该可以在你的[博客](https://jam.mounui.com)文章下看到 giscus 评论系统了。

![image-20240108164425214](https://res.mounui.com/2024/df9c2e5101d293f1aaa3ee8c252eaa7f9d6ba1.png)

##### 总结

以上就是在 Hexo Volantis 主题环境下配置 Giscus 评论系统的步骤。希望这篇文章对你有所帮助！如若遇到任何问题，欢迎在评论区留言讨论。
