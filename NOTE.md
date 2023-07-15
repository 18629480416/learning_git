
[TOC]
# git 基本命令

- 配置git 用户名称
git config --global user.name "***"    
- 配置git 用户邮箱
git config --global user.email "***"  
- 初始化git 仓库
git init

- 查看当前提交状态
git status
- 添加文件到暂存区
git add .
- 将文件从暂存区删除
git rm --cached file 

- 恢复修改文件
git restore file

- 恢复到git add 前的状态
git restore --staged file


- 提交文件到本地仓库 
git commit -m "提交描述"

备注：此时 git status 显示：nothing to commit,working directory clean

- 删除仓库文件  
  
1. rm file  
   
2. 删除暂存区文件：git rm file  
   
3. git commit -m "描述"  
   


- 新建分支
git checkout -b dbg_lichen_star

- 推送本地分支到远程
git push origin dbg_lichen_star:dbg_lichen_star

# 删除远程分支、远程文件、远程文件夹
## 删除远程文件

git rm --cached filename(具体删除的文件)  

git commit -m "del: xxx"  

git push origin branch-name(具体的分支名字)
 
## 删除远程文件夹

git rm -r --cached directory-name(具体删除的文件夹)  

git commit -m "del: xxx"  

git push origin branch-name(具体的分支名字)

## 删除远程分支
- git查看分支：  
  
查看本地分支 git branch  

查看远程分支 git branch -r  

查看本地和远程分支 git branch -a


- git删除分支：
  
删除本地分支 git branch -d 本地分支名  

删除远程分支 git push origin --delete 远程分支名

