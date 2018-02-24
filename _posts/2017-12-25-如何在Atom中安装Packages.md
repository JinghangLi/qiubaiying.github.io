---
layout:     post
title:      在Atom中手动安装Packages插件
subtitle:   命令行安装简介
date:       2017-12-25
author:     LJH
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - Atom
    - Packages
    - 手动安装
---
# 前言
### Atom
Atom与markdown的package相配合，可以配置为轻量化的文本编辑器。

### Markdown
Markdown是一种可以使用普通文本编辑器编写的标记语言，通过简单的标记语法，它可以使普通文本内容具有一定的格式。  
[Markdown tutorials](https://www.markdowntutorial.com/)

# 步骤
1. 在Atom的[Packages网页](https://atom.io/packages)中选择想要安装的packages
2. 找到需要的Package后，进入页面，点击 **Repo** 进入该Package在Github中的开源网页
3. 点击 **Clone or download** 复制 web URL 用于 **git Clone** 命令
4. 打开终端，进入隐藏文件目录
```
$ cd .atom/packages/
```
5. 在package目录下克隆这个项目（git clone + 在第三步中复制的 web URL 以teletype的package为例 ）
```
$ git clone https://github.com/atom/teletype.git
```
6. 下载好后，会在package目录下看到自己刚刚下的包，可以用命令 **ls** 查看
```
$ ls
```
7. 进入下载好的package
```
$ cd +package的名字
eg：
$ cd markdown
```
8. 进入后，开始安装
```
$ sudo npm install
```
9. 等待安装好以后，就重启atom。

*注释：如果反馈没有安装npm，则可以在输入命令自己安装npm*
```
$ sudo apt-get install npm
```
