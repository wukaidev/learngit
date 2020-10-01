# learngit
## 1.下载项目

**git clone**  https://github.com/wukaidev/learngit.git #从github下载项目

## 2.更新远程的内容到本地

**git fetch**是将远程主机的最新内容拉到本地，用户在检查了以后决定是否合并到工作本机分支中。

**git pull**则是将远程主机的最新内容拉下来后直接合并，即：**git pull = git fetch + git merge**，这样可能会产生冲突，需要手动解决。

git fetch origin master #从远程主机的master分支拉取最新内容 
git merge FETCH_HEAD #将拉取下来的最新内容合并到当前所在的分支中

## 3.上传内容到远程仓库

**git push** origin master #把本地仓库提交到远程仓库的master分支中

$ git push origin test:master #提交本地test分支作为远程的master分支

$ git push origin test:test #提交本地test分支作为远程的test分支

git push origin :test #刚提交到远程的test将被删除，但是本地还会保存的，不用担心。

README.md中新增加的一句，用来测试git stash
