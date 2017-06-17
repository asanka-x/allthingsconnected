---
title: Useful GNU/Linux commands
date: 2013-02-08
layout: Post
link: http://asankan.info/2013/02/08/useful-gnulinux-commands/
author: asankanissanka
description: 
post_id: 61
created: 2013/02/08 04:11:00
created_gmt: 2013/02/08 04:11:00
comment_status: open
post_name: useful-gnulinux-commands
status: publish
post_type: post
---

# Useful GNU/Linux commands

**To find groups that a user belong** **               **~$ id -nG _        Output_ group1 group2 group3 **To remove user from a particular group** Ex :- To remove above user from group1 

              ~$ usermod -G group2,group3

**To unlock dpkg** ~$ sudo fuser -vki /var/lib/dpkg/lock ~$ sudo dpkg --configure -a ** **** ****Connect to Amazon EC2 instance via terminal** ** ****            **  ~$ ssh -i username@public-dns 

** **** **