## git简明教程_by nJcx

- 介绍

git是 Linus，也就是Linux kernel 的作者所写的分布式版本控制系统。下面介绍一下git是怎么使用的：

# 1

先安装git
```bash
sudo apt-get install git git-core

```
然后我们先设置Git的user name和email：

```bash
>git config --global user.name "nJcx"
>git config --global user.email "njcx86@gmail.com"
```
然后我们再生成Git SSH Key,一直回车就行了，然后我们打开当前用户目录下即～/.ssh/id_rsa.pub这个文件，把里面的东西添加到github、码云、coding上，就可以用了

```bash
>ssh-keygen -t rsa -C “njcx86@gmail.com”
```

我们先建个目录，并且在目录里面初始化git所需的相关文件，里面会有一个.git 的隐藏文件夹
```bash

> mkdir git 
>cd git && git init
>echo "# git_" >> README.md

```
我们在里面加了一个README.md文件

```bash

> git add .
> git commit -m "add more" 
>git remote add origin git@github.com:njcx/git_.git
>git push -u origin master

//第一步,用命令 git add 告诉Git,把文件添加到仓库
//用命令 git commit （-m 就是加注释的意思）告诉Git,把文件提交到仓库:
//第三步，添加远程仓库
//第四步，把本地文件变动提交远程仓库
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
# 2

既然是版本控制系统，我们肯定可以回退到历史上某个文件状态，我们先用 git log 看一下有哪些历史commit tag

```bash
commit 5b42df0cfd1b5d6cdfc7d5b251ea770ca35cbec1
Author: nJcx <1666276469@qq.com>
Date:   Thu Jun 8 18:16:57 2017 +0800

    add more

commit d171df385fb3af5b092c65bfea5011316de936d0
Author: nJcx <1666276469@qq.com>
Date:   Thu Jun 8 17:53:49 2017 +0800

    first commit

```
就像这样



 