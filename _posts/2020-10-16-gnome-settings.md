---
layout: post
title: "Gnome Desktop Settings"
date: 2020-10-16
categories: reading
---
Here are the settings for my current Ubuntu/Gnome desktop environment.

![Comment]({{ site.url }}/images/desktop.png)


### Theme / Icons
- [Pling Store](), download as a AppImage(executable). It can download/organize/store themes. For ubuntu 20.04, which uses GTK3 as default desktop environment, you can search under GTK3 categories.

- [Gnome Tweak Tools](https://itsfoss.com/gnome-tweak-tool/), use the following command to install. It can apply the changes to the system.

{% highlight bash %}
sudo apt install gnome-tweaks
{% endhighlight %}


My current settings:
- Theme: Orchis Dark
- Icon: Papirus


### Dock

- [Dash to Panel](https://extensions.gnome.org/extension/1160/dash-to-panel/), a Win10/KDE style panel. It can tweak the behaviors of the different area. The good thing is that it can perfectly replace system default dock.

- [Applications Menu](https://extensions.gnome.org/extension/6/applications-menu/)

- [Clipboard Indicator](https://extensions.gnome.org/extension/779/clipboard-indicator/)

- [Horizontal workspaces](https://extensions.gnome.org/extension/2141/horizontal-workspaces/)

- [Open Weather](https://extensions.gnome.org/extension/750/openweather/)

- [Places Status Indicator](https://extensions.gnome.org/extension/8/places-status-indicator/)

- [Workspace Indicator](https://extensions.gnome.org/extension/21/workspace-indicator/)

### Useful Tools:

- [brightness-controller](https://github.com/LordAmit/Brightness), a python written program. It can change the brightness of the monitor by software.

- [Tilix](https://gnunn1.github.io/tilix-web/), a advanced terminal mangager.

- [FlatHub](https://flatpak.org/setup/), a richer software store for linux.

- [Timeshift](https://github.com/teejee2008/timeshift), backup system to avoid unpridictable problems caused by update/grub/etc. Can be install using apt-get.

### Timezone Conflict with Windows Dual Boot

- [Explanation](https://www.howtogeek.com/323390/how-to-fix-windows-and-linux-showing-different-times-when-dual-booting/)

{% highlight bash %}
timedatectl set-local-rtc 1 --adjust-system-clock
timedatectl
{% endhighlight %}

### Input Methods Configurations
I prefer fcitx to ibus. 

- Chinese: Sogou Pinyin 搜狗拼音
- Japanese: Mozc 

Mozc uses F7 to overwrtite Katakana. Remember to put English Keyboard as primary input method so that you can use ctrl+blank to toggle it with others. And ctrl+shift can toggle between others.

