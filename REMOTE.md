# GitRemote
git 使用说明
# 适用场景：没有克隆仓库，现在想要将本地仓库连接到远程仓库，并将内容推送到远程仓库
## 1. 如果本地还没有创建git仓库
git init  初始化git本地仓库
## 2. add 添加文件到暂存区
git add <filename> 添加指定文件
或者 git add * 添加所有
## 3. commit 到本地仓库的HEAD
git commit -m "对提交信息的概述"
## 4. git remote add origin <service> 关联远程仓库
git remote add origin <远程仓库地址>
## 5. push 将HEAD中的内容推送到远程仓库
git push origin master(远程仓库分支到名称)
### eq:这里可能会报错，原因是远程仓库的README.md文件本地没有，解决方法如下：
### 1. git pull --rebase origin master 将远程仓库的内容同步到本地并merge合并，相当于fetch+merge
### 2. git push origin master 推送到远程仓库


