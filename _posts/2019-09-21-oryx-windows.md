---
layout: default
title: "System76 Oryx Pro"
tags: blog
image: /assets/img/laptop.ico
---

## System76 Oryx Pro
Recently I purchased the [Oryx Pro](https://system76.com/laptops/oryx) from System76 as a new mobile workstation. I will do a proper review on this here later, but wanted to get some windows installation instructions down for those wanting to install windows for dual-booting purposes as I did.

## Windows Installation
{: #windows-install }
Windows can be installed on the laptop in the typical way. USB boot is enabled by default in the UEFI BIOS, F7 Just needs to be held down when powering on to open the boot menu. After installing most drivers can be installed automatically through Windows Update. Only a few drivers and utilities need to be installed outside of this. The 16" version of the Oryx Pro is essentially a Clevo P960 underneath (the 17" model appears to be a P970 but I can't completely confirm this). I prefer to install all official drivers before allowing Windows Update to run, though the only necessary items are the control center software to control fans, keyboard lighting, macros, and power modes; the audio drivers for proper headphone/set detection; and the fingerprint sensor driver which is not found by Windows Update. I also recommend using Nvidia's Geforce Experience to keep the video driver up to date. System76 doesn't provide windows drivers on their website, at least not publicly, but similar working drivers can be found from other companies selling Clevo based laptops. I used [Pro-Star](https://www.pro-star.com/driver-downloads) downloading drivers for the P960RF as this was the closest to my model according to the Clevo site and had the most up to date drivers.
