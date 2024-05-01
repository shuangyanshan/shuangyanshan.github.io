---
title: ardunio
date: 2024-04-27 03:05:59
description:
index_img:
tags:
categories: 
- knowledge
archive:
---


# 把用户文件夹改了名之后发现arduino崩了/只能用管理员权限运行/老是在创建原用户文件夹怎么办？
答：
1. 确保你删得干干净净，；连隐藏文件都被你删了（没错就是appdata中的.arduinoIDE文件夹）（推测，待验证）

2. 将上面提及的文件夹点开，把arduino—cli.yaml文件中的路径中的原用户名全部改成现在的用户文件夹名。然后重启软件。

*.arduinoIDE文件夹是*