---
layout: default
title: "Sleeper Build Part 3"
tags: blog
image: /assets/img/file.ico
---

## Getting the front panel to work
Still plugging away on this build, it goes slow when you can't spend a lot of money at once. I had wanted to get the motherboard in for fitment checks but I've seen quite a few DOA reviews for it so that will have to wait either until I can afford the CPU and cooling as well, or I can find another motherboard with the same features. Slight tangent off the work, but I've decided to go with AIO watercooling on the CPU which will require modifying parts of the front of the case, and will eliminate most if not all possible hard drive mounts. So I've got to get a motherboard with plenty of M.2 slots for SSDs. PCI-E is just too expensive for the drive sizes.


I took some time to go at adapting the wiring of the front panel board for use with a new motherboard. I bought a pack of "5.91" M/F Jumper Wires" off of DigiKey so that I could connect straight to a new board as needed. All of the wires were cut at their respective block ends and soldered together, so the result is considerably longer than the original. Not really necessary since the old board was shorter front to back than a full ATX board, but good to have just in case. I purchased a new momentary switch as well since the power button is kind of finicky on actuation but I don't have a solder wick or anything to properly remove it, and my local stores don't carry the tools. I suspect the current LEDs on the board are both green (they are uncolored when powered off, but the lenses in the front bezel are not tinted either) so I want to also at least replace the HDD activity light with one of the yellow LEDs I have left over from the PiDP-8 project. Need to find a way to get solder removal tools.
[Thanks to this page for wiring details](https://www.roberthancock.com/dell/fpconn.htm)

![Starting to solder](/images/sleeper-pc/3/solder-start.png)
![Wiring complete](/images/sleeper-pc/3/solder-finish.png)
![My notes](/images/sleeper-pc/3/notebook.png)

[[Previous Part]({{ site.baseurl }}{% post_url 2019-02-14-sleeper-build-part-2 %})] [[Next Part]({{ site.baseurl }}{% post_url 2019-04-02-sleeper-build-part-4 %})]
