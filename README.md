1. git与svn的差别是什么？
2. 安装git
3. 安装tortoise git
4. 分别使用git命令创建版本库和使用tortoise git创建版本库；
git init
git init "folder name"

git status
//show the working tree status
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
git rm <file_name>
//delete file from repository & filesystem
git rm -r <folder_name>
//delete all the files in folder named <folder_name> 
10. 忽略文件、文件夹
echo '.DS_Store' >> .gitignore
//quickly create .gitignore in terminal

in .gitignore:
-temp (just write down folder name)
//ignore folder names "temp"
-ignore.html (just write down file name)
//ignore file named "ignore.html"
-abc*
//ignore all files that name leading with "abc"
-*.py
//ignore all files that name ened with ".py"
-*.py?
//The character "?" matches any one character except "/"
11. 在gitee上注册账号，并创建远程仓库

12. 添加远程仓库

13. 将本地库push到远程库

14. 删除本地库，从远程库克隆

15. 创建分支
git chechout <branch_name>
//switch to branch names <branch_name>
git checkout <hash_value>
//switch to selected commit
git checkout -b temp
//switch to a new branch "temp"

git branch
//check all branch & current branch
git branch <branch_name>
//create a new branch with branch_name, 
//if there alrady have branch with the name you want to create, will return error

git branch --delete <branch_name>
//delete branch, cannot delete current active branch or branch not existing

git branch -D <branch_name>
//[forced delete]delete branch, cannot delete current active branch or branch not existing
16. 合并分支
git merge <branch_name>
//merge branch
17. 解决冲突
