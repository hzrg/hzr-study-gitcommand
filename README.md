# hzr-study-gitcommand
一、

1、git init
在当前项目的目录中生成本地的git管理（会发现在当前目录下多了一个.git文件夹）
2、git add .
将项目上所有的文件添加到仓库中，如果想添加某个特定的文件，只需把.换成这个特定的文件名即可。尤其注意 add后面. 要有一个空格
3、git commit -m "first commit"
表示你对这次提交的注释，双引号里面的内容可以根据个人的需要改。
4、git remote add origin https://自己的仓库url地址
将本地的仓库关联到github上
5、git push -u origin master
把代码上传到github仓库的
6、git branch -a
查看所有分支
7、git branch
查看当前使用分支（结果列表中前面标*号的表示当前使用分支）
8、git checkout 分支名
切换分支

二、更新github仓库
1、git status //查看仓库状态
2、git add * //用于更新所有代码
3、git commit -m "" //提交的备注
4、git push origin master //将本地仓库的代码更新到github的仓库
5、git pull //拉取当前分支的最新代码

三、解决问题
1、
