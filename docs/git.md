>Git 操作 换远程仓库地址

- [ ] git remote 查看所有远程仓库
- [x]  git remote get-url origin查看远程仓库origin的url地址
- [ ] git remote set-url origin xxx 给远程仓库修改地址
先增加第一个地址 git remote add origin url1
然后增加第二个地址 git remote set-url --add origin url2
增加第三个地址 git remote set-url --add origin url3

>【删除远程分支】

git remote remove origin


>【分支合并】

git checkout dev
git pull
git checkout master
git merge dev

>如果本地和远程分支关联了，就不需要 -u以及后面的命令了
git push -u origin master

>【查看远程仓库地址】
git remote -v

>【将本地代码推到远程仓库】
- 首先在github建立新的仓库获取仓库链接
- git remote add origin https://github.com/MoreCodeByTR/vue-demo.git。 // 增加远程仓库地址
- git branch -M master       // 分支重新命名
- git push -u origin master               


>【git版本回退】
- 查看所有的历史版本，获取你git的某个历史版本的id， git log
- 回退本地代码库：git reset --hard ID
- 推送到远程服务器：git push -f -u origin [branchName]
- 重新拉代码：git pull


>【git更新密码】

 git config


>【查看本地与远程分支关联关系】

git branch -vv

git push --set-upstream origin branch_name