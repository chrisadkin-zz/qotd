# Introduction

This repo is a homage to the Unix/Linux [message of the day](https://en.wikipedia.org/wiki/Motd_(Unix)) facility, to power this, a rich and abundant source of quips is requied, and it just so happens that such a source exists on twitter:

<img style="float: left; margin: 0px 15px 15px 0px;" src="https://github.com/chrisadkin/qotd/blob/main/images/Capture.PNG?raw=true">
<img style="float: left; margin: 0px 15px 15px 0px;" src="https://github.com/chrisadkin/qotd/blob/main/images/Capture2.PNG?raw=true">
<img style="float: left; margin: 0px 15px 15px 0px;" src="https://github.com/chrisadkin/qotd/blob/main/images/Capture3.PNG?raw=true">
<img style="float: left; margin: 0px 15px 15px 0px;" src="https://github.com/chrisadkin/qotd/blob/main/images/Capture4.PNG?raw=true">
<img style="float: left; margin: 0px 15px 15px 0px;" src="https://github.com/chrisadkin/qotd/blob/main/images/Capture5.PNG?raw=true">
<img style="float: left; margin: 0px 15px 15px 0px;" src="https://github.com/chrisadkin/qotd/blob/main/images/Capture6.PNG?raw=true">

# Deployment Instructions

A sample `payload.txt` file is provided that contains some quips, you are free to use this or alternatively you can harvest them from the twitter source referred to above.

1. Place your payload quip file somewhere on you your Linux filesystem, `/home/cadkin/payload.txt` for example

2. Add the following line to the .profile file in your home directory:
```
shuf -n 1 ~/payload.txt 
```
3. The simplest way to test this is to issue `newgrp -`, which - when using the sample payload.txt file provided will result in one of the following lines being displayed on the standard output of your terminal:
```
If you're tired, just set up a ladder and scatter some tools at the bottom, and take a nap there. If anyone finds you, you can just claim that you fell (Follow me for more great work tips!)
Well apparently you can't poke someone in the forehead and say "Skip Intro" when they start talking
Synonym: A word used in place of the one you can't spell
Fun fact: Betty White was actually Betty the Grey until she defeated a Balrog in the Mines of Moria
Just finished a book about "Stockholm Syndrome". It didn't really start well, but by the end I really liked it.
```
# Notes

Whilst every effort was made to develop qotd in accordance with Kelsey Hightower's [nocode](https://github.com/kelseyhightower/nocode), qotd failed to achieve this lofty goal by a single line of code, however it does fully integrate with nocode. Please refer to the [nocode](https://github.com/kelseyhightower/nocode) issues list before using it in production.
