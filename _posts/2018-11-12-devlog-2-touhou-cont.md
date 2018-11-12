---
layout: default
title: "Devlog #2 - Touhou Game"
tags: devlogs
---

## Framing out the game

The majority of the week was spent working on the basis of the game. The character sprite sheet is taken from sprite database (I'm sorry I promise I'll replace it), and the ground tiles are from open game art (may be replaced in the future).

![Not so big](/images/devlogs/2/base_assets.png)

Looking a bit into the character controller, a lot of time (like too much time) was spent working in the animator to get 8-way directional movement, as well as idles in those directions. The end result came out rather nice, but I do not look forward to re doing the animations again for other characters. The controller itself is a two part system currently, housing an input handler (I plan to do customizable input settings later on) and a 2D state machine built because I have a feeling it will be necessary moving forward. The camera is currently static while I decide whether I want a simple lerped-follow camera or have it stop at the edges of each "world tile" before moving to the next like in "A Link to the Past."

![Not so big](/images/devlogs/2/8-way_movement.gif)

The last piece of the game worked on was Discord rich presence integration. I know it is rather early, but I've played with rich presence before so I wanted to put it in quick so I know it's there and works. A few days were spent working with some guys on the discordrpc GitHub page to get it working in Windows IL2CPP builds. The end result seems to work well, and I'll need to work it into my main Discord RPC repo at some point this coming week/month.

![Not so big](/images/devlogs/2/discord-rp.png)
