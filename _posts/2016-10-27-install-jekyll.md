---
layout: post
title:  Mint安装Jekyll

date:   2016-10-27 21:08:00 +0800
categories: document
tag: Jekyll
---

* content
{:toc}




### 1. 安装过程中出现的问题

我用的是Linux Mint 18 Sarah Cinnamon 64-bit， 在安装和运行Jekyll的时候出现几个小问题，记录一下。



要安装Jekyll，需要先装ruby：

`sudo apt-get install ruby`

会自动安装ruby2.3版本，这时gem也同时安装好了。然后安装Jekyll：

`gem install jekyll`

这时可能会出现错误，去查看log发现是缺少了stdio.h头文件：

`sudo apt-get install libc6-dev`

然后执行`gem 'github-pages'`的时候又出现了一个Error：缺少zlib.h 头文件。执行下命令可解决：

`apt-get install zlib1g-dev`

