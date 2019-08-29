# GroceryStore
begin
#把内容输入到一个文件
echo "xxxx" > xxxx 
#把工作空间的某个文件添加到 cache
git add  xxxx
#把工作空间的所有内容添加到 cache
git add -A
#把 cache 当中的某个文件提交到本地库
git commit -m "xxxx"
#all
git commit -am "xxxx"
#cache ---->work file 恢复一个文件  file1 file2 恢复两个文件  . 恢复所有文件
git checkout readme.txt 
#git 状态查询
git status
#查看不同的地方 默认查看工作区和 cache
#git diff --cached   比较 cache 和 Repository
#git diff HEAD 工作区和最新的 Resository
#git diff commit-id 工作区和制定的 repository
#git diff --cached commit-id
#git diff --commit-id commit-id
git diff 
#reset 顾名思义   （HEAD~100）
git reset HEAD^
#git 的日志
git log git log --pretty=oneline
#oh my pretty pretty boy i love you 
git reflog  查看历史命令
#git rm --cached file_path
git rm 
git mv
#远程仓库的克隆岛本地库
git clone
#关联远程仓库
git remote add
#推送到远程仓库
git push
#拉取远程仓库的内容
git pull
#查看当前分支 -a 查看所有分支 -av 查看所有分支的信息 -avv 查看所有分支的信息和关系
git branch
#创建一个分支 基于当前分支创建分支
git branch  xxx
#基于 oldType 创建分支
git branch newBranch oldType
#切换分支
git checkout 分支的名字
#删除分支
git branch -d   xxx
#查看文件内容
git cat-file -p  commitid
#查看对象类型 blob commit tree
git cat-file -t commitid
