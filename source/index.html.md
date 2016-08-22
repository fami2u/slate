---
title: aics使用文档 －－ fami2u独立开发者组织

language_tabs:
  - shell

toc_footers:
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - resources
  - history

search: true
---

# AICS 概览

```shell

# 安装 aics:

 sudo npm install -g aics
    
```


  欢迎查阅aics使用文档。

  aics是一款覆盖Meteor应用开发周期的，提供Meteor应用极速开发体验的工具。

  在使用过程中遇到任何问题或有任何改进的建议欢迎在项目[讨论区](https://github.com/fami2u/aics/issues) 提出

# 项目部署 deploy



```shell

# Examples:
    $ aics deploy appName  # Deployment to http://appName.aics.cn 
    $ aics deploy appName --env env.json
```

用法: ` aics deploy [options] <project> <key>`

Deployment this project to fami2x.com microhost

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -m, --mobile-settings <mobile-settings.json> | Set mobile-settings from json file
  -s, --server-only                             | server only
  -e, --env <env.json>                         | Set environment variables from json file
  -d, --debug                                  | debug mode

# 服务器环境配置 setup

```shell
#  Examples:
    $ aics setup #  configuration your server
    
```

`Usage: aics setup [options]`

Configuration runtime environments on private server

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information


# 部署到私有服务器 push

```shell
#    Examples:
    $ aics push  # config package.js 
    $ aics push
    
```

`Usage: aics push [options]`

Deployment a project to private server

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -m, --mobile-settings <mobile-settings.json> | Set mobile-settings from json file
  -s, --server-only                             | server only
  -d, --debug                                  | debug mode

# 打印服务器日志 logs

```shell
#    Examples:
    $ aics logs  
    $ aics logs -t 100
    
```

`Usage: aics push [options]`

 Print logs on server

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -l, --lines <lines> | output the last N lines, instead of the last 50 by default

# 连接远程数据库 mongo

```shell
#  Examples:
    $ aics mongo
    
```

`Usage: mongo [options]`

Connection to a remote mongo database

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information


# 登录CLI adduser

```shell
#  Examples:
    $ aics adduser
    
```

`Usage: deploy [options] <project> <key>`

登录aics cli

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information


# 登录用户信息 whoami


```shell
#  Examples:
    $ aics whoami
    
```

`Usage: whoami [options]`

 显示 aics 登录用户信息

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information

# 生成aics配置文件 init

```shell
#  Examples:
    $ aics init -p [name] # 创建新的aics项目
    $ aics init -e [name] # 根据 name 生成一个项目
    $ aics init [name] # 生成一个 名为 name 代码包项目 
    
```

`Usage: init [options]`

生成aics配置文件

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -p, --project |  generate aics project conf
  -e, --example |  generate project from example project conf

# 添加 aics 代码包 add


```shell
#  Examples:
    $ aics add fami:readme
    
```

`Usage: add [options] [packagename]`

添加名为 packagename 的 aics 代码包 代码包地址: http://code.fami2u.com/

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  

# 更新依赖 update


```shell
#  Examples:
    $ aics update -a # 更新项目依赖的代码包的版本
    $ aics update [name] # 更新名为 [name] 的代码包依赖的代码包的版本
    
```

`Usage: update [options]`

更新项目或代码包依赖

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -a, --all <path> | update all packages in .aics/packages.json

# 发布 publish

```shell
#  Examples:
    $ aics publish -p [name] # 发布名为 [name] 的 aics 项目
    $ aics publish [name] # 发布名为 [name] 的 aics 代码包
    
```

`Usage: publish [options]`

发布aics项目或组件

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -p, --project <name> | 发布解决方案（项目）

# 添加文件 addfile

```shell
#  Examples:
    $ aics addfile -f README.md -t depot # 添加文件README.md 到 depot 组件包
    
```

`Usage: addfile [options]`

添加文件到组件

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -f, --file <path>  |  文件名或目录
  -t, --target <name> | 添加到的组件名称

# 显示文件 lsfile

```shell
#  Examples:
    $ aics lsfile -t depot # 显示 depot 代码包中的文件
    
```

`Usage: lsfile [options]`

显示指定代码包中的文件

参数  | 描述
--------- | -----------
  -h, - -help                                   | output usage information
  -t, --target <name> | 组件名称