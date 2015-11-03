Git is a distributed version control system.
Git is free software.


创建版本库
$ mkdir learngit
$ cd learngit
$ git init
$ git add readme.txt
$ git commit -m "wrote a readme file"

版本管理
$ git status
$ git diff readme.txt 
$ git log --pretty=oneline
$ git reset --hard HEAD^
$ git reset --hard 3628164
$ git reflog