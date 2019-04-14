# NetworkTools - 200
This challenge tripped me up for a little bit. It's one of those where you have a "duh!" moment.

# Prompt 

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/nwt1.PNG "NetworkTools")



# Guide

First thing let's look at the website.


![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/nwt2.PNG "NetworkTools")


You can try to use the ping/hostname tools, but they don't really do anything. 

After playing around the website for a long time, I wondered how exactly it was sending pings.


What would happen if you fuzzed the user input boxes?

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/nwt3.PNG "NetworkTools")

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/nwt4.PNG "NetworkTools")

We have command injection!

Let's see what running `google.com; ls` brings up

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/nwt5.PNG "NetworkTools")

There is a flag.txt, can we run `google.com;cat flag.txt`?

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/nwt6.PNG "NetworkTools")

Got it! our flag is 

**flag{tp_link_d_link_theyre_all_the_same}**
