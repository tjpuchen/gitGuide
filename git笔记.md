##git笔记


1.如何配置用户名邮箱及默认diff工具(初始使用前必须配置本地账号和邮箱)

git config --global user.name “Zhang san"
git config --global user.email  zhangsan@163.com
git config --global merge.tool vimdiff

2.克隆远程版本库

git clone <url>

3.获取git帮助的方法

git help <verb>
git <verb> --help
man git-<verb>
