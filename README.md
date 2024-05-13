# AWS-Cloud-Server

My first project...  AWS Cloud Server
﻿

Well, my Google drive is at 99% full and has been for quite some time. While doing the learning in the Coursera Google course, I figured I would also do some hands on stuff to train skills also. My first task, AWS Web-server. I found a walk through on YouTube from NetworkChuck . I followed this guide to use as a ‘Guided Project’. I decided on this project as it incorporates a few things that I have no experience in, AWS, and SSL. I also added my own level of difficulty by using Ubuntu as the main platform of use.

The walk-through was fairly straightforward, and easy to follow along with as far as the web based set up. I changed a few things though. My S2 server was not a T2.medium. I chose the T2 micro because I will not use this service often personally, so the cost involved with the difference had no value.

I did have a few ‘teaching moments’ throughout this project. Somehow I did not set up my S2 server with enough disk space. So, create new server and delete the old. And wouldn’t you know… I did it twice. Third times a charm! Then, the S3 bucket, again… third times a charm. With the bucket, I kept getting an error in Filecloud when switching to the S3 bucket, after trying a couple of time, I tried entering in the region, and low and behold, it worked. Filecloud has this as an optional setting, however, for me, it was required. I figured this out after creating 3 different buckets thinking that I messed something up in the creation. Low and behold, it was just an optional setting that was mandatory.

Then getting filesync installed on Linux so I could perform file transfers in OS. Here is a screen shot from the Filecloud website. But there is no documentation on how to actually run the program.

I, for the life of me could not get filecloud to fire up. ./filecloud, nope, GUI, none. So, off to Google I go. And I come across this github file  and man, did this work. Big shout out to Derek Shnosh! After reading and looking at things, apparently the issues are that the files needed are not set as executable, and I didn’t know where they were stored, but this script took care of those issues.

This was my very first experience with all of these services, AWS, Filecloud, and Cloudflare, and was also my first time imposing an SSL certificate. I can say, this, this right here, the tinker until it works is so very intriging to me. Its the reason that I have done this type of stuff as a hobby before. And now learning that people get paid for this, with other skill sets of course. And man, I can’t wait until my next physical project. I have a list of training ‘box’ projects to do, so I have some time to think about a physical one, but I think it will be a NAS for the house.

﻿
