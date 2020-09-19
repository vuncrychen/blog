---
layout: post
title: python-pyramid-practice
date: 2020-09-19 19:17
categories:
---

## code

```python
# pyramid(3): print the star tower, height = 3

def pyramid(height):
    start = 1
    while height > 0:
        print(' ' * (height-1) + '*' * start)
        start += 2
        height -= 1

pyramid(5)
```

***

## note

* pyramid() 參數值代表金字塔的**高度**

[view on github](https://github.com/vuncrychen/pythonBasic/blob/master/funcstartower.py)
