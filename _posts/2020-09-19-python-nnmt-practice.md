---
layout: post
title: python 九九乘法表練習
date: 2020-09-19 20:58
categories: pythonBasic
---

## code

```python
for i in range(1, 10):
    for j in range(1, 10):
        print(str(j) + " X " + str(i) + " = " + str(j*i) + '\t', end='')
    print("")
```

***

## note

* print("something", end='') 可以使 something 之後**不換行**
* 若需要同時 print 出數字和字串, 需要使用 `str()` 將數字轉型

[view on github](https://github.com/vuncrychen/pythonBasic/blob/master/nnmt.py)