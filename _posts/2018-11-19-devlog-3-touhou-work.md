---
layout: default
title: "Devlog #3 - Touhou Game"
tags: devlogs
image: /assets/img/file.ico
---

## Light game work

This week was a bit busy at University, so the update isn't as big this time. I started working on a camera manager script, which just does a simple lerped follow for now. I may work on having it perform section changes like ALttP in the future as it will need additional functions added for planned features.

![Camera follow](/images/devlogs/3/camera_lerp.gif)

I also began work on a customizable input manager. I've only put in the movement keys for now as that is what I am testing in this stage of the game. It supports saving and loading the keymap to a file, which is currently loaded (if it exists) in the awake function of the manager object. A UI is still needed to actually customize input at runtime, which will most likely be the first thing I work on this coming week.

![Input Manager inspector](/images/devlogs/3/input_serialization.png)
