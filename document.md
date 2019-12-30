# 1. GitHub的使用
## 1.1 配置github基本信息

    git config --global user.name 'github的用户名'
    git config --global user.email '自己的邮箱'


## 1.2 初始化github

    git init

- 分析
    1. 会在当前目录下出现.git文件


## 1.3 下载自己的项目到当前目录下

    git clone xx        // xx自己的项目地址


## 1.4 添加文件到暂存区

    git add 文件
    git add --all       // 添加全部文件到缓存区


## 1.5 查看修改过的文件

    git status


## 1.6 将暂存区的文件提交到本地仓库

    git commit -m "提交说明"


## 1.7 将本地的仓库提交到远程仓库中

    git push