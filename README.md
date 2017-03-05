hexo-new-vno
========

这个主题是原创为[onevat的vno](https://github.com/onevcat/vno), 它遵从简洁和响应式的设计风格，拥有一个独立的封面，易于集成的 Disqus 评论和多说系统，Google Analytics,字体图标以及多种颜色。
此主题的hexo版本由[空谷幽兰](//mlongbo.com/)最先创建,但是已不维护
我加了一些功能及对bug的修复，所以重新创建一个,[github地址](https://github.com/monniya/hexo-theme-new-vno.git)

## Demo Show

[Demo: 我的博客](https://monniya.com)

![主页封面](source/images/show/home.png)

![文章列表](source/images/show/list.jpeg)

## 封面

### 图片和颜色

将您的封面图片放到主题的 source/images/ 下，将图片文件改名为background-cover.jpg或修改_config.iml中background的cover字段值即可。您也可以改变封面的颜色。找到_config.iml中background的color字段值,然后替换成您需要的颜色即可。默认为您提供了七种选择：

* `cover-blue` - #2568A3
* `cover-green` - #156F78
* `cover-purple` - #493252
* `cover-red` - #E25440
* `cover-orange` - #FB9C50
* `cover-slate` - #3D4260
* `cover-disabled` - 透明

### 头像和简介

头像可以在封面中显示,将头像文件放到全局的 source/images/下, 修改_config.yml中的logo字段值即可。

您还可以在封面页上写一个简短的介绍, 填写全局的_config.yml(注意:不是主题下的_config.yml)中的description字段值, 支持html标签。


## Installation

### Install 安装

``` bash  
$ git clone https://github.com/monniya/hexo-theme-new-vno.git themes/new-vno
```

### Enable 主题启用设置

设置全局的<code>_config.yml</code>
theme: new-vno


## Configuration 主题设置
设置主题的配置文件：<code>_config.yml</code>

```yml
＃menu子菜单，可自定义
menu:
  #Archives: /archives
  黄金屋: /favourite
  时光机: /favourite/time.html
  #我是: /aboutme
＃rss需安装插件hexo-generator-feed，详细请看：https://monniya.com/2016/02/24/create-rss/
rss: /atom.xml
# description配置内容会出现在meta标签中，因此会被搜索引擎抓取
description: 

# 不填写的链接则不显示
social:
  weibo: https://weibo.com/monniya
  github: https://github.com/monniya
  stack_overflow: 
  facebook: 
  twitter: 
  google_plus: 

page_comment: true

# 封面中的头像
logo: /images/avatar.jpg
background:
  cover: /images/background-cover.jpg
  color: cover-purple

archive_date_format: MMM DD
fancybox: true

# 多说的帐号名, 不配置则不启用，使用disqus请去全局_config.yml中配置disqus_shortname
duoshuo_shortname: 

google_analytics: 谷歌跟踪ID
baidu_tongji: 百度统计识别码
favicon: /images/avatar-small.png
```
谷歌跟踪ID：
![谷歌统计](source/images/show/google-analytics.jpeg)
百度统计识别码：
![百度统计](source/images/show/baidu_tongji.jpeg)

### 文章

喵神没有设置categories，只用tags
例如：
```yml
---
title: 文章名称
date: 2016-03-03 10:46:46
tags: 分类
---
```
![百度统计](source/images/show/article.jpeg)

### 数学公式支持

# mathjax
mathjax: true
由于资源考虑，默认是不加载mathjax的，若需使用请在文章头部添加：
```yml
如下示例：
---
title: 侧耳倾听我的心
date: 2017-02-18 22:55:08
tags: 观观影
mathjax: true
---
```