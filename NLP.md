# Chapter 2: Binary & Data Representation

In this chapter, you’ll learn how information is represented inside the computer:

### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `1. Binary System.`
### ![#1589F0](https://placehold.it/15/1589F0/000000?text=+) `2. Data representation in binary.`
### ![#ff00ff](https://placehold.it/15/ff00ff/000000?text=+) `3. KiloByte, MegaByte, GigaByte, TeraByte.`

# `1. Binary System`

`Binary` is a `base 2` number system invented by Gottfried Leibniz that is made up of only two numbers: `0` and `1`. You may
have heard that computers work on ones and zeros. But almost nobody today actually deal directly with these ones and zeros,
but ones and zeros do play a big role in how computers work on the inside. 

<p align="center">
   Figure 1: Binary
</p>

<p align="center">
  <img height="300" width="400" src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/binary.jpg" alt="Binary"/>
</p>

Inside a computer are electric wires and circuits and carry all the information in a computer. 

<p align="center">
   Figure 2: Wire & Circuits
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/wc.png" alt="Binary"/>
</p>

How do the computers store or represent information using electricity? Well, if you have a single wire with electricity
flowing through it. The signal can either be on or off. That’s not a lot of choices. but it’s a really important start. With
one wire, you can represent a ‘yes’ or a ‘no’. true or false, a one or a zero. or anything else with only two options. This
on/off state of a single wire is called a bit. 

### A `bit` (short for binary digit) is the `smallest` unit of information the computer can store. A bit has a single binary value, either 0 or 1.

<p align="center">
   Figure 3: Bit: Zero and One
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/b2.png" alt="Binary"/>
</p>

<p align="center">
   https://delightlylinux.wordpress.com/2014/09/05/binary-lesson-7-bits-and-bytes/
</p>

If you use more wires, you get more bits. More ones and zeros with more bits. You can represent more complex information. But
to understand that, we need to learn about something called about the `binary` number system.

In the decimal number system, we have 10 digits from zero to nine. And that’s how we’ve all learned to count. 

# How do we count in Decimal (base 10)?

* `0`   Start at 0
* ...	  Count 1,2,3,4,5,6,7,8, and then...
* `9`	  This is the last digit in Decimal
* `10`  So we start back at 0 again, but add 1 on the left
* ...	  Count 11,12,13,14,15,16,17,18,19,20,21,22,...,97,98 and then...
* `99`  When we run out of digits, we ...
* `100` ... start back at 0 again, but add 1 on the left

In decimal number system, there’s the 1s position, the 10s position, the 100s position, and so on. For example, a three in the
100 position is a 300.

<p align="center">
   Figure 4: Three hundred and twenty seven
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/327.png" alt="Binary"/>
</p>

<p align="center">
   https://www.mathsisfun.com/decimals.html
</p>

In the binary number system, we only have two digits, zero and one. With these two digits, we can count put to any number.
Here’s how this works.

# How do we count in Binary?
	 	 
* `0`   Start at 0
* `1`	  Then 1
* `10`  Start back at 0 again, but add 1 on the left
* `11`	 	 
* `100` Start back at 0 again, and add one to the number on the left... <br/>
        ... but that number is already at 1 so it also goes back to 0 ... <br/>	
        ... and 1 is added to the next position on the left <br/>
* `101`	 	 
* `110`	 	 
* `111`	 	 
* `1000` Start back at 0 again (for all 3 digits), add 1 on the left
* `1001`	And so on!

In binary, each position also carries a value, but instead of multiplying by 10 each time, you multiply by two. there’s 1
poison, 2 position, 4 position, 8 position, and so on.

<p align="center">
   Figure 5: Binary to Decimal
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/b2d.png" alt="Binary"/>
</p>

<p align="center">
https://ncalculators.com/number-conversion/binary-to-decimal-hexa-octal-converter.htm
</p>

For example, the number nine in binary is 1001. Almost nobody does this math because computer do it for us. What’s important
is that any number can be represented with only ones and zeros. or by a bunch of wires that are on or off. The more wires use,
the larger the numbers you can store.

<p align="center">
   Figure 6: Binary and Decimal equivalents of 0 to 15
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/bd.png" alt="Binary"/>
</p>

With eight wires, you can store numbers between 0 and 255. That’s eight bits. 

## In most computer systems, a `byte` is a unit of data that is eight binary digits.

<p align="center">
   Figure 7: Byte
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/bit.jpg" alt="Byte vs Bit"/>
</p>

With just 32 wires, you can store all the way from zero to over four billion. Using the binary number system, you can 
represent any number you like. But what about other types of information? Like text, image, or sound? It turns out that all 
these things can also be represented with numbers.

# `2. Data Representation in Binary`

### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Text in Binary` 

Think of all the letters in the alphabet. You could assign a number to each letter. “A” could be “65”, “B” could be
“66”, and so on. You can then represent any word or paragraph as a sequence of numbers, and as we saw, these numbers
can be stored as on or off electrical signals. Every word you see on every webpage or your phone is represented using
a system like this.
	
ASCII is an abbreviation for American Standard Code for Information Interchange. ASCII is a table of characters for
computers. It is binary code used by electronic equipment to handle text using the English alphabet, numbers, and
other common symbols. 

<p align="center">
   Figure 8: ASCII Talbe
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/ASCII.png" alt="ASCII Talbe"/>
</p>

<p align="center">
   https://simple.wikipedia.org/wiki/ASCII
</p>

### ![#1589F0](https://placehold.it/15/1589F0/000000?text=+) `Image/Video in Binary`

Now, let’s consider images, videos and all the graphics you see on a screen. All of these images are made out of tiny
dots called pixels, and each pixel can be represented with numbers. When you consider that a typical image has
millions of these pixels, and a typical video shows 30 images per second, now, there are a lot of data here. 

<p align="center">
   Figure 9: Image in Binary
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/rgb.png" alt="Image"/>
</p>

<p align="center">
   Curtesy of Andrew Ng
</p>

### ![#ff00ff](https://placehold.it/15/ff00ff/000000?text=+) `Audio in Binary`

Every sound is basically a series of vibrations in the ear. Vibrations can be represented graphically as a waveform.
Any point on this waveform can be represented by a number. And this way, any sound can be broken down into a series of
numbers. If you want higher-quality sound, you will pick 32-bit audio over 8-bit audio. More bits means a higher range of
numbers.

<p align="center">
   Figure 10: Sound in Binary
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/sound.png" alt="Sound Waveform"/>
</p>

<p align="center">
   Curtesy of https://www.khanacademy.org/
</p>

When you use a computer to write code, or make your own app, you’re not dealing directly with these ones and zeros, but you
will be dealing with images, or sound, or video. So, if you want to understand how computers work on the inside, it all comes
down to these simple ones and zeros. and the electrical signals in the circuits behind them. They are the backbone of how all
computers input, store, process, and output information.

# `3. Kilobyte, Megabyte, Gigabyte, Terabyte`

<p align="center">
   Figure 11: Kilobyte, Megabyte, Gigabyte, Terabyte
</p>

<p align="center">
  <img src="https://github.com/XinYangSAU/CSCI1101-Intro-to-Computing/blob/master/Images/b.png" alt="Byte"/>
</p>

### ![#ff00ff](https://placehold.it/15/ff00ff/000000?text=+) `Kilobyte KB - about 1 thousand bytes`
	A small email text is about 2KB
	Text does not take a lot of bytes to store compared to image or video
	
### ![#0099ff](https://placehold.it/15/0099ff/000000?text=+) `Megabyte MB - about 1 million bytes`
	MP3 audio is about 1 megabyte per minute
	A high quality digital picture is about 2-5 megabytes	
	
### ![#cc0066](https://placehold.it/15/cc0066/000000?text=+) `Gigabyte GB - about 1 billion bytes`
	MP3 audio is about 1 megabyte per minute
	An ordinary computer might have 8GB RAM
	
### ![#009900](https://placehold.it/15/009900/000000?text=+) `Terabyte TB - about 1,000,000,000,000 bytes`
	You can buy TB hard drives todya

