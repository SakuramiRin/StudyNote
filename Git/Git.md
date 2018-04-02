# Git

## 分布式版本控制系统与集中式版本控制系统(CVS、SVN)的区别
  git的跟踪管理的是 修改  而非文件

## Git命令
```
git init /将此目录设置为git仓库目录

git add (filename) /将此文件添加到仓库

git commit -m (提交信息) /提交

git status /仓库的当前状态，有没有被修改

git diff /差分

git log /日志

git reset -hard HEAD^ /回退到上一个版本

git reset -hard (commit id) /回退之后再返回至已被覆盖的最新版本

git reflog /git操作命令记录

git checkout (local branch name) /切换本地分支

git checkout -b （local branch name） origin/(remote branch name) /切换远程分支

git checkout . /放弃修改

git checkout - (file name) /放弃指定文件修改

git reset /回退版本

```

## Git 的区域
  工作区 定义进仓库的文件夹
    隐藏文件夹 .git git的版本库
        版本库中又含有 stage（或叫index）的暂存区 和git帮我们自动创建的第一个分支master，以及指向master的指针HEAD
        git add执行了将文件添加到暂存区的操作  而git commit把暂存区的内容提交至分支