---
layout: post
title: "我的wordpress 下载插件改动"
date: 2013-02-01 11:24
categories: wordpess
---
最近折腾一个下载站很长时间了，这段时间比较懒散 偶尔才会抽点时间来做 下载原本打算用 [帝国CMS](http://www.phome.net/) 但又想要wordpress 那样强的TAG 功能 所以最后还是选择了用wordpress

网站很多说法，WORDPESS不合适做大一点的网站 因为性能问题 我看了异次元的站点 负载各方面都可以，于是想用它试试

推荐位方面，用的一个叫 [meta-box](http://wordpress.org/extend/plugins/meta-box/) 的插件 可以在文章发布页 定义 各种meta 这样就可以完全满足下载的并不多的推荐位

下载嘛！ 看想搞成 [异次元](http://www.iplaysoft.com/) 那样跳转到独立的[下载页](http://dl.iplaysoft.com/files/2097.html)

在网上找了很久的插件也试了很多，比如 [wp-downloadmanager](http://wordpress.org/extend/plugins/wp-downloadmanager/) [WordPress Download Monitor](http://wordpress.org/extend/plugins/download-monitor/) 这两个都有独立下载表的插件最后感觉到不尽人意后来看了一下 [Hacklog](http://ihacklog.com) 修改的 downloadmanager 不错有点接近下载页，用自己这点PHP毛皮修改了很多查阅了不少文档 才改出个差不多了。