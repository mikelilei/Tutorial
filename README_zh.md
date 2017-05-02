欢迎使用 Git Drive
=================================
Git Drive是一款专为iOS系统设计的，可以在移动设备上运行的Git版本控制软件，通过它可以将您手中已有的iOS设备变成一个功能完善的Git版本控制服务器，只需要从苹果应用商店下载安装即可，无需繁琐的安装步骤，也无需其它任何操作，1分钟之内就可以搭建好一个Git版本控制服务器。它完整的实现了Git Smart传输协议，传输稳定快速，并提供基于仓库的授权访问控制，支持对仓库进行shallow更新和下载操作。

基于Git分布式的架构，单点的损坏不会导致整个系统的瘫痪，所以Git Drive很适合作为Git存储网络中的一个节点，并且这个节点可以随身携带。

Git Drive除了是一款功能完整的Git版本控制服务器软件外，它还提供强大的Git客户端功能，使您能够在应用内直接对仓库进行进行管理，对文件进行查看。

和传统的代码托管模式不一样的是，通过使用Git Drive您的代码被存储在您自己的设备上，如果您同样使用iCloud，那么所有的仓库将会被同步到所有的设备上，通过这种模式可以使您充分利用iPhone或者iPad上的闲置空间来存放一些重要数据，对于一个小型的团队，也可以很方便以此来交换数据，同时也节省了自己搭建Git版本控制服务器的成本和时间。

## 快速开始
#### Git教程
如果您对Git本身还不太熟悉的话，这里有一个在线的Git教程，可以帮助您快速熟悉，并开始使用Git。
[一个非常棒的Git在线教程](https://git-scm.com/book/zh/v2)
#### 如何将已有的本地仓库上传到Git Drive
- 确保您的设备和PC已经连接到同一个WiFi。
- 打开Git Drive，并确保Git服务器处于开启状态，检查服务器开关为蓝色则为开启状态 ***（侧栏菜单 --> 服务器开关）***。
- 打开Git Drive Finder，让Finder为您在本地添加Git Drive域名映射。
- 在Git Grive上新建一个仓库 ***（左菜单 --> 所有仓库 --> 新建仓库）***，输入 ***myrepo*** 后点击***完成***。
- 在进入本地Git仓库后，输入下面的命令完成Git远程仓库的添加

```
git remote add myrepo http://gitdrive.com/myrepo
```
- 输入如下的命令将本地仓库Push到Git Drive

```
git push myrepo refs/heads/*:refs/heads/*
```

#### 如何将Git Drive上的仓库下载到本地

- 确保您的设备和PC已经连接到同一个WiFi。
- 打开Git Drive，并确保Git服务器处于开启状态，检查服务器开关为蓝色则为开启状态 ***（侧栏菜单 --> 服务器开关）***。
- 打开Git Drive Finder，让Finder为您在本地添加Git Drive域名映射。
- 在本地输入下面的命令来创建一个新仓库。

```
git clone http://gitdrive.com/your_repo_name
```
- 或者输入下面的命令来创建一个shallow的仓库

```
git clone —-depth=1 http://gitdrive.com/your_repo_name
```

目录
=================================
- [仓库管理](./docs/chapter_1_zh.md)
- [内容浏览](./docs/chapter_2_zh.md)
- [版本提交历史](./docs/chapter_3_zh.md)
- [Git服务器管理](./docs/chapter_4_zh.md)

