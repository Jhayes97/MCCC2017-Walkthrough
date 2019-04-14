# festivus - 100
This challenge is a pdf crack. The wordlist is small enough that we could do it manually, but we'll use our big CTF brains.

# Prompt

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/fes1.PNG "festivus")


# Guide 

It looks like we're going to have to use JtR to crack the pdf. Natively JtR doesn't support PDF, but using the community jumbo version, we can use pdf2john to turn the locked pdf into a hash, and feed the hash to john.

We could use the wordlist provided, but John itself uses a wordlist which I'd bet every word on the provided list is represented.

After downloading Jumbo John, or the individual pdf2john python script, let's put pdf2john to work.

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/fes2.PNG "festivus")

We store the hash inside of hash.txt, and feed that txt file to John

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/fes3.PNG "festivus")

Using the `-show` option, we get the password!

Now let's open the pdf with the password we cracked, and get our flag!

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/fes4.PNG "festivus")

**flag{f371vu5_f0r_7h3_r357_0f_u5}**
