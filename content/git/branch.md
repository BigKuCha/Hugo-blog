---
title: "Branch"
date: 2017-07-14T15:38:24+08:00
draft: false
categories: [git]
tags: [git]
---

Git branch
   
   git branch 不带参数：列出本地已经存在的分支，并且在当前分支的前面加“*”号标记，例如：
   #git branch
* master
   newbranch

   git branch -r 列出远程分支，例如：
   #git branch -r
   m/master -> origin_apps/m1_2.3.4
   origin_apps/hardware/test
   origin_apps/m1
   origin_apps/m1_2.3.4
   origin_apps/master
<!--more-->
   git branch -a 列出本地分支和远程分支，例如：
   #git branch -a
   * master
   newbranch
   remotes/m/master -> origin_apps/m1_2.3.4
   remotes/origin_apps/hardware/test
   remotes/origin_apps/m1
   remotes/origin_apps/m1_2.3.4
   remotes/origin_apps/master

   git branch 创建一个新的本地分支，需要注意，此处只是创建分支，不进行分支切换，例如：
   #git branch newbranch2
   #git branch
   * master
   newbranch
   newbranch2
   当前的分支依然是master，不进行切换。