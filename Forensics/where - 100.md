# where - 100
By far my least favorite problem. The goal was clear, but flag formatting was a bit of a recurring issue in this competition, which I'm glad they fixed in the later MCCC1

# Prompt

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/whe1.PNG "where")

# Guide
Based on the prompt, we can assume there are artifacts of the image location left in the EXIF data.
We could use  the `exiftools` command, or we could use google and save ourselves a google steps. If it were a live competition you'd want to go with the fastest method, so let's pretend we're under the heat of time and use google.

Using one of the first results for 'exif tool online', we plug in our image.

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/whe2.PNG "where")

Now let's throw those coordinates into google maps

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/whe3.PNG "where")

This looks nothing like a flag. Based on the prompt let's search for parks nearby.

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/whe4.PNG "where")

Believe it or not, there is your flag.

`killarney national park`

Not a great challenge, and there was zero indication for an atypical flag format. Sucks. However they did fix most of these issues in their later CTF.

