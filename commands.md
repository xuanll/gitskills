# Git commands

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
 
### 打标签
- git **tag** *v1.0* /[commit id/]

### 推送标签到远程服务器
- git **push** *origin* *v1.0*
- 一次性推送全部尚未推送到远程的本地标签

  git **push** *origin* --tags
  