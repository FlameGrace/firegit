# firegit

## Learning git repository.

## Remote 
+ git remote 列出所有的远程仓库
+ git remote -v 列出远程库详细信息
+ git remote add origin git@github.com:FlameGrace/firegit.git 链接远程仓库
## Reset  
+ git reset --hard HEAD 恢复到当前版本
+ git reset --hard HEAD^ HEAD^^ 恢复到上一个版本 上上一个版本
+ git reset --hard xx 回退到某一个版本
+ git push -f origin master  回退后，需要执行强制提交
## Log    
+ git log 列出日志
## Add    
+ git add (-f) xx 添加或强制添加
## Status 
+ git status 列出当前仓库状态
## RM 
+ git rm file 删除某个文件
## Push
+ git push origin master 上传本地分支仓库到远程仓库
+ git push origin v1.0 上传标签到远程 
+ git push origin --tags 上传所以标签
## Clone  
+ git clone git@github.com:FlameGrace/firegit.git 从远程仓库克隆项目
## Checkout  
+ git checkout -b dev 创建并切换到分支
+ git checkout -b dev origin/dev 创建远程分支到本地
+ git checkout master 切换分支
+ git checkout file 删除工作区修改
+ git checkout -- file 撤销工作区修改
## Branch  
+ git branch -d dev  删除分支
+ git branch -D dev 强制删除分支
+ git branch dev 创建分支 
+ git branch 列出所有分支
+ git branch --set-upstream dev origin/dev 指定本地分支与远程分支的链接
## Merge   
+ git merge dev 合并分支
## Stash
+ git stash 保存工作现场
+ git stash list 列出当前的快照
+ git stash drop xx销毁快照
+ git stash pop 恢复工作现场并删除快照
+ git stash apply xx 恢复工作现场 
## Pull
+ git pull 从远程仓库下载最新的版本
## Tag
+ git tag v1.0 创建一个标签
+ git tag 列出所有标签
+ git tag -a v1.0 -m "dd" 对指定的标签创建说明
+ git show v1.0 查看说明文字
+ git tag -s v1.0 xxxxx 给指定的标签用私钥签名  必须安装gpg
+ git tag -d v1.0 删除本地标签
+ git push origin v1.0  提交本地标签到远程仓库
+ git push origin :v1.0   删除远程仓库的标签
+ git push origin :refs/tags/v1.0  github删除远程tag，需先删除本地tag
## Checkout-ignore
+ git checkout-ignore -v xx  查找为什么添加不了某个文件，是否是忽略规则的原因
## Config
+ git config --global alias.st status 配置别名
## cocoapods
http://blog.csdn.net/stubbornness1219/article/details/50968000


