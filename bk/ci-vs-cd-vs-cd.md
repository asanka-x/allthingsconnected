---
layout: post
title: CI vs CD vs CD
date: 2013-01-24
tags: ["Concepts","devops","process","software engineering"]
---

<div>That said, to judge by the Humble/Farley book the distinction between Continuous Delivery and Continuous Deployment is just a little blurred. The authors acknowledge that continuous deployment into production is not always a good idea. They also imply that Continuous Deployment might mean only that your application is always ready and easy to deploy into production, not that you necessarily deploy it constantly:</div>
> <div>Your implementation should make it possible to deploy any version of your application that has made it past the automated tests into any of your environments at the push of a button, given the correct credentials.</div>
<div>Compliance and security are also factors that may rightly make it impossible to automate deployment to production completely.</div>
<div>Client-installed applications present some special difficulties which Humble and Farley discuss.</div>
<div>In summary then:</div>
<div>**Continuous integration**: your application always builds and passes its tests, including all the pieces from different sub-teams.</div>
<div>**Continuous delivery**: your application always builds and deploys to a test environment and passes its tests.</div>
<div>**Continuous deployment**: your application is always ready to deploy to production through a largely automated process.</div>
<div>**Update**: I received an email from Martin Fowler about this post. He refers to Jez Humble's post on [Continuous Delivery vs Continous Deployment](http://continuousdelivery.com/2010/08/continuous-delivery-vs-continuous-deployment/) and adds:</div>
> <div>- I would use your definition of Continuous Deployment for Continuous Delivery</div>> 
> <div>- I would change the definition of Continuous Deployment to say something like "every good build is released to production"</div>