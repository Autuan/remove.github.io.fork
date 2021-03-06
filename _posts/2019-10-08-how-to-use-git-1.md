---
layout:     post
title:      Git 二三事:使用Git前需要知道的事儿
subtitle:   每位程序员都知道的一个工具
date:       2019-10-08
author:     Autuan.Yu
header-img:
catalog: true
tags:
    - Git
    - 版本控制
---

> 谁控制了过去，就等于控制了未来；谁控制着现在，就等于控制了过去

## 前言
相信每位程序员都不会对Git感到陌生,本文主要讲解关于Git的一些知识,可能有些小伙伴对Git已经了然于胸,但是,温故而知新,也是一件好事.不是吗?

## 协议
### 贡献者协议
一般来说,程序员所写的程序,版本归属于付款人或赞助人.  

但由于开源项目的无付款人和赞助人,版权会由贡献者协议划分.  

简单地来说,就是:  

>  如果你对一个开源项目提交了一个新的贡献,同时将你对这串代码的版权转让给这个项目.  

具体地细则会根据不同的协议而有不同,常见的版权协议有:  
[Google](https://cla.developers.google.com/about/google-individual), [.NET](https://cla.dotnetfoundation.org/)等  

### 分发许可
如果你自己对属于自己的项目进行了开源,就要选择一个适合的分发许可,也就是大家知道的`开源协议`

常见的开源协议有 `MIT`/`APACHE` 等,对其中各个协议有问题的小伙伴,可以参考[阮一峰的博客内容](http://www.ruanyifeng.com/blog/2011/05/how_to_choose_free_software_licenses.html)  

### 特别注意
版权只保护代码,不保护想法,所以有很多逆向工程,将项目逆向后重写了主要代码然后重新打包,就是一个新的项目了,请大家一定要注意

## 安装
关于Git的安装,网上已有许多教程,本文不再赘述  

不过请各位小伙伴注意,过老的版本,很可能功能受限

## 角色权限
作为团队合作工具,Git 自然有角色权限,如下:  

|权限名(中文)|权限名(英文)|权限|
|---|---|---|
|系统管理员|Owner|拥有所有权限|
|项目管理员|Master|无法删除项目及修改项目可视等级等|
|项目开发人员|Developer|创建非保护分支,修改代码等|
|项目测试人员|Reporter|下载项目,修改项目等|
|Guest|访客|创建issue以及留言讨论功能|

## 分支
Git 区别于其他版本控制工具的最大一个特色,就是`分支`系统了  

所谓的分支就是在当前分支上的代码基础上,作出不同的修改,然后在需要的时候,合并到项目统一分支上  

分支的使用并没有什么限制,一般地,为了更好的团队合作,会做出一些约定来规定项目参与人员使用分支

比如说Github的(分支策略)[https://github.com/git/git]

一般都会有线上环境,测试环境等分支,具体以各公司的实际要求而定
