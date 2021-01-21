---
title: Git 命令学习笔记

tags: ['Git', '命令']
---

在我接触到Hexo的博客中，我也认识到了Git的强大。~~特别是可以用Git来偷老师课件~~

# 下载及安装Git

由于我主要是使用Windows作为开发环境，因此我是以Git for Windows来作为素材

下载地址：[http://git-scm.com/](http://git-scm.com/)

安装一路无脑下一步即可，注意选择编辑器最好选择常用的编辑器

安装完成，随意右键，见到“Git GUI here”和“Git bash here”就成功了

![](https://cdn.jsdelivr.net/gh/zzysite/imgs@main/20210122020727.png)

# 从Github克隆项目至本地

打开接收克隆的文件夹，右键打开Git bash，执行以下命令

```shell
git clone 仓库地址
```

如需要克隆到指定目录，可以使用

```shell
git clone 仓库地址 本地路径
```

# 同步项目到Github

打开本地的项目文件夹，右键打开Git bash。