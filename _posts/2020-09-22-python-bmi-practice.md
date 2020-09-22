---
layout: post
title: python bmi 計算練習
date: 2020-09-22 16:58
categories: pythonBasic
---

## code

```python
# bmi -> 體重除以身高(m)平方

# bmi < 18.5 = 過輕
# 24 > bmi > 18.5 = 適中
# bmi >= 24 = 過重

def height_converter(h):
    return h/100

def make_bmi(h, w):
    return w/(h*h)

height = input("身高(cm): ")
weight = input("體重(kg): ")

new_height = height_converter(int(height))

bmi = make_bmi(new_height, int(weight))

min_bmi = 18.5
max_bmi = 24

if bmi < min_bmi:
    print("過輕!", end="")
    print(" (bmi: " + str('%.1f' % bmi) + ")")

elif bmi < max_bmi:
    print("健康!", end="")
    print(" (bmi: " + str('%.1f' % bmi) + ")")

else:
    print("過重!", end="")
    print(" (bmi: " + str('%.1f' % bmi) + ")")
```

***

## note

* 使用 input("") 來取得使用者輸入值, 引號內可直接 print 輸入要求
* print('%.1f' % bmi) 四捨五入到小數點第一位

[view on github](https://github.com/vuncrychen/pythonBasic/blob/master/bmi.py)
