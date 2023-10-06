# git使用在实际开发中-指令版本



讲解视频： [Git工作流和核心原理 | GitHub基本操作 | VS Code里使用Git和关联GitHub_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1r3411F7kn/?spm_id_from=333.1007.top_right_bar_window_default_collection.content.click&vd_source=d6cbfce424d90414a859cc5aee71d89e) 

概论：

![](E:/3-GitTest/picture/Snipaste_2023-10-06_21-17-33.png)



git config --global user.name "global"

git config --global user.email

git config --global --list



git init

git status

git add txt,md

 git commit

git log

touch .gitignore



git branch newbranch

git branch

git checkout



git branch -d newbranch

git branch -D newbranch



git checkout -b temp

git commit -a -m "first commit"

 

git merge newbranch



git ls-tree -r <branch-name>

 在这个命令中，`` 是您要查看的分支的名称。这个命令将列出指定分支下的所有文件和它们的详细信息，包括文件的类型（blob）、文件的SHA-1哈希值、文件的大小以及文件的路径 ----just a test

git merge  //别的分支合并到当前的分支上。





just a test。



git push origin --delete <branch-name>

<<<<<<< HEAD

remote resonpd：

build resonpd in github

git clone git@github.com:hiki-jinqiang/Simple-GitTest.git

git remote -v

git push

git fetch origin

git diff origin/main



 git remote add <remote-name> <remote-url> 

 其中 `` 是您为远程仓库起的名称，通常为 `origin`， `` 是远程仓库的URL。例如： 





git push -u origin newbranch

 这将推送当前分支 `newbranch` 到远程仓库 `origin` 并将其设置为上游分支。一旦设置了上游分支，您就可以使用 `git push` 和 `git pull` 命令，而不必再指定远程分支的名称。 



git push origin newbranch

 这将只推送当前分支，但不会将其与远程分支关联起来。在以后的推送和拉取操作中，您需要显式指定远程分支的名称。 

=======



git push origin --delete <branch-name>

 在这个命令中，`` 是您要删除的分支的名称。例如，如果要删除名为 `my-branch` 的分支，可以运行： 

>>>>>>> master



下载分支，然后又测试。





git clone -b master <url>

cd filename

git branch

git remote -v

git push

git pull

 

