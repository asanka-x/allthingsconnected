---
title: Processing Multi-Stage Tasks using Firebase Queue
date: 2016-08-23
layout: Post
link: http://asankan.info/2016/08/23/processing-multi-stage-tasks-using-firebase-queue/
author: asankanissanka
description: 
post_id: 180
created: 2016/08/23 23:54:55
created_gmt: 2016/08/23 18:24:55
comment_status: open
post_name: processing-multi-stage-tasks-using-firebase-queue
status: publish
post_type: post
---

# Processing Multi-Stage Tasks using Firebase Queue

This is an implementation of [Pipes and Filter Pattern](https://msdn.microsoft.com/en-us/library/dn568100.aspx) which is a commonly used [Cloud Design Pattern](https://msdn.microsoft.com/en-us/library/dn568099.aspx). The most common approach to implement this pattern is via multiple queues as shown in the following figure.

![ic709558](https://asankanissanka.files.wordpress.com/2016/08/ic709558.png)

###### Pipeline Using Multiple Queues ([Ref : MSDN](https://msdn.microsoft.com/en-us/library/dn568100.aspx))

The prosed solution here uses a bit different approach than above and use a single queue instead of multiple queues as shown below.

![Data Flow Diagram](https://asankanissanka.files.wordpress.com/2016/08/data-flow-diagram.png)

###### Pipeline Using a Single Queue

To practically implement a solution like above the common approach would be to maintain a state for each queue message and assign a state for each workers(filters) to filter the messages accordingly before execution. However recently when I was trying out [Firebase Realtime Database](https://firebase.google.com/docs/database/) I found [Firebase Queue](https://github.com/firebase/firebase-queue) which is a queue implementation on top of the Firebase Realtime Database and it turned out that it comes with a out of the box solution for maintaining a state (their term is [specs](https://github.com/firebase/firebase-queue/blob/master/docs/guide.md#defining-specs-optional)) for queue messages as described above. So I worked on a PoC to evaluate this and in my personal opinion it's really cool. But this is not enough to make a dicission so I was looking at various benefits we can achieve here with the usage of [Firebase Realtime Database](https://firebase.google.com/docs/database/).

### Benefits

  * Using firebase realtime behaviour we can easily show the progress of the running tasks on a front-end
  * Since it's single queue it's less hazzle to implement and maintain
  * Uses push instead of polling to notify workers about new tasks
  * Implementation has been made super easy with their library
  * Nicely support to be run in a clustered environment distributing workload among nodes

### Use Cases

  * In scenarios where REST APIs facilitate time consuming processing heavy back­end functions
  * In scenarios where triggered background tasks run for streaming data