---
layout: post
title: Powerline 美化 bash prompt
date: 2020-09-27 16:56
categories: bash
---

## instruction:

* 安裝 python3 和 pip3  
```console
sudo apt install python3 python3-pip
```

* 安裝 powerline-status
```console
pip3 install powerline-status
```

* 安裝 powerline 字體
```console
git clone https://github.com/powerline/fonts
```
```console
./fonts/install.sh
```

* 配置 .bashrc
```console
cat >> .bashrc << EOF
```
```console
source $(pip show powerline-status | awk '/Location:/{print $2 "/powerline/bindings/bash/powerline.sh"}')
```
```console
EOF
```

完成~

***

## note

* 使用 apt-cache depends <pkg-name> 來找尋套件相依性
* EOF 代表檔案的結尾 (End Of File)

***

## 引用資源
[powerline 設定](https://www.cnblogs.com/fsjohnhuang/p/6057013.html)

[apt-cache 使用](https://samwhelp.github.io/book-ubuntu-basic-skill/book/content/package/how-to-find-out-package-dependency.html)
