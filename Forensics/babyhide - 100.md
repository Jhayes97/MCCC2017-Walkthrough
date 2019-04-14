# babyhide - 100
As a low level steganography question, there are only so many things it could be. I saved you the time and only show the actual method.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/bb1.PNG "Obey me, poison")

# Guide

Skipping over the other possibilities for a low level Steg challenge, I'll take you straight to the meat of it.

Using binwalk we are able to see if any additional files have been tacked on to the end of this image, and actually, there is!

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/bb2.PNG "Obey me, poison")

We then extract the pdf using `foremost` or `binwalk -e` and open up the PDF


![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/bb3.PNG "Obey me, poison")

There's our flag.

**flag{baby_come_back}**
