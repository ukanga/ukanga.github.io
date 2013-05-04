---
layout: post
title: "256 color support in gnome-terminal"
date: 2013-05-04 19:59
comments: true
categories: 
- gnome
- terminal
- powerline
- vim
- tip
---

To get the fancy color stuff that [powerline](https://github.com/Lokaltog/powerline) provides and the great color schemes
available for vim on gnome-terminal, you will have to ensure that $TERM is reported
correctly. Under Profile Preferences > Title and Command > Custom Command set 
`env TERM=xterm-256color /bin/bash`. 

Got these tip from [Blando's Blog](http://wujingyue.blogspot.com/2012/06/let-ubuntu-gnome-terminal-support-256.html).
