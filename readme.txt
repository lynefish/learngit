Git is a distributed version control system.
Git is free software.

远程管理
ssh-keygen -t rsa -C "youremail@example.com"

创建版本库
mkdir learngit
cd learngit
git init
git add readme.txt
git rm test.txt
git commit -m "wrote a readme file"

本地版本管理
git status
git diff readme.txt 
git log --pretty=oneline
git reset --hard HEAD^
git reset --hard 3628164
git reflog
git diff HEAD -- readme.txt 
git checkout -- readme.txt//工作区回退
git reset HEAD readme.txt//暂存区回退

远程协作
git remote add origin git@github.com:michaelliao/learngit.git
git push -u origin master
由于远程库是空的，我们第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。
git push origin master
git clone git@github.com:michaelliao/gitskills.git

分支管理
查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>
