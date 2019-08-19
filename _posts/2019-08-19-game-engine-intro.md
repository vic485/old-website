---
layout: default
title: "Game Engine Intro"
tags: devlogs
image: /assets/img/file.ico
---

## Beginning Game Engine Development
Recently, I've been doing a lot of 2D projects in Unity playing with different game styles. In between that I've searched for a "best" engine to build these games in. Unity was my first choice, however as someone who is (obsesively) concerned with disk space, I couldn't find a decent way to strip out large portions of the 3D engine without breaking packages. Unreal I immediately crossed off my list as I know it to be a heavy engine, and only heard bad things about using 2D in it. Godot seemed like an interesting option with an increasing interest from others, but the C# in it is still Mono backed and experimental in ways. Finally I checked Cocos2D though I'd prefer to avoid JS if I can, and XNA is well, XNA.

All of this led me back to an old project I had thought of a while back. What if I built my own engine?
## Engine Design
To start, the entire engine is being built in C# on the latest .Net Core 3.0 preview. This allows me to use the latest versions of the language in runtime, and quickly build for cross-platform applications. Typically you would use something lower level such as C++ for the engine itself, but since this will be a purely 2D engine I feel that the modern .Net runtime is perfectly able to keep up.

Since .Net Core has no GUI or windowing system out of the box, I'll be using GLFW to handle this with the glfw-net package from ForeverZer0. OpenGL is going to be the initial rendering system in the engine since it is easy to work with, though it would be nice later to come back with vulkan for better performance. Since I do not currently own or plan to own a Mac device, metal would be out of the question and Windows and Linux will be the primary output targets of the engine. 

Lastly part of the design spec is to keep the engine light on both resources and storage space. Ideally the engine will be split into multiple non-reliant dlls for things such as core mechanisms, physics, and audio, in order to only ship what is needed. The entirety of the engine will be open source on [GitHub](https://github.com/vic485/EdoEngine) licensed under BSD-3 so check it out.
