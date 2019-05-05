#删除本地分支

git branch -d [localBranch]

#拉取远程分支

git fetch origin [remotebranch]

git checkout -b [localBranch] origin/[remotebranch]

#缓存/恢复本地修改

git stash

git stash pop

#撤销本地commit

git reset --soft [commitID]    保留代码

git reset --hard [commitID]    全部撤销 不保留代码

#提交分支数据到远程(远程branch 不存在时)

git push origin [local_branch]:[remote_branch]

#删除远程分支

git push origin --delete [remote_branch]

#删除本地分支

git branch -d [local_branch]
