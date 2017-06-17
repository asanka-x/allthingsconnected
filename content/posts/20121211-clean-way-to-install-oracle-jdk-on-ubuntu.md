---
title: Clean way to install Oracle JDK on ubuntu
date: 2012-12-11
layout: Post
link: http://asankan.info/2012/12/11/clean-way-to-install-oracle-jdk-on-ubuntu/
author: asankanissanka
description: 
post_id: 7
created: 2012/12/11 19:20:00
created_gmt: 2012/12/11 19:20:00
comment_status: open
post_name: clean-way-to-install-oracle-jdk-on-ubuntu
status: publish
post_type: post
---

# Clean way to install Oracle JDK on ubuntu

There are several ways to install JDK on linux and there are several JDK versions available for ubuntu. But as my personal choice I would prefer Oracle JDK the most.  
  
Basically there are two main ways to install JDK on ubuntu  
Download JDK linux package and install it  
Add the repository containing oracle JDK packages and install using "apt-get"  
  
I'll be focusing on the second method since it's a more clean way to install, that it will install the packages to the most suitable locations. Obviously we can install it to our preferred location following the first method but if we are configuring a production server it is recommended to follow the standard locations to which the JAVA like environments should be installing.  
  
This is all you have to do (See this is simpler than the first method)  
  
  
    sudo add-apt-repository ppa:webupd8team/java  
    sudo apt-get update  
    sudo apt-get install oracle-java7-installer