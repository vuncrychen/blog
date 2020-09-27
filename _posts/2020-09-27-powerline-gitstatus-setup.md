---
layout: post
title: powerline-gitstatus 美化 git
date: 2020-09-27 22:37
categories: bash
---

## instruction:

* 安裝 powerline-gitstatus
```console
pip3 install powerline-gitstatus
```

* 參考 [powerline-gitstatus](https://github.com/jaspernbrouwer/powerline-gitstatus) 專案內的指示做設定, 或使用我推薦的 [設定檔](https://github.com/spacemoose/powerline_cofiguration)
```console
cd ~/.config
```
```console
git clone https://github.com/spacemoose/powerline_cofiguration.git powerline
```

* 重新載入 powerline
```console
powerline-daemon --replace
```

完成~ (順便附上一張成果圖)
![pic](https://github.com/vuncrychen/blogger_pic/blob/master/20200927.png?raw=true)

***

## 引用資源
[powerline-gitstatus 專案](https://github.com/jaspernbrouwer/powerline-gitstatus)

[powerline-gitstatus config](http://www.glenstark.net/2016/02/powerline-git-fedora)
