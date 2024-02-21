
git常用命令

    git init                                      初始化git仓库
    git add .                                     暂存所有文件
    git commit -m '说明注释'                      提交产生版本记录    每次提交，把暂存区内容快照一份
    git branch 分支名                             创建分支
    git branch                                    查看本地分支
    git branch -d 分支名                          删除分支
    git checkout 分支名                           切换分支
    git merge 分支名                              把分支提交历史记录合并到当前所在分支
    git remote add 远程仓库别名 远程仓库地址       别名唯一，地址是.git结尾的网址
    git pull 远程仓库别名 分支名                   完整写法：git pull 远程仓库别名 远程分支名:本地分支名
    git push 远程仓库别名 分支名                   完整写法：git push 远程仓库别名 本地分支名:远程分支名
    git clone 远程仓库地址                         从0得到一个远程的Git仓库到本地使用
