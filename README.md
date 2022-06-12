# trial_GitHub
First Git trial  

------

# 2022_06_12update

## GitHub常见按钮

+ Pin/Unpin 将该项目钉到你的主页上/将该项目从主页上移除

  `若未设置任何项目置顶，则主页第一个模块是Popular repositories，即 系统推荐的受欢迎仓库；而只要置顶了某个项目，这一模块就会被替代为Pinned，即 已被置顶的（仓库）。`

+ Watch/Unwatch 接收/不接受该项目的新通知

  `可以选择通知的范围。一：参与或者被@时通知；二：接收所有变化通知；三：忽略所有通知；四：自定义——在参与和被@基础上增加一些可被通知的事件。`

- Star/Starred 星标/已星标

  `可以在自己主页中找到Star过的项目，并分类。主要为了使用时能快速找到；也为一些看起来不错的项目提供了吃灰的场所。`

- Fork 分岔，岔开 —— 类似开辟一个新的分支

  `这个分支是自己的，完全独立于原项目，可以任意CRUD{即增加(Create)、检索(Retrieve)、更新(Update)和删除(Delete)}；`

  `当然，你也可以为原项目出一份力，给源仓库发送Pull Request：如果原作者认为你的修改版本还不错，就会将你代码中的修改合并到自己的库中。`

## Git操作流程

- DOS命令（Disk Operating System 磁盘操作系统）

  - cd 进入指定目录；

  - md/mkdir 新建目录；

  - rmdir 移除目录；dir 查看当前目录中的文件和文件夹 —— linux中是ls，short for list；

  - 要显示以 “.”开头的隐藏文件/文件夹，用 dir /a:h —— linux中ls -la即可显示所有； 

    `当然，用git bash的话，就不需要dir了，它和linux命令是通用的；直接ls -la即可显示当前目录下的所有项目。`

- git init

  `如果是空的文件夹，会提示Initialized empty Git repository in 路径/.git；`

  `而如果是既有项目，会提示Reinitialized existing Git repository in 路径/.git；`

- git clone

  `点击Code按钮，复制HTTPS链接至命令行即可`

- vim .git/config

  `查看配置文件`

- git status

  `查看当前目录的文件状态；提示Untracked files，会列出未追踪的文件列表`

- git add

  `追踪项目中新增的文件/文件夹`

  `git add ./ 追踪多个文件/文件夹，有无斜杠皆可。`

  `在VSCode里点击Source Control中文件名右侧的加号亦可暂存，暂存后状态会从Changes变成Staged Changes 即暂存的更改；并且可以加上Message，再点击“√”进行提交。`

- git commit -m "版本信息"

  `提交之后再git status就不会提示有Changes了。`

- git branch -M main —— 切换到主分支，我们的小东西只有一个主分支，不用动它

- git remote add origin git@github.com:simplylike/trial_GitHub.git

  `Code > SSH → copy it`

  `即 将新的本地仓库与GitHub仓库关联起来`

- 推送出去：git push -u origin main

- 修改完成后提交：git commit
  
- 如多人同时处理同一个仓库，提交之前最好先拉一下：git pull

- 把仓库转移到组织当中：Settings > Transfer Repository
