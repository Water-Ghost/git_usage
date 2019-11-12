# git Guide

## 1 添加文件
切换到工作目录
`$ cd /target/dir`  
初始化工作目录  
`$ git init`  
添加当前目录到git  
`$ git add .`  

## 2 添加到远程仓库
`$ git remote add origin https://github.com/your/repository/link.git`  

## 3 push 
设定upstream  
`$ git push --set-upstream origin master`  
推送文件  
`$ git push -u origin master, or git push.`  

## 4 获取远程数据
### 4.1 fetch and merge  
* Fetch files  
git fetch  
`$ git fetch <远程主机名> //这个命令将某个远程主机的更新全部取回本地`  
or fetch the specified branch  
`$ git fetch <远程主机名> <分支名> //注意之间有空格`  
commonly used command  
`$ git fetch origin master`
or simply use  
`$ git fetch`  

* Check the updates info  
`$ git log -p FETCH_HEAD`  

* Merge the updates  
`$ git merge FETCH_HEAD`  

### 4.2 pull
* Synopsis  
`$ git fetch [<options>] [<repository> [<refspec>…]]`  
or simply  
`$ git fetch`  

## 5 修改后提交
`$ git commit -m "change text"`  
push见[步骤3](#3-push)  
