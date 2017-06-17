---
layout: post
title: Android Wireless Debugging
date: 2013-11-15
tags: ["android","debugging","mobile","Tutorials"]
---

If you are a mobile app developer, you surely have noticed that it's a burden to debug having connected your device via a USB cable. And it's a waste if your PC has only few USB ports. So anyways there is a cool solution for this.

If both your PC and your android device are connected to a wireless network (should be in same network), you can debug your device wireless.

<span style="text-decoration:underline;">**Step 1**</span>

Connect your device to your PC via a USB connection (Make sure USB debugging is on)

<span style="text-decoration:underline;">**Step 2**</span>

Go to your android platform-tools directory and open a command window and run
<pre>               adb tcpip 5555
               adb connect <Device IP>:5555</pre>
<span style="text-decoration:underline;">**Step 3**</span>

Disconnect USB connection. Now you can debug your device wireless, you can run "adb logcat" and check whether it's working.

To switch back to USB run the following command
<pre>               adb usb</pre>