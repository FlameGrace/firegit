# firegit
# Learning git repository.
## Remote
1. git remote 列出所有的远程仓库
2. git remote -v 列出远程库详细信息
3. git remote add origin git@github.com:FlameGrace/firegit.git 链接远程仓库
## Reset  
1. git reset --hard HEAD 恢复到当前版本
2. git reset --hard HEAD^ HEAD^^ 恢复到上一个版本 上上一个版本
3. git reset --hard xx 回退到某一个版本
## Log   
1. git log 列出日志
## Add  
1. git add (-f) xx 添加或强制添加
## Status
1. git status 列出当前仓库状态
## RM
1. git rm file 删除某个文件
## Push
1. git push origin master 上传本地分支仓库到远程仓库
2. git push origin v1.0 上传标签到远程 
3. git push origin --tags 上传所以标签
4. git push origin :refs/tags/v1.0 先删除本地tag再执行此命令删除远程标签
## Clone
1. git clone git@github.com:FlameGrace/firegit.git 从远程仓库克隆项目
## Checkout
1. git checkout -b dev 创建并切换到分支
2. git checkout -b dev origin/dev 创建远程分支到本地
3. git checkout master 切换分支
4. git checkout file 删除工作区修改
5. git checkout -- file 撤销工作区修改
## Branch   
1. git branch -d dev  删除分支
2. git branch -D dev 强制删除分支
3. git branch dev 创建分支 
4. git branch 列出所有分支
5. git branch --set-upstream dev origin/dev 指定本地分支与远程分支的链接
## Merge
1. git merge dev 合并分支
## Stash  
1. git stash 保存工作现场
2. git stash list 列出当前的快照
3. git stash drop xx销毁快照
4. git stash pop 恢复工作现场并删除快照
5. git stash apply xx 恢复工作现场 
## Pull
1. git pull 从远程仓库下载最新的版本
## Tag
1. git tag v1.0 创建一个标签
2. git tag 列出所有标签
3. git tag -a v1.0 -m "dd" 对指定的标签创建说明
4. git show v1.0 查看说明文字
5. git tag -s v1.0 xxxxx 给指定的标签用私钥签名  必须安装gpg
6. git tag -d v1.0 删除本地标签
## Checkout-ignore 
1. git checkout-ignore -v xx  查找为什么添加不了某个文件，是否是忽略规则的原因
## Config
1. git config --global alias.st status 配置别名
