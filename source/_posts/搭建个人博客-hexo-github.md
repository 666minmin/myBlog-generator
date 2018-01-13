---
title: 搭建个人博客-hexo+github
date: 2018-01-13 13:24:24
tags:
---

如何用hexo创建博客网站
1、全局安装hexo:npm install -g hexo
2、创建文件目录（当前路径在桌面） mkdir myBlog
3、cd myBlog
4、hexo init
5、start _config.yml（设置author，title）
6、hexo generate
7、hexo serve
8、http://localhost:4000/

如何用hexo写文章
1、hexo new "搭建个人博客-hexo+github" 
2、start "搭建个人博客-hexo+github".md （编辑文章具体内容）
3、hexo generate
4、hexo serve
5、http://localhost:4000/

如何用hexo修改网站主题：
1、选择中意的主题：https://hexo.io/themes/
2、下载主题（eg）：cd themes;git clone git@github.com:iissnan/hexo-theme-next.git 
3、start _config.yml（设置theme）
4、hexo generate
5、hexo serve
6、http://localhost:4000/ 

hexo生成博客网站如何部署到github上面
1、在gitub上面创建空的仓库
2、安装git部署插件：npm install hexo-deployer-git --save
3、安装项目相关依赖：npm i
4、start _config.yml（设置type,repo）
5、hexo clean
6、hexo generate
7、hexo deploy

网站源码如何部署到github上面
1、在github上面创建空的仓库
2、在网站源目录
echo "# yyyy" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:666minmin/yyyy.git
git push -u origin master
3、git add .
4、git commit  -m "提交信息"
5、git push origin master