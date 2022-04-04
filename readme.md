# push file to the remote repository

自己使用创建 git 仓库:过程是：选择要push的本地项目根目录

1. git init //初始化项目，执行完此命令后会生成一个.git文件夹
2. git add . //将本地项目所有文件添加到git管理，.指全部文件
3. git commit -m “提交描述信息"
4. git remote add origin 刚刚新建的Github地址 //将本地项目与远程git仓库关联
5. git push -u origin master /git push -f origin master，-f 强制将本地项目push到远程仓库

---
```
git init
git add README.md
git commit -m "first commit"
git remote add origin ***
git push -u origin main
git push -u origin master
```

**git remote add** 如果出现这样的问题，**fatal: remote origin already exists.**<br>
解决方案是移除: ```$ git remote rm origin ```