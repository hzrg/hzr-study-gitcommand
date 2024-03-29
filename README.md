![](https://github.com/hzrg/hzr-study-gitcommand/blob/master/images/git.png)
# hzr-study-gitcommand
## git常用命令
1. git init
在当前项目的目录中生成本地的git管理（会发现在当前目录下多了一个.git文件夹）
2. git add .
将项目上所有的文件添加到仓库中，如果想添加某个特定的文件，只需把.换成这个特定的文件名即可。尤其注意 add后面. 要有一个空格
3. git commit -m "first commit"
表示你对这次提交的注释，双引号里面的内容可以根据个人的需要改。
4. git remote add origin https://自己的仓库url地址
将本地的仓库关联到github上
5. git push -u origin master
把代码上传到github仓库的
6. git branch -a
查看所有分支
7. git branch
查看当前使用分支（结果列表中前面标*号的表示当前使用分支）
8. git checkout 分支名
**切换分支**
9. 更新远程分支列表
git remote update origin --prune
10. 删除远程分支Chapater6
git push origin --delete Chapater6
11. 删除本地分支 Chapater6
git branch -d  Chapater6
12. 把当前工作现场“储藏”起来，等以后恢复现场后继续工作
git stash
13. 合并分支
git merge -m "merged buf fix 101" issue-101
14. 删除分支
git branch -d issue-101
15. 查看保存的工作
git stash list
16. 恢复存储的内容
git stash apply    git stash drop
git stash pop
17. 创建并切换分支
git checkout -b 分支名

## 更新github仓库
1. git status //查看仓库状态
2. git add * //用于更新所有代码
3. git commit -m "" //提交的备注
4. git push origin master //将本地仓库的代码更新到github的仓库
5. git pull //拉取当前分支的最新代码

## 解决问题
1. 使用git push -u origin master把代码上传到github仓库时：error:failed to push some refs to 'xxx'
解决方法：
git pull --rebase origin master
git rebase --continue
git add .idea/workspace.xml
git rebase --continue
git push -u origin master
即：先pull后push
2. git老是提交.idea/workspace.xml,临时删除命令：
git rm --cached -r -f .idea
git commit -m 'delete .idea'

