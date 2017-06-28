---
title: Centos如何升级最新的git
date: 2017-06-23 02:23:44
categories: 服务器
tags: Centos
---
## 安装编译git时需要的包（重要）
yum install curl-devel expat-devel gettext-devel openssl-devel zlib-devel
yum install  gcc perl-ExtUtils-MakeMaker

## 删除已有的git
yum remove git

## 下载git源码
cd /usr/src
wget https://www.kernel.org/pub/software/scm/git/git-2.9.4.tar.gz
tar xzf git-2.9.4.tar.gz

## 编译安装（一行一回车）
cd git-2.9.4
make prefix=/usr/local/git all
make prefix=/usr/local/git install
echo "export PATH=$PATH:/usr/local/git/bin" >> /etc/bashrc
source /etc/bashrc

## 检查一下版本号
git --version
显示为：git version 2.9.4

## 把在服务器生成的公钥放到github上

## 汇总
```js
yum install curl-devel expat-devel gettext-devel openssl-devel zlib-devel
yum install  gcc perl-ExtUtils-MakeMaker
yum remove git
cd /usr/src
wget https://www.kernel.org/pub/software/scm/git/git-2.9.4.tar.gz
tar xzf git-2.9.4.tar.gz
cd git-2.9.4
make prefix=/usr/local/git all
make prefix=/usr/local/git install
echo "export PATH=$PATH:/usr/local/git/bin" >> /etc/bashrc
source /etc/bashrc
git --version
cd ~
ssh-keygen -t rsa -C "你的邮箱@163.com"
```
