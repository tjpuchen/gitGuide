# git笔记


#### 1.如何配置用户名邮箱及默认diff工具(初始使用前必须配置本地账号和邮箱)

git config --global user.name “Zhang san"  
git config --global user.email  zhangsan@163.com  
git config --global merge.tool vimdiff  

#### 2.克隆远程版本库

git clone <url>  

#### 3.获取git帮助的方法

git help <verb>  
git <verb> --help  
man git-<verb>  
  
#### 4.查看本地工作空间状态的命令
 
 git status  

#### 5.add 过程中将文件的修改，新建，添加到暂存区的参数

git add .

#### 6.diff 时 HEAD和工作区比较的参数

git diff HEAD

#### 7.commit 时 填写提交log的参数

git commit -m "message"  

#### 8.将本地已提交的内容，推送到远程仓库

git push origin [远程branch_name]

#### 9.在本地切换分支

git checkout [本地分支branch_name]   注：在本地切换分支时，本地工作目录必须都已提交，否则将会把未提交的内容merge到目标分支中

#### 10.删除文件夹并存入暂存区

git rm -rf 文件夹

#### 11.查看提交日志

git log 

#### 12.创建标签、补打标签、删除标签、将本地所有标签推送到服务器

git tag tag_name  
git tag tag_name HASH_version  
git tag -d tag_name  
git push origin --tags  

#### 13.修改最后一次提交

git commit --amend  

#### 14.取消本地工作空间文件的修改

git checkout filename  

#### 15.取消已经暂存的文件

git reset filename

#### 16.将本地工作空间，暂存区及本地仓库都重置到历史都某一个版本

git reset--hard hash_version

#### 17.查看，创建、删除、合并分支，如何将本地分支推送到服务器

git branch -a  
git checkout -b branch_name  
git branch -d branch_name  
git merge branch_name  
git push origin branch_name  

#### 18.恢复贮藏文件

git stash pop

#### 19.拉取远程创建的分支(本地没有的分支)到本地

git fetch origin [远程分支名]:[本地分支名]  
git checkout [本地分支名]

#### 20.更新远程分支修改内容到本地

git checkout [本地分支名]  
git pull origin [远程分支名]  

或者

git checkout [本地分支名]  
git fetch origin [远程分支名]  
git merge [本地分支名]   

在本地分支没有代码修改（add or commit）的时候，方法一 和 方法二效果是一致的。  
但如果本地有了新的commit但没有push，pull方法就会自动的merge代码，而fetch需要自己merge。  











