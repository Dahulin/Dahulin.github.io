---  
layout: article  
title:  "怎样利用github与jekyll搭建博客"  
date:   2018-01-03 20:00:00 +0800  
categories: posts rwd
image:
  feature: GitHub.png
  teaser: GitHub.png
---  

## 怎样利用github与jekyll搭建博客
1. 注册一个github的账号和下载github。 desktop（如已经有github账户可忽略此步骤）
2. 在github中建立一个基于你的用户名的repository: 比如说我，就要建立名为dahulin.github.io的repo。
3. 下载ruby（需要ruby来使用本地jekyll）最简单的方法是直接将集成好的Ruby installer来进行安装。
4. 安装RubyGems，gem是一个ruby的包管理系统，可以用gem很方便的在本地安装ruby应用。
- gem安装方法很简单

```
//在RubyGems官网上下载压缩包，解压到你的本地任意位置
//在Terminal中
cd yourpath to RubyGems //你解压的位置
ruby setup.rb
```
- 有了gem，安装jekyll就很简单了，直接在Terminal里面输入以下代码：

```
$ gem install jekyll 
```
5. 到这一步简单博客框架已经搭建好，你可以选择去寻找合适的模板fork过来慢慢修改，也可以自己慢慢一步步美化和增添内容。
6. 然后你可以开始写自己的文章，所有的文章直接放在_posts文件夹下面，格式就是我们之前提到的markdown文件，默认的格式是.md和.markdown文件。每篇文章的开始处需要使用yml格式来写明这篇文章的简单介绍，格式如下：

```
---  
layout: article  
title:  "RWD2 学习笔记"  
date:   2018-01-03 20:00:00 +0800  
categories: posts rwd
image:
  feature: 网页笔记.png
  teaser: 网页笔记.png
---  
```
- layout就是article，让jekyll知道你这是一篇article，很直观。需要注意的是里面的date，必须按照yml的语法来写，否则就会出现编译错误。
7. 以上是我参考网上一些教程结合自己操作尝试得出的一些学习笔记。