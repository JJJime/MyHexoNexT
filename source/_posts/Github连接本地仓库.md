---
title: Github连接本地仓库
copyright: right
date: 2021-09-30 00:20:22
tags: Github
---

##  如题



以下所有的设置都只是为了从本地仓库上载到自己的Github仓库而非clone，因为hexo博客的特点就是在本地创建库，生成相应的文件后使用命令`hexo d`上载到自己的博客仓库，因此连接自己的GitHub仓库是必不可少的步骤，否则只能localhost看看了，其他人无法访问的。

### 正文开始

-----



在终端中运行以下命令（这是四条命令的组合命令，请将所有的Mail与UserName改成自己的用户名和ID）：

{% note default %}

git config --global user.name "username"  &&  git config --global user.email "email@gmail.com" &&  ssh-keygen -t rsa -C "email@gmail.com" && cat ~/.ssh/id_rsa.pub

{% endnote %}

执行过后会输出自己的 {% label info@Key值 %} ，然后打开Github-点击右上角头像-设置

![](https://i.loli.net/2021/09/30/B4GNzqDkYxCaZEh.png)

选择 SSH & GPG Keys

![](https://i.loli.net/2021/09/30/Cm1QlABhTdfp4H9.png)

点击右上角的New SSH KEY 将自己一开始获取的 {% label info@Key值 %} 复制进去就好了，记得提交哦～

![](https://i.loli.net/2021/09/30/rE4gb7aCS8Rqoec.png)



嗯结束了，结束的有些突然，但是还是结束了
