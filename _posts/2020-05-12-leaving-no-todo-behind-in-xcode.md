---
layout: post
title: "Leaving no TODO behind in Xcode"
date: 2020-05-12
---

In Xcode, you can make TODO and MARK comments that you can see in both the Jump Bar and the new minimap.
I find these really useful to use.

    //TODO: don't forget this important task

But I also have a tip on how to make your todos never get forgotten about. Just make them into a warning! Like so:

	#warning("TODO: don't forget this important task")

I have made a TeaCode expander to combine these:

    todo  don't forget this important task

expands to:

    //TODO: don't forget this important task
    #warning("TODO: don't forget this important task")

Going even further, you could create a TODO() function that outputs the TODO in the console like so:

	func TODO(_ todo: String) {
      os_log(.info, "TODO: %s", todo)
	}

And add that to your expander or snippet so you expand into:

	//TODO: don't forget this important task
	#warning("TODO: don't forget this important task")
	TODO("don't forget this important task")

But what is this craziness? Well, now when you prioritise tasks, you can use the console output as a guide to prioritise the TODOs that get **hit** the most during runtime. Filter on "TODO:", and sort and rank the results.

Sometimes this is overkill but I have found it useful. You can even make your **TODO** function output line number and file, and maintain the count for you if you want to go the extra mile.

Using these techniques, you can feel safe in the knowledge that no **TODO** gets left behind and ensure that you don't work on a piece of code that never actually gets called.
