---
layout: post
title: "To ObjC or Not To ObjC"
date: 2020-03-10
---

A common question I see on Twitter is something along the lines of [@raphaelschaad](https://twitter.com/raphaelschaad)'s [tweet](https://twitter.com/raphaelschaad/status/1221179164184604672).

I say, if you are starting a "FRESH iPhone app" in 2020, you should choose Swift. Many people say to stick to ObjcC but I disagree. Here's why:

1. Swift is the future, it's here to stay, and all new tutorials, APIs, etc... are going to be Swift-first so it's time to get with the programme.
2. The tooling and compile times will improve so there is only upside but I think we are comparing apples to oranges when discussing compile times of ObjC vs Swift (I will elaborate below).
3. We've reached ABI stability which means that apps to do not have to carry the weight of all the libraries with them any more.
4. Swift is a genuinely powerful language that has some incredible features that are worth exploring. I've been blowing my mind recently watching [pointfreeco](https://www.pointfree.co/) videos. If you are interested in levelling up your coding skills, Swift gives you that opportunity more than ObjC in my humble opinion.
 
## The Compile-Time Fallacy

Whilst it is true that currently ObjC compiles faster than the equivalent Swift, this misses the point. It's a bit like the Megahertz Myth of the 90s in that it does not measure all the things it should. My workflow with ObjC would be to write code, compile, step through to see what it actually does and what types are really being passed around, and then correct and repeat as necessary. ObjC happily compiles code that just doesn't do what you intended. You have to check it does after compilation with your human sponge-brain. It's a natural flow to get into; bash some code out, hit build and run, look inside the variables. But we don't measure the bit after hitting build and run in compile-time comparisons.

When I first started using Swift, it was jarring. It won't let you hit build and run as frequently. You have to get the types right before it even compiles. You can't run a piece of code to see if the correct types are being used. It feels like Swift is being a dick to you. It is a big change but over time you become more adept at getting it right before building, the latest error message improvements are a help here too, and once it compiles you do not then have to step through the code checking the types are correct because they just are. My observation is that the human type-checking you need to do with ObjC is way slower than the compiler type-checking in Swift. So Swift is not slower to develop with than ObjC if you factor in the additional post-compilation human work I think ObjC necessitates.

Coming from ObjC to Swift requires a big mindset change and resetting habits formed over years but it is totally worth it.