# git使用在实际开发中-指令版本



讲解视频： [Git工作流和核心原理 | GitHub基本操作 | VS Code里使用Git和关联GitHub_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1r3411F7kn/?spm_id_from=333.1007.top_right_bar_window_default_collection.content.click&vd_source=d6cbfce424d90414a859cc5aee71d89e) 

概论：

![](E:/3-GitTest/picture/Snipaste_2023-10-06_21-17-33.png)

**git配置基本信息：**

git config --global user.name "global"

git config --global user.email

git config --global --list



**git常用命令：**

git init

git status

git add txt,md

 git commit -m "first commit"

git commit -a -m "first commit"   //提交

git log

git ls-tree newbranch <filename>

ls

cd

touch .gitignore



**git 分支相关命令：**

git branch newbranch  //创建指令

git branch                       //查看branch

git branch -r                   //查看远程仓库分支

git checkout  newbranch  //切换分支

git branch -d newbranch  //删除分支

git branch -D newbranch //直接删除分支

git checkout -b temp         //创建分支并切换

git merge newbranch  //在当前分支下合并newbranch分支。



git ls-tree -r <branch-name>    //查看分支 ，在这个命令中，`` 是您要查看的分支的名称。这个命令将列出指定分支下的所有文件和它们的详细信息，包括文件的类型（blob）、文件的SHA-1哈希值、文件的大小以及文件的路径 



**git远程仓库：**

git remote -v                                         //查看远程仓库

git remote add origin https:....... //添加远程创库

git remote set-url origin  newhttps：.....   //修改origin的url

git remote remove origin                 //删除origin

git push origin --delete <branch-name>      //远程删除分支，需要权限



git push         //在有上游分支设定情况可直接上传

git push -u origin newbranch             // 这将推送当前分支 `newbranch` 到远程仓库 `origin` 并将其设置为上游分        支。一旦设置了上游分支，您就可以使用 `git push` 和 `git pull` 命令，而不必再指定远程分支的名称。 

git push origin newbranch          // 这将只推送当前分支，但不会将其与远程分支关联起来 

git push origin --delete  branch      //删除远程仓库的branch



git clone git@github.com:hiki-jinqiang/Simple-GitTest.git      //下载远程仓库

git clone -b my-feature git@github.com:hiki-jinqiang/Simple-GitTest.git   //下载指定的分支的仓库

git pull         //

git fetch origin branch      //拉取远程仓库分支到本地仓库

git fetch origin feature-branch:my-feature  // 例如，假设您要从远程仓库 `origin` 拉取名为 `feature-branch`    的分支到本地并将其命名为 `my-feature` 

git merge origin/my-feature  // 如果您想将远程分支的更新合并到您的本地分支，可以使用 `git merge` 



git diff origin/main     // 比较



**git special operation**

git checkout .  // 在Git中，要将本地仓库的更改更新到工作区 

git checkout -- filename      // 要将本地仓库的更改更新到工作区 ，新的文件或目录的路径 





















