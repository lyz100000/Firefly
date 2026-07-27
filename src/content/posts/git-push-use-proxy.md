---
tags: [开发工具]
title: Git Push速度慢?设置代理
published: 2026-07-27 20:43:00
description: Git设置代理
image: https://git-scm.com/images/logo@2x.png
category: 前端开发
draft: false
---
# 前言
在使用Git Push时，发现速度较慢，故打开Clash使用代理，发现并无效果。推测git默认不走系统代理，所以需要配置git的http代理。

# 方法
使用终端或cmd等输入
```cmd
git config --global http.proxy http://localhost:7890
```
将`http://localhost:7890`更改为自己的代理服务器即可。