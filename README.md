# Note 学习笔记
## 一、sass
1. sass 基于ruby环境 先安装ruby
2. npm install -g node-sass   (全局安装node-sass)
3. node-sass -w css.scss aa.css --output-style expanded 
## 二、git 常用命令
### 1.取得git仓库
<1> 初始化一个版本仓库

    git init

<2> 克隆远程仓库

    git clone git@xbc.me:wordpress.git(url)  可加仓库名
   
<3> 添加远程版本库origin，语法为 git remote add [shortname] [url]

    git remote add origin git@xbc.me:wordpress.git
    
<4> 查看远程仓库

    git remote -v
    
### 2.提交修改

<1> 添加当前修改的文件到暂存区

    git add .

<2> 如果你自动追踪文件，包括你已经手动删除的，状态为Deleted的文件

    git add -u
   
<3> 提交修改

    git commit -m '你的注释'
    
<4> 查看文件状态

    git status
    
<5> 跟踪新文件

    git add readme.txt

<6> 从当前跟踪列表移除文件，并完全删除

    git rm readme.text
   
<7> 仅在暂存区删除，保留文件在当前目录，不再跟踪

    git rm -cached readme.txt
    
<8> 重命名文件

    git mv readme.txt readme
    
<9> 查看提交的历史记录

    git log

<10> 修改最后一次提交注释的

    git commit --amend
   
<11> 忘记提交某些修改，下面的三条命令只会得到一个提交。

    git commit –m "add readme.txt"
    
    git add readme_forgotten
    
    git commit –amend
    
<12> 假设你已经使用git add .，将修改过的文件a、b加到暂存区 现在你只想提交a文件，不想提交b文件，应该这样
     
    git reset HEAD b
    
### 3.基本的分支管理
<1> 创建一个分支

    git branch iss53

<2> 切换工作目录到iss53

    git checkout iss53
   
<3> 将上面的命令合并到一起，创建iss53分支并切换到iss53

    git checkout -b iss53
    
<4> 合并iss53分支，当前目录为master

    git merge iss53
    
<5> 合并完成后没有出现冲突，删除iss53分支

    git branch -d iss53

<6> 拉取远程仓库的数据

    git fetch
   
<7> fetch会拉取最新的远程仓库数据，但不会自动到当前目录下，要自动合并

    git pull
    
<8> 查看远程仓库的信息

    git remote show origin
    
<9> 建立本地的dev分支 追踪远程仓库的develop分支

    git checkout –b dev origin/develop



