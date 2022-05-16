---
layout: post
title:  "Terminal command line"
date:   2020-09-01 11:15:00 +0800
categories: cs
---
```echo $PATH```  
+ pwd: present working directory  
+ This command will list all the files and folders in your current directory.  
```ls -l```  
+ rm: remove a file  
  ```rm file1```
+  This command will remove the dir1 directory recursively. In other words, it will delete all the files and directories in dir1 in addition to dir1 itself. Be careful with this command!  
  ```rm -r dir1```
+ cp: copy a file  
 ``` cp lab1/original lab2/duplicate```  
 + mv: move or rename a file  
  ```mv lab1/original lab2/original```  
 ```mv lab1/original lab1/newname```  
This command does not move the file but rather renames it from original to newname.
+ When you have an incomplete name (for something that already exists), try pressing the tab key for autocomplete or a list of possible names.
#### stop firewall
```systemctl stop firewalld```  
#### start redis
```redis-server /opt/redis.conf
   redis-cli  
```  
