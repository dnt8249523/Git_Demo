1. git与svn的差别是什么？
2. 安装git
3. 安装tortoise git
4. 分别使用git命令创建版本库和使用tortoise git创建版本库；
git init
git init "folder name"
5. 添加文件到版本库
git add "filename"
git add README
git add *.html

git add .
//add all, will only add files located in the root directory.
git add -a 
or
git add --all
//add all
6. 修改文件并提交到版本库；
git commit -m "some message"
git commit -m "some message(title)" -m "some description"

git commit -a -m"some message"
//do "git add" & "git commit" at the same time
7. 查看提交历史；比较历史的差异修改；
git log 
//show history
git log -p
//-p Or -patch, which shows the difference
git log -p -2
//-2 to show only the last two entries.

git diff
//show the changes between local file and staging file
8. 修改文件后，还原；
git log
//check all commit history
git log --oneline 
//check commit history in this branch

git checkout <hash value>
//switch to the pointed commit
9. 删除文件
10. 忽略文件、文件夹
11. 在gitee上注册账号，并创建远程仓库
12. 添加远程仓库
13. 将本地库push到远程库
14. 删除本地库，从远程库克隆
15. 创建分支
git checkout -b temp
//switch to a new branch "temp"

git branch
16. 合并分支
17. 解决冲突