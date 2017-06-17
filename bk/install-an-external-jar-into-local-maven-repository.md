---
layout: post
title: Install an external jar into local Maven repository
date: 2013-01-16
tags: ["Linux","Maven","Tutorials"]
---

## 

<div>
<div>Sometimes, you project will have dependency on a jar which is not in official maven repository, and maybe it is propriety jar file which will never be part of maven repository. In this case, you have to put it to your local repository your self to solve the dependency.</div>
<div>There is a install plug in to do this job, which is something like:</div>
<pre>mvn install:install-file -DgroupId=  
-DartifactId=  
-Dversion=  
-Dfile=  
-Dpackaging=jar 
-DgeneratePom=true</pre>
<div>For example, you want to install the danga's memcached client plugin, you can do:</div>
<pre>mvn install:install-file -DgroupId=com.danga 
-DartifactId=memcached 
-Dversion=2.0.1 
-Dfile=java_memcached-release_2.0.1.jar 
-Dpackaging=jar 
-DgeneratePom=true</pre>
<div>This will add the memcache jar into your local Maven2 repository under groupId com.danga and artifactId memcached, you can then edit your pom.xml adding this dependency.</div>
<div>However, the maven eclipse can not recognize it since it always search from public repository.</div>
</div>