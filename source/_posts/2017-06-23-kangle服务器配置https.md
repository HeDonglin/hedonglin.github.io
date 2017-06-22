---
title: kangle服务器配置https
date: 2017-06-23 01:48:31
categories: 服务器
tags: kangle
---
## 使用netstat -nap 命令查看服务器端口是否被占用，并且设置网站的端口
一般情况下不会被占用的，但是如果你是设置了VPN(如搬瓦工)它会默认采用443端口的；
在这里设置后easypanel管理面板才会显示SSL标志
<img src="/images/kangle-1.png" alt="kangle-1.png" />
<img src="/images/kangle-2.png" alt="kangle-2.png" />
## 申请免费SSL
<https://cloud.tencent.com/product/ssl?fromSource=gwzcw.231631.231631.231631>
<img src="/images/kangle-4.png" alt="kangle-4.png" />
<img src="/images/kangle-5.png" alt="kangle-5.png" />
<img src="/images/kangle-6.png" alt="kangle-6.png" />
<img src="/images/kangle-7.png" alt="kangle-7.png" />
<img src="/images/kangle-8.png" alt="kangle-8.png" />
## kangle服务器使用的是用到Nginx格式的公钥和私钥
公钥：.crt
私钥：.key
<img src="/images/kangle-3.png" alt="kangle-3.png" />
<img src="/images/kangle-9.png" alt="kangle-9.png" />
## 设置完后重启kangle服务器
<img src="/images/kangle-10.png" alt="kangle-10.png" />
<img src="/images/kangle-11.png" alt="kangle-11.png" />
## 查看是否被侦听状态
<img src="/images/kangle-12.png" alt="kangle-12.png" />

