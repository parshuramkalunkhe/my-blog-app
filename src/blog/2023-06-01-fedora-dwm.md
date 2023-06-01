---
title: fedora and dwm
description: Like most people, I started with Ubuntu. As time passed, I become a
  distro hopper, switching Linux distributions within months. Ubuntu is the only
  distribution that I have......
author: parshuram kalunkhe
date: 2023-06-01T13:27:04.323Z
tags:
  - post
image: /assets/blog/dwm.png
imageAlt: 2023-06-01T13:27:04.347Z
---
# fedorarice

Like most people, I started with Ubuntu. As time passed, I become a distro hopper, switching Linux distributions within months. Ubuntu is the only distribution that I have used for more than 5 months. Now, I'm thinking of sticking with only one distribution that does exactly what it needs to do and nothing more. So, I decided to go with fedora. The reason I choose fedora is because it stand between the most rock solid debian and rolling release arch linux distribution and there are lots of people who wants a stable and rolling release linux distribution. 

You can download Fedora iso from there official website.

https://fedoraproject.org/

Getting started with installation of suckless tools on your freshly install fedora linux.

before installing suckless tools we need to install some basic packages and dependencies. 

```
sudo dnf install git vim cmake gcc libXft-devel libX11-devel libXinerama-devel @base-x firefox thunar mpv htop neofetch xinput feh patch zathura zathura-pdf-mupdf
```

After installing the packages we ready to go and install suckless tools

Installing dwm : Dynamic window manager

```
git clone https://git.suckless.org/dwm
cd dwm 
sudo make clean install
```

Installing st : simple terminal 

```
git clone https://git.suckless.org/st
cd st
sudo make clean install
```

Installing dmenu : Dynamic menu for x

```
git clone https://git.suckles.org/dmenu
cd dmenu
sudo make clean install
```

Now, create a file .xinitrc in your home/user directory and put this inside it :

```
#!/bin/bash

exec dwm 
```

I will add more stuff here soon.....