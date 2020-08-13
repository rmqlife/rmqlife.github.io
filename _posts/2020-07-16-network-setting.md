---
layout: post
title: "How to Build a Subnet when Signal is weak with an Ubuntu"
date: 2020-07-16
categories: note
---

It can be really painful when the WIFI signal is weak. This post aims to solve the problem and create a LAN with an old WIFI router and a linux machine. 

Here are my hardware settings:
* A WIFI router
* A desktop installed with Ubuntu 18.04
* A WIFI adapter (optional, can establish a stronger connection to the central router) 

And here are the main steps:
* Connect the desktop with the router through an ethernet cable
* Launch the network tool preinstalled on Ubuntu by typing **nm-connection-editor** in terminal
* Click **+** button and select **Ethernet** to set the rule
* Under the tab **IPV4 settings**, choose the option **Shared to other computers** for **Method** drag-down menu.

Here is a draft for the wired connection:
![Wired Connection]({{ site.url }}/images/adaptive_network_setting.png)

Then it's time to enjoy your stable and private WIFI connections!
