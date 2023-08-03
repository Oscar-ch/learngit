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
   ```

## 分支管理

1. 什么是分支？
2. 如何创建分支？

   Key:git checkout -b dev或者 git switch -c dev, git branch

3. 如何切换分支？

   Key:git switch master

4. 如何合并和删除分支？

   Key:git merge dev,git branch -d dev

5. 如何在保留分支情况下合并？

   Key:git merge --no-ff -m"merge without ff" dev

6. 如何对远程库版本回退？

   Key:git push -f origin master

## BUG分支

1. 当前dev分支暂时无法提交，但是需要立即在master分支上修复bug，应该怎么办？

   Key:

   ```git

   git stash
   git switch master
   git switch -c issue-101
   ........
   git switch master
   git merge --no-ff -m "merged bug fix 101" issue-101
   git stash list

   git stash aplly(删除stash中的内容需要 git stash drop)
   或者
   git stash pop(自动删除)

   ```
