# git学习
###git基础命令
- Git仓库配置：
> git config --global user.name "Your Name"  
> git config --global user.email "email@example.com"

- Git初始化：
> git init

- 添加文件到Git仓库：
> git add File_Name  
> git commit -m Message

- 查看git提交状态：
> git status

- 查看文件修改情况：
> git diff

- 查看提交历史记录：
> git log  
> git log --pretty=oneline

- 查看命令历史记录：
> git reflog

- 丢弃工作区修改：
> git checkout -- File_Name

- 撤回暂存区修改：
> git reset HEAD File_Name

- 删除Git仓库里的文件：
> git rm File_Name

- 恢复工作区误删除的文件：
> git checkout -- File_Name

- 恢复仓库中误删除文件（回滚到未删除的版本）：
> git reset --hard HEAD^  

### git远程连接
- 关联远程库
> git remote add origin git@server-name:path/repo-name.git

- 第一次推送master分支
> git push -u origin master

- 推送master分支
> git push origin master

- 克隆仓库
> git clone

- 关联远程分支
> git branch --set-upstream-to=origin/Branch_Name Branch_Name

- 查看远程库信息
> git remote -v

- 从远程拉取最新信息
> git pull

- 从本地推送分支
> git push origin Branch_Name

- 在本地创建和远程分支对应的分支
> git checkout -b Branch_Name origin/Branch_Name


### 分支管理
- 创建并切换分支
> git checkout -b Branch_Name

- 仅创建分支
> git branch Branch_Name

- 切换分支
> git checkout Branch_Name

- 查看当前分支
> git branch

- 合并某分支到当前分支
> git merge Branch_Name

- 删除分支
> git branch -d Branch_Name

- 查看分支合并图
> git log --graph

- 强行删除未合并的分支
> git branch -D Branch_Name

