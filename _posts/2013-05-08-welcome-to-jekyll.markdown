---
layout: post
title:  "如何使用Jekyll"
date:   2013-05-08 01:14:27
categories: jekyll update
---
#1.jekyll介绍
Jekyll是github提供的一个静态网站生成器，可以生成类blog的网站。由于是静态网站，不提供评论功能。

就是说可以直接在本地的文件中编写一个博客/网页的内容，使用文本，html，markdown都可以，然后用jekyll发布。

同时jekyll提供自带的web服务器，可以启动一个blog服务。
jekyll也是github pages的引擎， 因此jekyll生成的网站可以直接部署到github上。

#2.在mac/linux上安装jekyll:
安装
sudo gem install jekyll

如果遇到错误，先运行： sudo gem update --system

然后取到jekyll代码（需要demo site）

git clone https://github.com/mojombo/jekyll.git

cd jekyll/site

jekyll serve 

启动demo的site，可以通过http://localhost:4000访问demo site。

#3.创建jekyll site

jekyll new  myblog

cd myblog

jekyll -w serve


-w 表示watch站点的改动，自动build。

#4.增加博客/网站内容
可以按照yyyy-mm-dd-title.md的文件名在_posts目录创建markdwon格式的博客文件，文件写完后：

jekyll build

jekyll -w serve 

即可访问到新加的文件。

[jekyll-gh]: https://github.com/mojombo/jekyll
[jekyll]:    http://jekyllrb.com
