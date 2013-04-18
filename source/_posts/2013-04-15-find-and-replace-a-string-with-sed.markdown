---
layout: post
title: "find and replace a string with sed"
date: 2013-04-15 15:38
comments: true
categories: [bash, sed, commandline] 
---
**Find and replace a string from several files with sed**

```bash
$ find  . -name '*.html' -type f -exec sed -i 's/\ language="javascript"//g' {} \;
```
