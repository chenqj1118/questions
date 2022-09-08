https://blog.csdn.net/growing_tree/article/details/111659444
关于Sourcetree  免登录注册破解

git stash 
git reset --soft HEAD^
git reset --hard HEAD^



git branch  查看当前哪个分支

git checkout dev 切换至dev分支

git tatus 查看当前状态 有无要提交的修改

git  pull 更新

git add .  添加当前目录的所有文件到暂存区

git commit -m [message] 提交暂存区到仓库区

git push [remote] [branch] 上传本地指定分支到远程仓库



1. //直接删除
2. $ git rm test.txt
3. $ git commit -m "remove test.txt"
4. //删错了，恢复
5. $ git checkout -- test.txt

| 命令         | 说明                                     |
| :----------- | :--------------------------------------- |
| `git add`    | 添加文件到仓库                           |
| `git status` | 查看仓库当前的状态，显示有变更的文件。   |
| `git diff`   | 比较文件的不同，即暂存区和工作区的差异。 |
| `git commit` | 提交暂存区到本地仓库。                   |
| `git reset`  | 回退版本。                               |
| `git rm`     | 删除工作区文件。                         |
| `git mv`     | 移动或重命名工作区文件。                 |

### 提交日志

| 命令               | 说明                                 |
| :----------------- | :----------------------------------- |
| `git log`          | 查看历史提交记录                     |
| `git blame <file>` | 以列表形式查看指定文件的历史修改记录 |

### 远程操作

| 命令         | 说明               |
| :----------- | :----------------- |
| `git remote` | 远程仓库操作       |
| `git fetch`  | 从远程获取代码库   |
| `git pull`   | 下载远程代码并合并 |
| `git push`   | 上传远程代码并合并 |

1、git查看本地分支

```
git branch
```

2、git 查看代码仓库远程分支：

```
git branch -r
```

（1）git切换到要合并的分支上：

```
git checkout V1.0.2.SP3
```

 (2)git merge合并sp2的代码：

```
git merge V1.0.2.SP2
```