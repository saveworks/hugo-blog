---
date: "2020-10-22T07:35:57+08:00"
draft: false 
title: "Github添加sshkeys"
tags: ["git","github"]
series: ["github"]
categories: ["github"]
img: 
summary: "初始篇"
toc: true


---

## linux 服务器和github
1. linux 生成ssh key
```
$ssh-keygen -t rsa -b 4096 -C "you@email.com"
```
一路回车
```
enerating public/private rsa key pair.
Enter file in which to save the key (/home/revin/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/revin/.ssh/id_rsa.
Your public key has been saved in /home/revin/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:G1SjKGLsGi7ieerKGe+PutJHKBvrXwqUEiX4JEuUMS4 saveworks@163.com
The key's randomart image is:
+---[RSA 4096]----+
|+++       o      |
|+*o    . o .     |
|E*+ . . o        |
|o+o. . .         |
|oo..    S        |
|*o. .    o       |
|+X . .  .        |
|O B.=            |
|*@BB..           |
+----[SHA256]-----+


```
2. 生成ssh key后,添加到githubz中

3. 检查linux 和服务器端是否一致 
```
ssh-add l
```
4. 测试
```
ssh -T git@github.com
```








## 版本控制

| Version | Action                   | Time       |
| ------- | ------------------------ | ---------- |
| 1.0     | Init                     | 2020-10-22T07:35:57+08:00|
