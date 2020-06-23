# 学习笔记
## git
> ### 一. 基本知识介绍[^菜鸟教程]   
> > 1. 安装配置  
> > - 下载地址<http://git-scm.com/downloads>  
> >
> > 2. 设置用户名和邮箱
> > - `git config --global user.name “你的用户名”`
> > - `git config --global user.email “你的邮箱”`  
> >
> > 3. 查看配置
> > - `git config --list`  
> > 
> >4. 修改用户名和邮箱  
> > - `git config --global --replace-all user.name “你的用户名”`
> > - `git config --global --replace-all user.email “你的邮箱”`  
> > 
> ### 二. 工作流程及工作区，暂存区，和版本库
> > 1. 工作流程  
> > ![](C:\Users\deii\Desktop\新建文件夹 (3)\微信图片_20200623191122.jpg)
> >
> > 2. 工作区，暂存区，和版本区
> > ![](C:\Users\deii\Desktop\新建文件夹 (3)\微信图片_20200623191054.jpg)  
> >
> ### 三. 创建仓库 [^ -h]
> > 1. git init
> > - <u>使用当前目录作为git仓库,只需要初始化即可</u>
> >
> > 2. git init newrepo
> > - <u>newrepo目录下会出现一个.git的目录,所有Git需要的数据和资源都存放在这个目录</u>
> >
> > 3. git clone 
> > - git clone [^<repo>]  [^ <directory> ]
> >
> ### 四. 常用命令
> > 1. mkdir
> > > - 创建新文件夹
> > 2. touch
> > > - 创建新的文件
> > 3. git add
> > >  - 将文件添加至暂存库中
> > 4. git status
> > > - 检查文件状态
> > 5. git commit
> > > - 将暂存区里的改动提交到本地的版本库
> > > - 主要用 -m“注释”
> > 6. git branch
> > > - 查看本地分支
> > > - -d 删除本地已合并的分支
> > 7. git checkout
> > > - 切换分支
> > 8. git cherry-pick
> > > - git cherry-pick commit1 commit2: 把commit1和commit2复制到当前分支
> > > - git cherry-pick commit-id：git会自动根据commit-id查找所属分支，并把分支上该commit-id对应的提交内容增加到当前分支
> > > -  git cherry-pick branchName:  把branchName分支的最后一次提交增加到当前分支
> > 9. git push
> > > - 将本地版本库的分支推送到远程服务器上对应的分支
> > 10. git log 
> > >  - 看你commit的日志
> > 11. git reset
> > > - 修改HEAD的位置，即将HEAD指向的位置改变为之前存在的某个版本
> > > - ![](C:\Users\deii\Desktop\新建文件夹 (3)\微信图片_20200623202130.png)
> > 12. git stash
> > > -   备份当前工作区的内容，保存到git 栈中，从最近的一次commit中读取相关内容
> > 13. git revent
> > > - 是用于“反做”某一个版本，以达到撤销该版本的修改的目的\
> > > - ![](C:\Users\deii\Desktop\新建文件夹 (3)\微信图片_20200623202603.png)
> > 14. git pull
> > >  - 本地与服务器端同步
> > 15. git remote
> >  > - 列出所有远程分支
> > 16. git diff
> > > - 查看尚未暂存的更新
> > > # 命令图
> > >   ![](C:\Users\deii\Desktop\新建文件夹 (3)\微信图片_20200623214311.jpg)