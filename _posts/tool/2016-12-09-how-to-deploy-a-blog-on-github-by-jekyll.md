---
layout: post
title: 在Github上搭建自己的jekyll博客
tag: 工具
keyword: 'Jekyll, Github'
description: null
published: true
---

> 本文主要是根据yansu的[博客][1]及github上的[源码][2]进行建立的,为了记录搭建的过程,特此进行记录.

> 本文主要记录了我在搭建过程中的修改.

## 创建一个库
将该[库][2]fork到自己的github,并修改为`username.github.io`.

## 创建本地目录
将库clone到本地.

## 域名配置
删除`CNAME`文件,从而使用默认域名.有自己域名的,可以直接在该文件中修改为自己的域名.这里,我使用了默认的域名.

## 配置文件
修改`_config.yml`文件,将里面的变量全部修改为自己的.

这里主要讲一下blog中头像的设置.首先将自己的头像上传到自己的github中,然后点击图像打开,复制浏览器中url到`_config.yml`的avatar变量中.
下面设置ico图标,可以在[网站][3]中,上传自己的头像在线生成;然后选择合适尺寸的图标下载到本地;最后,按照上述方法,获取url并赋值给`favicon`变量.

## 博客文件
`_posts`目录保存了所有博客,会被jekyll处理成静态的html文件.

删除该目录下的所有文件,并按照自己的喜好建立新的文件夹,可以方便管理自己的博客.

> 另外,在`_posts`下符合`YYYY-MM-DD-xxxxxx.md`的文件,都会被jekyll认定为博客内容.因此写博客时要注意保存的文件名.



[1]: http://yansu.org/
[2]: https://github.com/suyan/suyan.github.io
[3]: http://www.ico.la/
