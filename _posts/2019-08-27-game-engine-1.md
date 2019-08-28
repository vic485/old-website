---
layout: default
title: "Game Engine Update"
tags: devlogs
image: /assets/img/file.ico
---

## Game Engine Progress
After starting work on the game engine last week, the first part to get built was the logging system to catch errors and messages in the future. I wanted to keep a similar api to Unity, so a public **Debug** class is being used to handle all logs even in the engine. This may be changed later if special logging is needed for specific parts of the engine. Below is an example of some **Debug.Log()** messages sent to both the console and a log file. (Originally in the active directory, this was moved to a local AppData folder on Windows and .config on *nix)

![Cross-platform and regional logging](/images/engine/logging-test.png)

A window system has also been started, using GLFW currently. An abstraction window class is being built so that this can be easily changed in the future if needed. Currently it opens a black 1280x720 window until a settings system is in place, and OpenGL is implemented.

![GLFW Window](/images/engine/initial-window.png)
