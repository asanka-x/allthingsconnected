---
title: CI vs CD vs CD
date: 2013-01-23
layout: Post
link: http://asankan.info/2013/01/23/ci-vs-cd-vs-cd/
author: asankanissanka
description: 
post_id: 62
created: 2013/01/23 20:11:00
created_gmt: 2013/01/23 20:11:00
comment_status: open
post_name: ci-vs-cd-vs-cd
status: publish
post_type: post
---

# CI vs CD vs CD

That said, to judge by the Humble/Farley book the distinction between Continuous Delivery and Continuous Deployment is just a little blurred. The authors acknowledge that continuous deployment into production is not always a good idea. They also imply that Continuous Deployment might mean only that your application is always ready and easy to deploy into production, not that you necessarily deploy it constantly:

> Your implementation should make it possible to deploy any version of your application that has made it past the automated tests into any of your environments at the push of a button, given the correct credentials.

Compliance and security are also factors that may rightly make it impossible to automate deployment to production completely.

Client-installed applications present some special difficulties which Humble and Farley discuss.

In summary then:

**Continuous integration**: your application always builds and passes its tests, including all the pieces from different sub-teams.

**Continuous delivery**: your application always builds and deploys to a test environment and passes its tests.

**Continuous deployment**: your application is always ready to deploy to production through a largely automated process.

**Update**: I received an email from Martin Fowler about this post. He refers to Jez Humble’s post on [Continuous Delivery vs Continous Deployment](http://continuousdelivery.com/2010/08/continuous-delivery-vs-continuous-deployment/) and adds:

> \- I would use your definition of Continuous Deployment for Continuous Delivery
> 
> \- I would change the definition of Continuous Deployment to say something like "every good build is released to production"

## Comments

**[http://camdentonteaparty.org](#28 "2013-07-24 22:35:18"):** The following blog post, “CI vs CD vs CD | Asanka's Blog...” indicates the fact that u comprehend what precisely you are communicating about! I actually entirely agree with your post. Many thanks ,Roseanne

**[Massage](#29 "2013-08-07 15:20:47"):** Thanks so much for the blog article. Fantastic.

**[Daniel Beaulieu](#30 "2013-08-10 03:58:25"):** **Daniel Beaulieu...** I value the blog article.Really thank you!...

**[Massage](#31 "2013-08-15 08:21:06"):** A spherical of applause for your blog post. Amazing.

