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

#当Dev branch 和master 产生分支路的时候， 使用rebase 来merge， 避免历史中产生旁路
git checkout experiment

git rebase master

  conflict resolve
  
git rebase --continue


git checkout master

git merge experiment

git push


#用squash 合并commit

git checkout experiment

git rebase -i master


git checkout master

git merge experiment

git push

----------------------------------------------------------------------
Step 1. Fetch and check out the branch for this merge request

git fetch origin
git checkout -b junbo origin/junbo
Step 2. Review the changes locally

Step 3. Merge the branch and fix any conflicts that come up

git fetch origin
git checkout origin/dev
git merge --no-ff junbo
Step 4. Push the result of the merge to GitLab

git push origin dev
Tip: You can also checkout merge requests locally by following these guidelines.
-----------------------------------------------------------------------
