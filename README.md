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
