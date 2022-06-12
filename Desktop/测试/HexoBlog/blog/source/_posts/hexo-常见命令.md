---
title: hexo 常见命令
date: 2022-06-04 19:56:31
tags: 博客 资料
---
**hexo clean**
> 清除缓存文件 db.json 和已生成的静态文件 public  <!--more-->

	网站显示异常时可以执行这条命令试试。
**hexo g**或**hexo generate**
> 生成网站静态文件到默认设置的 `public` 文件夹   

	便于查看网站生成的静态文件或者手动部署网站；
	如果使用自动部署，不需要先执行该命令；
	hexo g 是 hexo generate 的缩写，命令效果一致。
**hexo s**或**hexo server**
> 启动本地服务器，用于预览主题。默认地址：[http://localhost:4000/](http://localhost:4000/),4000端口  

	hexo s 是 hexo server 的缩写，命令效果一致；
	预览的同时可以修改文章内容或主题代码，保存后刷新页面即可；
	对 Hexo 根目录 _config.yml 的修改，需要重启本地服务器后才能预览效果。
**hexo d**或**hexo deploy**
> 自动生成网站静态文件，在本地生成.deploye_git文件夹，并将编译后的文件上转到GitHub上

	hexo d 是 hexo deploy 的缩写，命令效果一致。
**hexo n**或**hexo new**  
例如：hexo n "我的第一篇博客文章"，会生成标题为`我的第一篇博客文章`的文章
> 新建博客文章，如果标题有空格，则加上引号
	
	文章标题可以在对应 md 文件里改，新建时标题可以写的简单些；
	hexo n 是 hexo new 的缩写，命令效果一致。 

**hexo new [layout] <title>** 
> 可以在命令中指定文章的布局（layout），不指定默认为 `post`，也可以通过修改` _config.yml` 中的 `default_layout `参数来指定默认布局。创建的新文章会自动加上指定布局对应的模板文件中的内容。

[hexo新手教程](https://zhuanlan.zhihu.com/p/85037427)