---
title: Android Wireless Debugging
date: 2013-11-15
layout: Post
link: http://asankan.info/2013/11/15/android-debugging-over-lanwifi/
author: asankanissanka
description: 
post_id: 76
created: 2013/11/15 04:21:53
created_gmt: 2013/11/15 04:21:53
comment_status: open
post_name: android-debugging-over-lanwifi
status: publish
post_type: post
---

# Android Wireless Debugging

If you are a mobile app developer, you surely have noticed that it's a burden to debug having connected your device via a USB cable. And it's a waste if your PC has only few USB ports. So anyways there is a cool solution for this. If both your PC and your android device are connected to a wireless network (should be in same network), you can debug your device wireless. **Step 1** Connect your device to your PC via a USB connection (Make sure USB debugging is on) **Step 2** Go to your android platform-tools directory and open a command window and run 
    
    
                   adb tcpip 5555
                   adb connect <Device IP>:5555

**Step 3** Disconnect USB connection. Now you can debug your device wireless, you can run "adb logcat" and check whether it's working. To switch back to USB run the following command 
    
    
                   adb usb