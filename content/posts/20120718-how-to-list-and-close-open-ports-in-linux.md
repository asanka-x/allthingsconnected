---
title: How to list and close open ports in linux
date: 2012-07-18
layout: Post
link: http://asankan.info/2012/07/18/how-to-list-and-close-open-ports-in-linux/
author: asankanissanka
description: 
post_id: 19
created: 2012/07/18 03:38:00
created_gmt: 2012/07/18 03:38:00
comment_status: open
post_name: how-to-list-and-close-open-ports-in-linux
status: publish
post_type: post
---

# How to list and close open ports in linux

This guide will be demonstrating you how to get the status of the ports and to free up a port which is in use.  
_(Note : Following commands were tested on a ubuntu 11.10 installed pc)_  
_  
_  
List down all listening ports  
**netstat -lpn**  
  
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name  
_tcp        0      0 0.0.0.0:49027                          0.0.0.0:*                LISTEN      13098/java   _  
_tcp        0      0 127.0.0.1:9160                        0.0.0.0:*                LISTEN      13098/java   _  
_tcp        0      0 127.0.0.1:3306                        0.0.0.0:*                LISTEN      -           _  
_tcp        0      0 0.0.0.0:8080                            0.0.0.0:*                LISTEN      13098/java   _  
_tcp        0      0 0.0.0.0:33395                          0.0.0.0:*                LISTEN      13098/java   _  
_tcp        0      0 127.0.0.1:631                          0.0.0.0:*                LISTEN      -           _  
_tcp        0      0 127.0.0.1:7000                        0.0.0.0:*                LISTEN      13098/java _  
  
  
Use grep for filtering out the 8080 port.  
  
You can use following command:  
**netstat -lpn | grep 8080**  
  
You'll get output something like this  
  
_tcp        0      0 0.0.0.0:8080            0.0.0.0:*               LISTEN      13098/java_  
  
Here my process id is 13098 and it is the process that is using port 8080  
  
Kill the process using following command:  
**sudo kill 13098**  
  
Now port 8080 is free.