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



# 2. 高效使用github
## 2.1 名称搜索

    in:name xx                      // 搜索标题为xx的项目
    in:readme xx                    // 搜索项目的readme包含xx的项目
    in:description xx               // 搜索项目描述中包含xx的项目


## 2.2 下载量筛选

    in:name xx stars:>1000         // 下载量大于1000


## 2.3 语言筛选

    in:name xx language:javascript


## 2.4 时间限制

    in:name xx pushed:>2019-09-03



# 3. 关联本地的仓库到远程的仓库

## 3.1 清除本地的关联，防止其他关联占用

    git remote rm origin

## 3.2 关联本地仓库和远程仓库

    git add git remote add origin xx        // xx为克隆下载的地址

## 3.3 添加本地的仓库

    git add .
    git commit -m ''

## 3.4 推送
如果是第一次推送，同时确保远程仓库中没有内容，则使用如下的命令

    git push -u origin master

如果不是远程仓库中与README.md文件，那么我们应该使用如下的命令,表示强制推送，即会覆盖源文件

    git push -f origin master



# 4. 同步远程仓库到本地

    git pull --force  <远程主机名> <远程分支名>:<本地分支名>
    git pull                       // 开始更新
 
