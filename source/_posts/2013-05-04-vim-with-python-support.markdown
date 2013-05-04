---
layout: post
title: "Vim with python support"
date: 2013-05-04 16:18
comments: true
categories: 
 - vim
 - python
 - raspbian
 - raspberrypi
---

I beat around the bush with my raspberrypi on raspbian trying to get python
 support in vim, almost got to compiling vim from source, but it gave me the
 chance to learn something new.

*  If you want to check if vim has support for python then use the has() function i.e
```:echo has('python')```
*  To install vim with python install `vim-nox` or get a suggestion from the package manager when you try to install `vim-python`.
*  To compile a debian package from source, check [this debian forum link](http://forums.debian.net/viewtopic.php?f=16&t=38976).
