---
title: Install an external jar into local Maven repository
date: 2013-01-16
layout: Post
link: http://asankan.info/2013/01/16/install-an-external-jar-into-local-maven-repository/
author: asankanissanka
description: 
post_id: 65
created: 2013/01/16 11:09:00
created_gmt: 2013/01/16 11:09:00
comment_status: open
post_name: install-an-external-jar-into-local-maven-repository
status: publish
post_type: post
---

# Install an external jar into local Maven repository

## 

Sometimes, you project will have dependency on a jar which is not in official maven repository, and maybe it is propriety jar file which will never be part of maven repository. In this case, you have to put it to your local repository your self to solve the dependency.

There is a install plug in to do this job, which is something like:
    
    
    mvn install:install-file -DgroupId=  
    -DartifactId=  
    -Dversion=  
    -Dfile=  
    -Dpackaging=jar 
    -DgeneratePom=true

For example, you want to install the danga’s memcached client plugin, you can do:
    
    
    mvn install:install-file -DgroupId=com.danga 
    -DartifactId=memcached 
    -Dversion=2.0.1 
    -Dfile=java_memcached-release_2.0.1.jar 
    -Dpackaging=jar 
    -DgeneratePom=true

This will add the memcache jar into your local Maven2 repository under groupId com.danga and artifactId memcached, you can then edit your pom.xml adding this dependency.

However, the maven eclipse can not recognize it since it always search from public repository.

## Comments

**[traffic](#32 "2013-06-04 09:39:19"):** Thank you ever so for you post.Much thanks again. Cool.

**[space jam jordans for sale](#33 "2013-06-11 17:42:01"):** “I expect that the design of the OS will be much more minimal and cleaner with most, if not all, of the skeuomorphism gone from the OS. There will be additional functionality as new APIs are incorporated into the release, but the focus will be on the look and feel of the user experience,” Baker said.

**[abercrombie](#34 "2013-08-08 22:05:47"):** Install an external jar into local Maven repository | Asanka's Blog... [abercrombie femme](http://2013abercrombiekids.webs.com/http://2013abercrombiefitch.webs.com/)

