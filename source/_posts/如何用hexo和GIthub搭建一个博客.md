---
title: 如何用hexo和GIthub搭建一个博客
date: 2017-11-24 00:57:01
tags:
---
### 第一步
在 GitHub 上新建一个空 repo，repo 名称是「你的用户名.github.io」（请将你的用户名替换成真正的用户名）注意，这里是用户名，不能随便取个名字。我的用户名是lapland917 例：lapland917.github.io.
### 第二步
建立一个安全文档。启动git bash 进入文档后输入一下代码

```
npm install -g hexo-cli
```
用来安装Hexo

```
hexo init myBlog
```
在目标文件下，建立myBlog的文件夹

```
cd myBlog
```
进入文件夹

```
npm i
```
```
hexo new 开博大吉 
```
你会看到一个 md 文件的路径，编辑这个.md 文件，内容自己想

```
start _config.yml
```
用编辑器配置它

把第 6 行的 title 改成你想要的名字

把第 9 行的 author 改成你的大名

把最后一行的 type 改成 type: git

在最后一行，与 type 平齐，另起一行 repo: 仓库地址 （请将仓库地址改为「你的用户名.github.io」对应的仓库地址，

```
npm install hexo-deployer-git --save
```
安装 git 部署插件

```
hexo deploy
```
这步完了以后，刷新「你的用户名.github.io」对应的 repo ，开 GitHub Pages 功能，如果已经打开了，就直接点击预览链接，博客就搭建完成了。

完


第二次上传博客，只需要输入下面的代码就行了

1 博客的名称 
```
hexo new <flie>
```


2 然后编辑makedown文件

3 
```
hexo generate
```

4
```
hexo deploy
```
