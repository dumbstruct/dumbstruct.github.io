---
layout: default
title: "dumbStruct.first"
---

Welcome to Dumb Struct by Andrew Brian. Dumb Struct is intended to be my blog about Swift. I've been using Swift almost every day since Chris Lattner announced it at WWDC '14. I was lucky enough to be in the audience that day and remember the surprise and excitement I felt from day 1. Every day, I learn more and get deeper into what you can express in the language. Emphatically, I don't think Swift is a dick. However, it is so powerful and feature-rich now it is harder to think of it as an easy language than when it was launched.
There are already some good blogs about Swift, [Hacking with Swift](https://www.hackingwithswift.com) and [Swift by Sundell](https://www.swiftbysundell.com) are two excellent examples. I will not try to reproduce them here but will be driven by the things I find interesting about Swift, linking to other articles that I find interesting. Hours after I registered [dumbstruct.com](http://dumbstruct.com/), Brent Simmons posted [Immutable Swift Structs](https://inessential.com/2020/01/16/immutable_swift_structs) which precipitated a Twitter discussion on whether to default to let or var in structs. I will post my thoughts on this in another post but the TLDR is that I agree with Brent and favour immutability.

The humble struct is the building block of much of what Swift can do. I think of dumb structs as having little or no variables and/or maybe 1 function. Dumb structs feature heavily in my code but they also power things like SwiftUI which is built on a struct with no variables and a single body function. The struct can become incredibly powerful through ruthless simplicity. A really dumb struct would hold just 1 immutable value. And it is worth doing even this.

struct Dumb { let author = "Andrew Brian" }