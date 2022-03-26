+++
title = "使用zola建立博客"
date = 2022-01-09T18:18:18+08:00

[taxonomies]
tags = ["Rust"]

+++

> zola 是使用 Rust 编写的较为流行的静态网页生成工具，主要用于博客的搭建。接下来我会简单描述在 Github Pages 上使用 zola 搭建博客的整个过程
---
## 初始化你的博客
### 安装 zola  
我使用的是 Windows 下的 WSL, 使用 Homebrew 作为包管理工具，安装命令为: 
```
brew install zola
```
### 初始化目录
使用 zola init 命令初始化博客目录
```
zola init blog
```
## 安装主题
### 进入主题文件夹
```
cd blog/themes
```
### 将主题添加为子模块
```
git submodule add https://github.com/carpetscheme/lightspeed.git lightspeed
```
### 自动CI/CD
参照官方文档: *[传送门](https://www.getzola.org/documentation/deployment/github-pages/)*
## 使用体验🐱
> 基于 Cargo，安装简单。相较于先前使用的 Pelican 生成效率更高。生成的文章的名称有预处理，对非英语使用者较为友好。缺点是目前生态不够完善，主要是主题方面，但是用作写作足矣
