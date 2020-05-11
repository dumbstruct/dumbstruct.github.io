---
layout: post
title: "Composable Architecture TeaCode Bundle"
date: 2020-05-10
---

I've been working with [The Composable Architecture](https://github.com/pointfreeco/swift-composable-architecture) from pointfreeco for several months now and I love it. One of the great things for me is that it has a strong opinion on how to set up an app. But this also means that there is a bit of boiler plate that you end up adding to each view. You need a **state** and **action** enum. Quite often there is a **reducer** and the **init()** sets up the **store** the same way each time.

The whole point of TCA is that it is composable so you end up with a lot of **states, actions, stores, and reducers** throughout your code.
To help, I made some TeaCode expanders. Now that TCA has had it's first release I've adapted my expanders and am sharing them [here](/assets/teacodebundles/ComposableArchitecture.tcbundle.zip).

<video width="320" height="240" controls>
  <source src="/assets/videos/TeaCodeCA.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
