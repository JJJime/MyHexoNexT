---
title: Hexo搭建日记1-安装Hexo博客
copyright: right
date: 2021-09-29 21:59:30
tags: Hexo搭建及个性化
---





## 前言

这是我搭建的第二个Hexo博客了，第一次搭建是因为跟风，这次搭建是因为对博客园太失望了

作为一个，热爱生活的计算机小白，总会想在哪里写些东西，一开始是CSDN，后来因为cnblog可以个性化，就搬家到了cnblog，用了一段时间之后，对自己进行了灵魂双问：

{% note success  %}

好看吗？还行....好用吗？一般....

{% endnote %}

虽然我也有一个搭建在Hexo上的博客，但是安装了个主题之后也没有进行优化，大概长这个样子（忽略那些博文：我上传了进行测试的）

![](https://i.loli.net/2021/09/29/ELaAWewdhVKiM9X.png)

之前我在写博客的时候，写到了【科学上网】，然后发布失败，这也倒无所谓，我不写就行了，遵守规矩，但是但是！！终于终于！！有一次有一次！！发生了一件让我受不了的事，那就是：博客优化！

大部分服务器进行博客优化都是几分钟，博客园用了几天，这期间无法上传博客，许多博客打不开，同时还删除了一部分博客，其中包括我的数篇，如果有违规其实删掉了我没意见，但是他居然给我删掉了几篇我的Markdown笔记....我十分信任cnblog，本地都没有进行备份...而且那都是用到之后随手打开博客就能找到的东西，我受不了了....所以，就开始了Hexo之路。

在正文开始之前，推荐一个人美心善技术牛写的还详细的小姐姐的博客：[【点这里就行勒】](https://www.jmyblog.top)

-------



## 安装Hexo

<font size = 2>以下命令皆省略`sudo`如果权限不足请自行加上，如果每次都加嫌麻烦请先运行`sudo su`</font>

-----

### 本地安装hexo博客

Hexo的安装很简单，只要安装[【Nodejs】](https://nodejs.org/zh-cn/)之后，一切用指令就能完成，首先运行以下命令，安装Hexo

{% note default %}

npm install hexo-cli -g

{% endnote %}

创建一个空白文件夹，使用命令执行以下命令（二选一）

{% note default %}

hexo init

sudo hexo init filename

两者的区别在于，第一条命令直接将您的空白文件夹作为本地仓库进行clone，第二条命令会在您创建的文件夹下创建一个名为filename的文件夹后在此文件夹下clone，文件夹名称可以自行更改。

{% endnote %}

这样一来hexo文件就创建好了，然后运行以下以下两条命令，检查下依赖，防止部署后期出现问题：

{% note default %}

​	npm install

​	npm update

{% endnote %}

这样一来hexo博客便{% label success@成功创建 %}，可以在此文件夹下执行 `hexo s` 启动博客，并在浏览器中输入`localhost:4000`查看运行状态，在贴图之前，先给四条hexo常用命令：

{% note warning %}

hexo clean 清理本地生成的文件

hexo g 生成本地文件

hexo s 本地运行hexo

hexo d 上传到github仓库（ 到这里还没配置github仓库，这条命令没有用哦～ ）

{% endnote %}

看看此时的运行状态：

![](https://i.loli.net/2021/09/29/46GhdwkxrD53aKX.png)



界面确实有点简单哈～还有点丑丑的，所以才会需要配置博客主题，但是在那之前，我们先在Github上配置一下博客～

首先先在自己的[Github](https://github.com/new)上创建自己的同名仓库，明明格式为  `用户名.github.io` ，如下图所示（因为我已经创建过了所以是红色的）：

![](https://i.loli.net/2021/09/30/Yjk9sulQ7fPratc.png)





所以我们接下来就要配置博客主题啦～

我的博客使用的是NexT主题，NexT有三种风格，如下：

![](https://i.loli.net/2021/09/30/GCNgAzOErUW6qtd.png)

通过配置theme/next/_config.yml文件可以修改，如果NexT不是你的菜的话，可以[【点击这里】](https://www.jianshu.com/p/bcdbe7347c8d)看一下别人的推荐







