---
layout: post
title:  "Git Command Line"
date:   2020-08-14 14:44:32 +0800
categories: git
---
```git log --stat``` （按向下箭头往下滚动）

git diff id1 id2；不带参数可以比较暂存区和工作目录；  
git diff --staged：对比仓库和暂存区  
按 q 停止查看git log 输出  
git checkout commit id: 检出某个commit  
git checkout abcdef：最新的commit（commit id 可以输入提交 ID 的前四个）  
git reflog，which shows you all the commits that have been checked out recently
mv file1 file2(如果不指定文件夹则重命名)  
```git config --global core.editor "'D:/Program Files (x86)/Microsoft VS Code/Code.exe' -n -w"```  
git add 添加文件到 staging area  
查看状态：git status  
如果你意外地将某个文件添加到暂存区中，可以使用 git reset lesson_2_reflections.txt，此命令会从暂存区中删除该文件，但它仍在你的工作目录中。  
git checkout master: 从某个commit返回（HEAD处于检出旧分支的分离状态）  
git reset --hard：放弃工作目录或暂存区的所有更改  
### 分支：experimental feature/different version
git branch: 查看分支  
git branch 分支名：创建分支；  
git checkout 分支名  
git checkout -b 分支名：创建分支并检出  
直观地查看提交历史记录: git log --graph --oneline master coins  
git merge master 分支名;  
git merge 还将在合并的版本中包含当前检出的分支  
git show commit_id: 查看commit与父级的比较  
git branch -d 分支名：删除分支  
合并冲突时：git merge --abort：将文件恢复到你开始合并之前的状态  
 git branch --set-upstream-to=origin/远程分支 本地分支：本地分支与远程分支建立联系  
撤销commit  
```git reset --hard commit_id```  
#### 暂存  
```git stash```  
```git stash pop```
### git全局配置
git config --global push.default upstream  
git config --global merge.conflictstyle diff3  
git config --global color.ui auto  
将以下一行添加到 .bash_profile  
alias vsc="D:/Program Files (x86)/Microsoft VS Code/Code.exe"
### 其他命令行
移到主目录：cd ~  
查看隐藏目录：ls -a  
退出vim :q  

修改最近的某个commit message  
+ ```git rebase -i HEAD~3/SHA-1码/--root ```   
+ ```git commit --amend```
+ ```git rebase --continue``` option
+ ```git push origin master [-f]```  
拉取时远程有修改，先  
```git pull --rebase```  
pull远程仓库的代码到本地，强行覆盖本地的所有修改  
```git pull --rebase origin master```
