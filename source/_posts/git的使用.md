---
title: git的使用
date: 2018-01-13 13:47:51
tags:
---

git的使用
一、配置gitHub-添加SSH key
1、一台电脑对应一个SSH key
2、一个SSH key可以访问你所有的仓库

二、配置git
git config --global user.name 你的英文名
git config --global user.email 你的邮箱
git config --global push.default matching
git config --global core.quotepath false
git config --global core.editor "vim"

三、使用git

1、本地创建仓库
创建本地目录结构，在本地目录里面：
git init //初始化本地仓库
git status -sb //显示当前所有文件的状态A\M\D
git add 文件路径 //用来将变动加到暂存区
git add .//目录的所有变动加到暂存区
git commit 文件路径 -m "信息" //用来正式提交变动，提交至.git仓库
git commit . -m "信息"
git log //查看变更历史
如果远程被修改，先pull,再push

2、将本地仓库上传到GitHub
git remote add origin git@github.com:xxxxxx/git-demo-1.git
git push -u origin master

3、下载GitHub上的仓库到本地
git clone git@github.com.xxx
