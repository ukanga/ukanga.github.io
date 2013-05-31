---
layout: post
title: "python sorted list of dictionaries"
date: 2013-05-31 12:22
comments: true
categories: 
 - python
 - dict
 - dictionaries
 - sort
 - sorting
 - sorted
 - list
---

Picked up sorting list of python dictionaries from [stackoverflow](http://stackoverflow.com/questions/72899/in-python-how-do-i-sort-a-list-of-dictionaries-by-values-of-the-dictionary).
```python
items = [{"name": "Denno", "type": "nickname"}, {"name": "Ugali", "type": "food"}]
sorted_items_by_type = sorted(items, key=lambda k: k['type'])
```
Alternatively:
```python
from operator import itemgetter
sorted_items_by_type = sorted(items, key=itemgetter('type'))
```
