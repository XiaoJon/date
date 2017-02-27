# date
资料的收集和总结


Git命令
关联远程库：git remote add origin git@server-name:path/repo-name.git
推送最新修改：git push -u origin master  -u推送所有
更新服务器：git pull origin master
克隆：git clone git@serverName:path/repo-name.git
查看远程仓库：git remote -v
删除远程仓库：git remote rm origin

初始化仓库：git init
查看状态：git status
查看修改内容：git diff
查看提交历史：git log   --pretty=oneline参数可以查看commit_id
查看命令历史：git reflog
选择版本：git reset --hard commit_id     HEAD表示^上一版本
覆盖暂存区：git reset HEAD file
覆盖工作区的file：git checkout -- file
添加到暂存区：git add file
删除暂存区：git rm file
提交到版本库：git commit -m "xxx"

查看分支：git branch
创建分支：git branch <name>
切换分支：git checkout <name>
创建+切换分支：git checkout -b <name>
合并某分支到当前分支：git merge <name>      rebase 也可以
删除分支：git branch -d <name>

将改动暂存：git stash
查看暂存区：git stash list
恢复暂存区：git stash apply
删除最近一条stash：git stash drop
恢复并删除一条stash：git stash drop
清除stash：git stash clear
