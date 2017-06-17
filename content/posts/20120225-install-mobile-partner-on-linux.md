---
title: Install Mobile Partner on linux....
date: 2012-02-25
layout: Post
link: http://asankan.info/2012/02/25/install-mobile-partner-on-linux/
author: asankanissanka
description: 
post_id: 21
created: 2012/02/25 05:04:00
created_gmt: 2012/02/25 05:04:00
comment_status: open
post_name: install-mobile-partner-on-linux
status: publish
post_type: post
---

# Install Mobile Partner on linux....

I think all of the Huawei mobile partner modems are automatically detected by Ubuntu 10.10 or higher, we just have to plug and play. But we can't send/receive SMSs or use data counter (Statistics) since the modem is detected and configured by network manager, so we don't get a GUI for mobile partner.  
  
If you want get the GUI you can download the driver from link bellow.  


  
[Download GUI Mobile Partner driver](http://www.mediafire.com/?j3a63cq1p4847tp)  
  
It's work for CDMA and GSM modems. After downloading the driver, follow this instruction to install it  
  
1.) Extract the downloaded file

                    Use your preferred tool to extract the zip file

  


2.) Open a terminal and type

  


                    cd /Linux # Goto extracted directory & open Linux folder

                    sudo chmod -R 777 install # Give execute permission

                    sudo ./install # Run "install" shell script

  


3.) Press enter when you get noticed please input the absolute path for install, the installation file will be placed on default path

  


![](http://asankanissanka.files.wordpress.com/2012/02/installmobilepartner1.png?w=300)

  


  
Wait untill installation progress is finished. After that, when you plug the modem, the GUI for mobile partner will be automatically open. And now you can use the GUI for short messaging and data counting.  


![](http://asankanissanka.files.wordpress.com/2012/02/installmobilepartner31.png?w=300)

## Comments

**[bckurera](#1 "2012-03-08 03:22:09"):** yeah this(Safaricom) works for Fedora as well. But I nt supported for my Fedora 15, 64bit !!But doing well with 32bits.

**[Asanka Nissanka](#2 "2012-03-08 03:47:33"):** I couldn't try this on a 64-bit version. So thanks for mentioning that. Anyways some of the dongles (Like Dialog dongles) come along with the linux mobile partner.

**[mpe](#3 "2012-09-02 14:46:46"):** thanks mate.... it's working

**[Asanka Nissanka](#4 "2012-09-02 17:20:50"):** You are welcome bro !!!! And thank you for the feedback :)

**[pushpikede](#6 "2012-11-11 14:53:55"):** This does not work in my system. Installing this software made xubuntu unable to detect my Huawei e156g which was working flawlessly ever before. It was very difficullt to remove the software and even after removing it, my system failed to detect the dongle. I had to underwent a really hard time to get it back to work.  
Beware that this is not a normal Ubuntu software and installing it will change a few of your system files which would be very difficult to reset. Before installing this check whether your dongle is supported.

**[Anonymous](#7 "2012-12-02 17:52:21"):** can u upload drivers for 64-bit also?

**[Asanka Nissanka](#8 "2012-12-02 18:17:22"):** well I don't have drivers for 64-bit at the moment but I'll give it a try, Anyways thank you for your interest

**[linux](#10 "2013-05-17 00:51:55"):** I am no longer positive the place you are getting your information, however great topic. I must spend a while finding out more or understanding more. Thanks for great information I used to be looking for this information for my mission.

**[Sherrill](#11 "2013-05-29 17:00:08"):** I came to your "Install Mobile Partner on linux&" page and noticed you could have a lot more traffic. I have found that the key to running a website is making sure the visitors you are getting are interested in your subject matter. There is a company that you can get traffic from and they let you try it for free. I managed to get over 300 targetted visitors to day to my website. Visit them today: http://nsru.net/fdse

**[Hammock](#12 "2013-06-13 22:30:19"):** I do not possibly understand how I ended way up below, however imagined this set up once were terrific. I wouldn't realize who you might be even so undoubtedly ensure some sort of well-known blog writer in the event you are certainly not by now. Cheers!

**[iherb coupons](#13 "2013-08-20 23:30:56"):** Good day! I simply wish to give you a big thumbs up for your great information you've got right here on this post. I am coming back to your site for more soon.

