Git Init

该命令用于初始化一个  Git 仓库，一般直接使用 `git init` 即可。另外 `git init` 支持使用模板，可以在某些情况下方便初始仓库使用。

命令
```
git init --template=<template>
会将 template 目录下的文件拷贝到 .git 目录下
```

可能使用场景

1. 在公司会将全局的 git config 配置为公司的相关信息（user.name 和 user.email），在这种情况下，创建自己的仓库时 `git init` 出来的也会同样使用全局的 config 信息。这个时候使用 --template 就可以比较方便的解决这个问题

```
git init --template=<template>

其中 template 是一个目录，里面包含一个 config 文件, 里面增加一些基本的信息（user.name 和 user.email 以及其他最基本的信息）。
```

这样新仓库的用户名和邮箱就是自己的了。

