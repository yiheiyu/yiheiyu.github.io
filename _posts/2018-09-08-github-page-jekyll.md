---
layout: post
title: 使用Jekyll&Github Page搭建自己的个人博客
categories: Jekyll
description: 使用Jekyll&Github Page搭建自己的个人博客
keywords: Jekyll,GithubPage
---
Github Pages 是在Github上托管的静态网页。从2016年6月15日开始，通过域名github.io访问使用的是https协议。Github Pages的代码仓库容量限定是1G,并且带宽限制是100G或者每月10万次访问。
jekyll是一个简单的免费的Blog生成工具，类似WordPress。但是和WordPress又有很大的不同，原因是jekyll只是一个生成静态网页的工具，不需要数据库支持。但是可以配合第三方服务,例如Disqus。最关键的是jekyll可以免费部署在Github上，而且可以绑定自己的域名。

**目录**

* TOC
{:toc}

## 安装配置Jekyll
Jekyll只是一个静态网页的生成工具，想必你有过一定的了解，在这里不过多介绍。
Jekyll的官网地址：[Jekyll - 简单静态博客网站生成器][1]
步骤：
1. 安装Ruby.
2. 安装Devkit.
3. 安装Jekyll.

### 安装Ruby
> Ruby官方下载地址：[Downloads][2]

![](/images/posts/jekyll/ruby_download.png)

找对应自己系统的版本下载即可。
安装完成之后输入
> ruby -v
测试是否安装成功

```Shell
C:\Users\zhao>ruby -v
ruby 2.4.4p296 (2018-03-28 revision 63013) [x64-mingw32]
```

### 安装DevKit
因为我下载的是Ruby+Devkit 2.4.4-2 (x64) ，附带着就把DevKit也安装了，不过多解释，直接安装就好。
> Ruby官方下载地址：[Downloads][2]

![](/images/posts/jekyll/devkit-download.png)

### 安装Jekyll
Ruby+Devkit 安装完之后开始安装Jekyll
> gem install jekyll

```Shell
C:\Users\zhao>gem install jekyll
Fetching: public_suffix-3.0.3.gem (100%)
Successfully installed public_suffix-3.0.3
Fetching: addressable-2.5.2.gem (100%)
Successfully installed addressable-2.5.2
Fetching: colorator-1.1.0.gem (100%)
Successfully installed colorator-1.1.0
Fetching: http_parser.rb-0.6.0.gem (100%)
Temporarily enhancing PATH for MSYS/MINGW...
Building native extensions.  This could take a while...
Successfully installed http_parser.rb-0.6.0
......
```

安装完之后测试一下
> jekyll --version

```Shell
C:\Users\zhao>jekyll --version
jekyll 3.8.3
```

没有问题

### 新建博客
都配置好之后输入以下命令新建一个Jekyll本地静态博客
> jekyll new myblog

![](/images/posts/jekyll/jekyll-new-myblog.png)

如果没有报错，会在当前目录下生成一个myblog的文件夹
![](/images/posts/jekyll/myblog.png)

本地博客就建好了

### 运行本地博客
博客文件生成之后，在myblog目录下，输入以下命令运行服务器：
> jekyll serve

![](/images/posts/jekyll/jekyll-serve.png)

在浏览器中访问：`http://127.0.0.1:4000/`

![](/images/posts/jekyll/success.png)


没有问题

## GitHub Page
Github Pages 是在Github上托管的静态网页。通过域名`xxx.github.io`来访问。

### 创建一个GitHub账户
创建GitHub账户不过多解释。

### 新建一个repository
例如你的GitHub名称是yiheiyu，就创建一个名为yiheiyu.github.io的repository。
![](/images/posts/jekyll/github-repository.png)




[1]: http://jekyllcn.com/
[2]: https://rubyinstaller.org/downloads/
