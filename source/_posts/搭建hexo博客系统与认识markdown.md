---
title: 搭建hexo博客系统与认识markdown
date: 2016-11-02 17:42:48
tags: web
---
### 导语

> 经过一通折腾，终于搭建好了hexo博客系统，这里不详细介绍hexo的搭建方法，主要针对自己遇到的问题和Markdown的使用做一些说明。

## 一、hexo搭建总结

具体hexo搭建网上有很多，这里不细说，给大家几个推荐：

***
- [史上最详细的Hexo博客搭建图文教程](https://xuanwo.org/2015/03/26/hexo-intor/)
- [Hexo在github上构建免费的Web应用](http://blog.fens.me/hexo-blog-github/)
- [小白独立搭建博客--Github Pages和Hexo简明教程](https://my.oschina.net/ryaneLee/blog/638440)
***

我搭建的过程中主要遇到了hexo搭建好后执行hexo d报错的问题

解决方案为将_config.yml中deploy部分改为

	deploy:
		type: git
		repository: https://github.com/yyjTom/yyjTom.github.io.git 
		branch: master

我这里直接用https连接即可，只需要将type类型的github改为git即可上传。

## 二、认识Markdown

主流推荐的编辑器为：

***
- Windows: MarkdownPad
- Linux: ReText
- Mac:Mou
- Wordpress:WordPress › Markdown for WordPress and bbPress « WordPress Plugins
***

这里我使用了MarkdownPad，先不说语法，上图吧：
![markdown截图](http://og0axgozc.bkt.clouddn.com/markdown%E6%88%AA%E5%9B%BE.png)

初级入门推荐阅读文章[认识与入门 Markdown](http://sspai.com/25137),
如果需要更深度的学习看文档吧[Markdown 语法说明(简体中文版)](http://wowubuntu.com/markdown/index.html)。