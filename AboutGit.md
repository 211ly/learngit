## 创建仓库

| $ mkdir name             | 创建 repository                 |
| :----------------------- | :------------------------------ |
| **$ cd learngit**        | **进入 repository**             |
| **$ pwd**                | **显示当前目录**                |
| **$ git init**           | **转为git可以管理的repository** |
| **$ git add readme.txt** | **将文件添加到repository**      |
| **$ git commit -m**      | **-m后输入本次提交的说明**      |
| q                        | 退出                            |

## 版本回退

文件修改后，使用add和commit提交给仓库

| $ git status             | 了解当前仓库的状态                                |
| :----------------------- | ------------------------------------------------- |
| **$ git diff name**      | **获得文件修改的内容**                            |
| **$ git log**            | **查看对repository的历史记录**                    |
| $ git reset --hard HEAD^ | 将仓库中的文件回退到上一个版本^,~100回退100个版本 |
| $ git reflog             | 记录每一次的命令                                  |

HEAD指向的版本就是当前的版本，使用git reset --hard commit_id来更改版本，使用git log查看提交的历史，git reflog查看命令的历史

## 工作区和暂存区

工作区（Working Directory）: 可见的目录，比如一个文件夹就是(learngit)

版本库（Repository）：隐藏目录.git并不算工作区，而是Git的版本库。Git版本库中包含一个暂存区（stage），git add命令会将文件的修改添加到暂存区，而git commit是把暂存区所有的内容提交到当前分支。

![1710903075587](C:\Users\YI\AppData\Roaming\Typora\typora-user-images\1710903075587.png)