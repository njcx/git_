#### git简明教程_by nJcx

- 介绍

git是 Linus，也就是Linux kernel 的作者所写的分布式版本控制系统。下面介绍一下git是怎么使用的：

先安装git
```bash
sudo apt-get install git git-core

```
我们先建个目录，并且在目录里面初始化git所需的相关文件，里面会有一个.git 的隐藏文件夹
```bash

> mkdir git 
>cd git && git init
>echo "# git_" >> README.md

```
我们在里面加了一个README.md文件

```bash

> git add . && git commit -m "add more" && git push -u origin master

//第一步,用命令 git add 告诉Git,把文件添加到仓库
//用命令 git commit （-m 就是加注释的意思）告诉Git,把文件提交到仓库:
//第三步，把本地文件变动提交远程仓库
```
查看本地是否有变动或者状态
```bash
>git status

```
查看差异或者修改的内容
```bash
>git diff
```
查看提交的tag

```bash

>git log

```


 