---
title: Git没commit就被reset的挽救方法
date: 2017-06-18 17:44:53
categories: 辅助工具
tags: git
---
## git reset --hard 这是一个非常可怕的命令，主要有三个作用
1. 新建的文件已暂存没提交状态回到新建文件之前也就该文件消失（主要）
2. 克隆下来的文件，修改后添加到暂存，使用命令后回到克隆下来的状态，不保留已修改的内容
3. 已提交状态，提示当前位置的HEAD版本）

## git fsck --lost-found （找回刚才add后修改没commit的文件）
文件就在.git/lost-found/other文件中
<img src="/images/git-2.png" alt="丢失的文件" title="丢失的文价" />
复制出来后一个个拖到sublime编辑看是什么内容然后复制回去即可；（没有其他更好的方法了）

## 保持良好的习惯，反正commit又不花钱，还可快速回到修改后的状态
必须记得git add .
必须记得git commit -m


