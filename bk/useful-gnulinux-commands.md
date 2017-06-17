---
layout: post
title: Useful GNU/Linux commands
date: 2013-02-08
tags: ["commands","Linux","terminal","Tutorials"]
---

**To find groups that a user belong**

**               **~$ id -nG

_        Output_

group1 group2 group3

**To remove user from a particular group**

Ex :- To remove above user from group1
<div>              ~$ usermod -G group2,group3</div>
**To unlock dpkg**

~$ sudo fuser -vki /var/lib/dpkg/lock

~$ sudo dpkg --configure -a
**
****
****Connect to Amazon EC2 instance via terminal**
**
****            **  ~$ ssh -i username@public-dns
<div></div>
**
****
**