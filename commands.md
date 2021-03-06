# [Git commands](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)

* 运行 Git Bash ，进入到安装目录 直接运行 "Git Bash" (Windows 下 "Git Bash.vbs")

### 从远程仓库(Github)Clone
- git **clone** git@github.com:*xuanll*/*u3dnotes*.git 

### 新增/更新文件
- git **add** file.txt

### 删除文件
- git **rm** file.txt

### 本地commit提交
- git **commit** -m "comments"

### 本地分支master推送到远程origin
- git **push** *origin master*

### 查看当前仓库状态
- git **status**

### 拉取远程仓库内容
- git **pull** --rebase *origin master*

### 查看log信息 
- git **log** --pretty=oneline

### 查看分支合并图
- git **log** --graph 

### 查看远程库信息
- git **remote** -v 

### 创建并切换到分支
- git **checkout** -b *0723*
- 等同于两个命令的组合：

  git **branch** *0723*
  
  git **checkout** *0723*
  
### 合并分支0723到当前分支

- git **merge** *0723* 
 
### 打标签
- git **tag** *v1.0* [commit id]

### 推送标签到远程服务器
- git **push** *origin* *v1.0*
- 一次性推送全部尚未推送到远程的本地标签

  git **push** *origin* --tags
  
### 丢弃工作区修改(未添加到暂存区， **-- 后有空格**)
- git **checkout** -- *commands.md*

### 丢弃修改（已添加暂存区）
1. git **reset** *HEAD* *commands.md*
2. git **checkout** -- *commands.md*

### 历史版本时光机
- git **reset** --hard commit_id   

### 查看命令历史
- git **reflog** 

### 生成SSH密钥(ssh_pub文件)
- ssh-keygen -t rsa -C "example@mail.com"

### Fetch
- git **fetch**

### 本地仓库推送到Github
- git **remote add** *origin* *https://github.com/xuanll/HelloPebble.git*
- git push -u origin master  

> - 远程库的名字就是origin，这是Git默认的叫法
> - 第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。

### 在服务器端建立Git仓库
- git **init** *--bare* sample.git