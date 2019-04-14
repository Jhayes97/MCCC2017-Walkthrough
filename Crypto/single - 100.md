# single - 100
This challenge was not ideal to do by hand, as you're looking at about 256 possibilities. Let's put our python chops to the test.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/sin1.PNG "single")


# Guide

Ok, let's make a python script that will automate all of that tedious work for us.

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/sin2.PNG "single")

You can see that we're using a for loop to iterate through every possible xor in range chr(256), or all ascii characters. If the first 4 letters of the decoded message == "flag", then we have the script print out the full result


![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/sin3.PNG "single")


There we go, there's our flag.

**flag{the_xor_basis_of_all_crypto}**

