#Git 的用法
 1.git init 初始化git仓库  
 2.git add filename 把要添加的文件放进缓存区,可执行多步      
 3.git commit -m "description"  把缓存区的文件提交到仓库  
 
 4.git status 查看仓库的状态  
 5.git diff 查看修改的内容  
 
 6.git log 查看提交的历史 确定回退的版本  
 7.git reflog 查看命令的历史 确定未来的的版本  
 8.git reset --head commit-id 确定要穿梭到的版本  
 
 9.git checkout -- filename  撤销工作区的修改  
 10.git reset HEAD filename  把暂存区的修改撤销放到工作区  
 
 11.git checkout -- filename 用版本库的版本代替工作区的版本  
 12.git rm filename 删除版本库中的文件  
 
 13.git remote add origin git@github.com:xxxxx/xxx.git 本地仓库跟远程仓库关联  
 14.git push -u origin master 第一次提交加-u
  
  
 15.git checkout -b dev 创建并切换到分支dev  
    git checkout -b dev=git branch dev+git checkout dev  
 16.git branch  列出所有分支,当前分支前面有*  
 17.git checkout master 切换到master分支  
 18.git merge dev   合并dev分支的修改  
 19.git branch -d dev 删除dev分支  
 20.合并分支可能造成冲突,先解决冲突,再提交就可以了  
 21.git log --graph 查看合并分支图
 
 22.git merge --no-ff -m "description" dev 有痕迹的合并分支可以用git log查看分支历史  
 
 23.git stash 保存正在进行的工作  
 24.git stash list 查看保存的目录  
 25.git stash apply 恢复工作现场但是不删除stash里的目录,需要删除用git stash drop  
 26.git stash pop 恢复工作现场并且删除stash里的目录  
 27.git stash apply@{0} 恢复指定的目录  
 
 28.git branch -D filename 删除没有合并过的分支  
 
 29.git remote 查看远程库的信息,加-v 显示详细信息  
 
 30.git tag v1.0 创建一个新的tag  
 31.git tag 查看所有tag  
 32.git tag -a "tagname" -m "tagdescription" 指定标签信息  
 
 33.git tag -d v1.0  删除一个tag  
 34.git push origin tagname 推送标签到远程仓库  
 35.git push origin --tags 推送所有未推送到远程的tag  
 36.git push origin :refs/tags/v0.9 删除远程的tag,先删除本地的tag,在执行此命令。
 
 
  
 
  
 
 