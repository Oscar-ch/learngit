# git学习

## 什么是git?

1. git用来干什么？
2. git是如何诞生的？
   1. Key：1991，Linus，Linux，2002，bitKeeper，2005，C，两周，1月,2008
3. 集中式和分布式版本控制系统有什么区别？
   1. Key：联网

## git如何使用？

1. 如何创建版本库并上传文件？

   Key:mkdir,cd,pwd,git init,git add,git commit -m ""

2. 如何修改上传文件？

   Key:git status,git diff,git add,git commit -m ""

3. 如何版本回退
   Key:git log,git log --pretty=oneline,git reset --hard HEAD^,cat ,git reflog

4. 什么是git的工作区和暂存区?

   Key:wd,stage,repository

5. 什么是git的管理修改？

   Key:第一次修改，git add,第二次修改，git add,git commit

6. 如何撤销修改？

   Key:git status,git restore --

7. 如何删除文件？

   Key；rm,git status,git rm,git commit -m""

8. 如何创建远程库？

   Key:ssh-keygen -t rsa -C "邮箱"

9. 如何连接远程库？

   Key:

   ``` git
   git remote add origin https://github.com/Oscar-ch/learngit.git
   git push -u origin master
   ```

10. 如何从远程仓库克隆？

   Key:

   ```git
   git clone git@github.com:Oscar-ch/learnJava

## 分支管理

1. 什么是分支？
2. 如何创建分支？

   Key:git checkout -b dev或者 git switch -c dev, git branch

3. 如何切换分支？

   Key:git switch master

4. 如何合并和删除分支？

   Key:git merge dev,git branch -d dev

5. s
