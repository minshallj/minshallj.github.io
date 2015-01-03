---
layout: post
title: Chromebook development
date: 2014-12-30
---

So, I just got a chromebook (acer 720) for Christmas (from my lovely wife) and I have been
trying it out for some development. My initial thoughts are as follows:

## The yay
Everything you see on the box except for the 16GB SSD. It's only $200, it has very decent
battery life, about 8 hours. The WiFi is alright, though I have a feeling it's
exploding my Comcast router because it started needing to be reset every few hours the day
the chromebook came on to the network. It's pretty snappy for quick and easy things,
though I haven't timed it for compiling a kernel.

(Crouton)[www.github.com/dnschneid/crouton] is how I am running a natural feeling
linux environment while on the chromebook. That way I can `apt-get` whatever I need
and compile anything else that I can't get normally. I was a little sad to see no
built in C compiler on the chromebook itself, but then I've never really been happy
with the way google treats the underlying Linux system for their products (e.g. android)

So far to simulate some work (since I'm out of a job and don't have a pet project
right now) I have been writing programs to submit to (codeeval)[www.codeeval.com/profile/minshallj].
Also I want to try out serving this blog in the chroot, and accessing it from the browser,
though I think there may be some issues with trying that out. Mainly, how do I access port
4000 of my `chroot`? So far development has been fine, using the vim from inside the chroot,
everything feels mostly normal. One slightly annoying thing is getting the files from the chroot
to somewhere where I can upload them, I just copy them into the ~/Downloads folder.

## The not-so-yay
I would like the Linux environment supplied by the chromebook to be more complete. At least
give me a c compiler, and the `make` utility... That way I can `wget` my way to glory,
I'd just have to compile any programs I wanted myself, which I'd prefer over not having
them at all... If google really wanted to go above and beyond, they'd make some kind of
repository, or work with the SUSE open build service, but google doesn't really seem
to focus on the Linux user aspect of chromebooks (or android for that matter).

The SSD size. First off, 16GB is pretty small, but I can probably make it work, if
I'm just working on one thing at a time. What gets me a little ticked off though is the actual
space I'm allowed to use is a little under 11GB, which is 25% less than advertised... I
don't mind missing a few gigabytes on a system with a terrabyte of space, that's not even
1% off of what's advertised, but this feels a little shady.

I haven't been impressed with the keyboard. It's definitely a step above some keyboards
for iPads and surface pros. For heavy development this wouldn't be the best machine, but
sometimes code just takes a few changes to fix or just a couple hundred of lines to complete.
The chromebook can work well in these cases, but I wouldn't start writing a whole new project
on it.

The WiFi is decent, but as I mentioned above it seems to be killing my router. If
this router wasn't just at my family's house (where I'm visiting for the holidays)
I'd probably look deeper into this, maybe run a packet capture so I could see if it's
some packet sequence which is exploding the router... Also if it wasn't a comcast router
I could possibly get some information from the logs on it...

## All in all
I like it. It's an easy machine to use when distractions are common, it's quick
to put down and pick back up, even turning it on only takes a few seconds. I'd
get a lot more use out of it if I was taking public transportation every day for
long periods, but I think I'll still put some good use into it in my day to day.
I think it will be especially useful when I'm watching my daughter and programming,
because it's easy for me to toss aside when she comes up to me. Also it will be good
for showing her hulu videos while in an airport or something.
