# galaxy - 300
This challenge was cool initially, but a bit confusing midway through. That probably just falls on me.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gal1.PNG "galaxy")


# Guide

Okay, so we're given a disk image. Let's go ahead and mount that.

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gal2.PNG "galaxy")

It looks like a bunch of junk, let's just run strings on every item and grep for 'flag'.

I'll save you the misses and show you the win, after running strings on the pdf and grepping for 'flag', we get

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gal3.PNG "galaxy")

**flag{forgot_my_flash_drive_on_egos_planet}**
