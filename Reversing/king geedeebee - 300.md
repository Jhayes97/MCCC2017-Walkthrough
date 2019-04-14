# king geedeebee - 300
This challenge was a fun one, it held the obfuscated flag inside, and held a secret to it. 

# Prompt

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gdb1.PNG "geedeebee")

# Guide
If you weren't aware, geedeebee is a reference to the GNU Debugger, or gdb. I run gdb with a helpful add-on called peda, so we'll be working with that.

Before I go into any mid-level RE challenge, I like to throw it into Ghidra and see exactly what I'm dealing with.


## Initial Ghidra inspection

We load the binary into Ghidra and navigate to the main() function.

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gdb3.PNG "geedeebee")


In the decompiled function it looks like it's storing our flag obfuscated in the variables, and then XOR'ing it with 0x32, let's convert some of this into ascii.

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gdb2.PNG "geedeebee")

We see it XORs our flag with the ascii number '2' and we can see our obfuscated flag, but it would be annoying to do it all by hand. Let's view it from the stack as it loads it into memory with gdb-peda.

## Viewing the stack with gdb-peda

We start gdb by setting a breakpoint at main, and strolling through a couple of the initial instructions until we can see something being written onto the stack

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gdb4.PNG "geedeebee")

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gdb5.PNG "geedeebee")
`]^SUIY[@PKmS[\\FmUTFm\\]FZ[\\Um]\\m_W}`
It looks like we have something on the stack here, and I'd bet that's our flag.



## Xor the string with our gained knowledge.

Let's XOR it with `2` and see if that brings anything back for us

![alt text](https://github.com/Jhayes97/MCCC2017-Walkthrough/blob/master/src/gdb6.PNG "geedeebee")


That looks like our flag. Correcting for some minor errors we get

**flag{kirby_aint_got_nothing_on_me}**

