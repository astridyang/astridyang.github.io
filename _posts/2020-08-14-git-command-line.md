---
layout: post
title:  "handle wrong pull request"
date:   2021-04-26
categories: git
---
1. reopen the pull request
2. checkout to the branch which you made the pull request
3. reset commit to the (which you want to reset) commit(that means remove all you new code)
4. git push --force
5. git push -d origin branch_name
6. git branch -d branch_name