#### git简明教程_by nJcx

- 介绍

git是 Linus，也就是Linux kernel 的作者所写的分布式版本控制系统。下面介绍一下git是怎么使用的：

先安装git
```bash
sudo apt-get install git git-core

```
我们先建个目录，并且在目录里面初始化git所需的相关文件，里面会有一个.git 的隐藏文件夹,
```bash
├── branches
├── COMMIT_EDITMSG
├── config
├── description
├── HEAD
├── hooks
│   ├── applypatch-msg.sample
│   ├── commit-msg.sample
│   ├── post-update.sample
│   ├── pre-applypatch.sample
│   ├── pre-commit.sample
│   ├── prepare-commit-msg.sample
│   ├── pre-push.sample
│   ├── pre-rebase.sample
│   └── update.sample
├── index
├── info
│   └── exclude
├── logs
│   ├── HEAD
│   └── refs
│       ├── heads
│       │   └── master
│       └── remotes
│           └── origin
│               └── master
├── objects
│   ├── 08
│   │   └── 2f946ba92b4925b01822045fa0d9e6ba159722
│   ├── 40
│   │   └── 6974cab3b2348fddf476fa5d3c01d3e2cdf2d9
│   ├── 4b
│   │   └── 825dc642cb6eb9a060e54bf8d69288fbee4904
│   ├── 5b
│   │   └── 42df0cfd1b5d6cdfc7d5b251ea770ca35cbec1
│   ├── 6a
│   │   └── 9a26c9a383223ee73a2c4d26e9320dad2dab65
│   ├── d1
│   │   └── 71df385fb3af5b092c65bfea5011316de936d0
│   ├── ee
│   │   └── 30a2259699e8d4e534799576fa9ab38b865b90
│   ├── info
│   └── pack
└── refs
    ├── heads
    │   └── master
    ├── remotes
    │   └── origin
    │       └── master
    └── tags

```
```bash

> mkdir git 
>cd git && git init
>echo "# git_" >> README.md

```
 