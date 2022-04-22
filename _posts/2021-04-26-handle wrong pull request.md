---
layout: post
title:  "handle wrong pull request"
date:   2021-04-26
categories: git
---
1. reopen the pull request
2. checkout to the branch which you made the pull request
3. reset commit to the (which you want to reset) commit(that means remove all you new code)
```
$ git reset --hard HEAD^         回退到上个版本
$ git reset --hard HEAD~3        回退到前3次提交之前，以此类推，回退到n次提交之前
$ git reset --hard commit_id     退到/进到 指定commit的sha码
```
4. git push --force
5. git push -d origin branch_name
6. git branch -d branch_name