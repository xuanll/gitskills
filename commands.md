# Git commands

* 运行 Git Bash ，进入到安装目录 直接运行 "Git Bash" (Windows 下 "Git Bash.vbs")

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