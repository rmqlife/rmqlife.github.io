---
layout: post
title: "Adaptive Network Settings with an Ubuntu"
date: 2020-07-16
categories: note
---

It can be really painful when the Wifi signal is weak. This post aims to solve the problem and create a LAN with an old wifi router and a ubuntu machine. 

Here are my hardware settings:
* A Wifi router
* A desktop installed with Ubuntu 18.04
* A Wifi adapter (optional, can establish a stronger connection to the central router) 

And here are the main steps:
* Connect the desktop with the router through an ethernet cable
* Launch the network tool preinstalled on Ubuntu by typing **nm-connection-editor** in terminal
* Click **+** button and select **Ethernet** to set the rule
* Under the tab **IPV4 settings**, choose the option **Shared to other computers** for **Method** drag-down menu.

Here is a draft for the wired connection:
![Wired Connection]({{ site.url }}/images/adaptive_network_setting.png)

Then it's time to enjoy your stable and private wifi connections!
