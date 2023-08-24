---
title: 帮助你从零开始搭建基于 Hexo 的个人博客！（持续更新中）
slug: crate-hexo-blog
date: 2023-04-27
categories:
- note4web
---

> 想着做一个系列视频来输出自己的建站经验，教大家如何制作个人博客，权衡利弊后，打算先写一篇博客尝试一下！

## 摘要

本文将从零开始教你如何创建一个属于你自己的、基于 Hexo 框架的静态个人博客，并通过 Github 与 Vercel 两个平台对你所创建的静态个人博客进行自动化部署，以实现对外界的展示。

## 前置条件

### 所需具备的技能或条件

* Markdown 的编写
* Git 的基本使用
* Github 网站的操作以及账号
* Vercel 网站的操作以及账号

### 所需安装的工具

* [Git](https://git-scm.com/book/zh/v2/%E8%B5%B7%E6%AD%A5-%E5%AE%89%E8%A3%85-Git) - 用于提交代码至 Github
* [Visual Studio Code](https://code.visualstudio.com/Download)（下文简称 VSCode） - 是一款备受好评的编辑器，同时也方便进行文件的管理
* [Node.js](https://nodejs.org/zh-cn) - 是 Hexo 框架所依附的平台

## 正式开始之前可能会遇到的问题

*为节约时间，本文暂时不展开进行相关软件的使用教学，对于新手们可能遇到的部分问题将列在下文(部分官方教程已用超链接绑定，可直接进行跳转学习)，请读者自行使用搜索引擎进行学习，也欢迎各位在评论区友善地进行分享与讨论。*

* [ ] [Github 账户以及 SSH 公钥的配置](https://git-scm.com/book/zh/v2/GitHub-%E8%B4%A6%E6%88%B7%E7%9A%84%E5%88%9B%E5%BB%BA%E5%92%8C%E9%85%8D%E7%BD%AE)
* [ ] VSCode 软件的语言切换
* [ ] VSCode 对 Markdown 文本的支持
* [ ] 系统环境变量的配置

## 那我们正式开始吧

*如果字段具有超链接，不妨点击跳转查看，因为此字段已经存在详细的官方教程，便没有必要赘述，也可将本文当作资讯的总结以及中继站点。*

### 一、先让Hexo站点在本地运行起来吧

1. [Hexo 的安装](https://hexo.io/zh-cn/docs/)

2. [Hexo 站点的初始化](https://hexo.io/zh-cn/docs/setup)

3. [Hexo 站点的基本配置](https://hexo.io/zh-cn/docs/configuration)

### 二、挑选一个自己喜欢的主题使用吧

1. [挑选 Hexo 主题](https://hexo.io/themes/)
2. [修改本地博客的主题](https://hexo.io/zh-cn/docs/themes) - 这里建议使用Git克隆方法安装新主题至本地博客项目中的themes文件夹，而不是npm安装方法，因为我们后期并不会打算将node_modules文件夹(npm安装方法的目标文件夹)上传至Github
3. 根据主题设计者的文档，配置主题并在本地测试

### 三、把个人博客上传并展示给朋友们吧

1. [在 GitHub 新建一个仓库](https://docs.github.com/zh/repositories/creating-and-managing-repositories/creating-a-new-repository) - 用于接收下一步所要提交的本地博客项目文件
顺便一提，新建仓库时你可以根据个人喜好来决定是否将仓库设为公开，这并不影响后续的部署。
2. [将本地项目文件夹初始化仓库](https://git-scm.com/book/zh/v2/Git-%E5%9F%BA%E7%A1%80-%E8%8E%B7%E5%8F%96-Git-%E4%BB%93%E5%BA%93)
如果你根据超链接所指向的参考文章中的步骤执行完了 ```git commit``` 指令，那你接下来只需在 VSCode 终端执行 ```git push``` 将你的个人博客推送到 Github 仓库即可。
3. 在 Vercel 控制台新建 hexo 项目并绑定先前所创建的 Github 仓库

---

（本文目前为简略版，详细内容待补充…）
