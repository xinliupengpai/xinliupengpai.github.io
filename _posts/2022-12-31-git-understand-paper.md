---
title: git常用命令
tags: ['git', '明白纸']
key: 2022-12-31-git-understand-paper.md
---


# git常用命令

## 编辑

### 初始化

```shell
git config --global user.name "xxx"
git config --global user.email "xx@xxx"
git config --global -l
git init
```

### 编辑

```shell
git add file
git add -A
git rm file
git commit -m "mark"
```

### 查看比对

```shell
git status

git diff file 工作区和暂存区
git diff --staged file 暂存区和版本库
git diff HEAD file 工作区和版本库
git diff --stat f6792677a4d9..master

git diff master dev
git diff dev origin/master

git log --pretty=oneline --graph --max-count=5
git reflog
```

### 储藏当前工作

```shell
git stash
git stash list
git stash pop
git stash apply stash@{0}
git stash drop stash@{0}
```

## 版本回退

### 回退工作区

```shell
git restore file
```

### 回退暂存区

```shell
git restore --staged file
```

### 回退仓库

```shell
git reset --hard xxxxxx # 版本回退
--soft # 暂存区和工作区的内容不会改变
--mixed # 默认，暂存区和版本库一致，所有变动保存在工作区。
--hard # 丢掉暂存区和工作区的变动
git revert xxxx # 撤销指定commit，产生新的提交
```

## 分支

### 创建

```shell
git branch testing # 创建分支
git branch dev; git push origin dev; # 创建远程分支
```

### 查看

```shell
git branch -vv # 查看
git branch -a
```

### 关联

```shell
git branch -u origin/dev dev # 设置远程分支
```

### 切换

```shell
git switch testing
```

### 合并

```shell
git switch master
git merge testing
git cherry-pick 4c805e2
```

### 删除

```shell
git switch master
git branch -d testing
git push origin --delete dev2 # 删除远程分支
```

## 远程仓库

### 关联

```shell
git remote add origin git@github.com:user_name/Repository_name.git
```

### 查看

```shell
git remote -v
```

### 修改

```shell
git remote update origin git@github.com:user_name/Repository_name.git
```

### 删除

```shell
git remote rm <name>
```

### 拉取

```shell
git fetch origin master
git merge origin/master

git pull origin master
```

### 推送

```shell
git push -u origin master
git push --force origin main
```
