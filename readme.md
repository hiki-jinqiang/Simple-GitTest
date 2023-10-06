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





git ls-tree -r <branch-name>

 在这个命令中，`` 是您要查看的分支的名称。这个命令将列出指定分支下的所有文件和它们的详细信息，包括文件的类型（blob）、文件的SHA-1哈希值、文件的大小以及文件的路径 ----just a test

git merge  //别的分支合并到当前的分支上。









 

