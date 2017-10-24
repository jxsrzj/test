### what is git?
- 是一个源代码管理工具。
- 在一个项目中，凡是由开发人员编写的都算源代码
- 源代码为什么需要管理？
- 让源代码可以被追溯，主要记录每次变更了什么，谁主导的这次变化
- 人为管理和维护比较麻烦。
- GIT是Linux之父当年为了维护Linux的源代码编写的一个工具
- GIT之前都用什么？  svn vss tfs  ......


# git基本命令

- 初始化一个仓库
```shell
cd 项目根目录
$ git init   //初始化一个本地的仓库
```

> 就是在本地文件中添加了一个.git的文件夹用于记录所有的项目变更信息

- 查看本地仓储的变更状态
```shell
$ git status
$ git status -s
```

- 添加本地暂存(托管)文件
```shell
$ git add <file>
$ git add --all  &&  git add .
```

类似于node_modules这种性质的文件夹不应该被托管

- 添加一个本地GIT的忽略清单文件
在代码库文件夹的根目录添加一个.gitignore文件
该文件用于说明忽略的文件有哪些

- 设置名字和email
```shell
$ git config --global user.email 'you@email.com'
$ git config --global user.name 'your Name'
```

- 提交被托管的代码变化到本地仓库
```shell
$ git commit -m '....'
```

- 查看提交日志
```shell
$ git log
```

- 回到指定版本
```shell
$ git reset --hard 
```

- 对比差异
```shell
$ git diff
```

### github是什么？
- 只是一个网站
- 同性交友社区 都是程序员。
- https://github.com/
- 提出概念 社交化编程
- github和git的关系？
- 它是git的服务提供商，提供了free仓库 - 前提，开源

