# keycap - 400
This challenge also suffers from poor flag formatting. But, I solved it very fast because I recognized the main idea from a previous CTF.

# Prompt


![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/key2.PNG "keycap")

# Guide

Okay, so we download this pcap and it looks strange.


![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/key1.PNG "keycap")

Certainly not a regular pcap file. It looks like usb data. For me this was a lightbulb, as this type of pcap challenge is all too common. I knew right away it was from traffic from a keyboard. 

Instead of writing our own python script, let's see if we can't find someone that has done the work for us already. 

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/key3.PNG "keycap")


Perfect. The link we are trying to use is here, huge thanks to this github user.

https://dbaser.github.io/2017/04/27/picoctf-2017-for80-just_keyp_trying/

After running his python script like the script kiddies we are, we get this.


![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/key4.PNG "keycap")

Confused? You should be. What the hell is this?

`FLAAG[OOMG-HHOW-DIID-TTHHIIS-GEET-HERRE-I-CCANT-COOMMPUTEER-GOOD111]`

After maybe 40 minutes of mangling the flag, my teammate and I figured out it was 

**flag{omg_how_did_this_get_here_I_cant_computer_good!!!}**

***Disclaimer***
My apologies that we ended up using someone else's solution to a similar challenge, and again a huge thanks to https://dbaser.github.io/2017/04/27/picoctf-2017-for80-just_keyp_trying/ for their script.

Usually, I would provide my own script but because of my previous exposure to challenges similar to these I figured I couldn't put together a script without ripping from the original scripts I had seen and deferred to using their scripts and giving the credit due.

In a pure CTF scenario however, You should use anything you can get yours hands on.
