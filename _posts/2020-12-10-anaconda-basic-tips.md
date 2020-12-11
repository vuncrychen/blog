---
layout: post
title: "[Windows 篇] Anaconda 基本使用技巧"
date: 2020-12-10 23:55:39
image: '/assets/img/post/'
description: 安裝 + 建立虛擬環境
tags:
- python
- windows
categories:
- python 學習之路
twitter_text: 安裝 + 建立虛擬環境
---

## 前言

今天來整理一下 Anaconda 在 Windows 上的一些操作, 最近有點忙, 所以下次再來整理 Pycharm 的設定, BTW 這篇應該會有很多截圖 :D

---

## 下載

這個應該很簡單吧...

[官網連結](https://www.anaconda.com/products/individual){:target="_blank"}

![anaconda_web](/assets/img/post/20201211/anaconda_web.png)

---

## 安裝

打開下載好的檔案, 會看到以下視窗

![install_1](/assets/img/post/20201211/install-1.png)

按下 Next

![install_2](/assets/img/post/20201211/install-2.png)

選擇 Just Me

![install_3](/assets/img/post/20201211/install-3.png)

選擇自己的安裝位置, Anaconda 本身沒有很大 2.7GB 而已, 但如果之後安裝很多套件...就不好說了

![install_4](/assets/img/post/20201211/install-4.png)

這裡就照預設就好, 不將 anaconda 加入環境變數

完成後就按下下一步吧!

---

## 初嘗 conda

剛安裝完打開應該會如下圖

![anaconda_home_page](/assets/img/post/20201211/anaconda-screen.png)

接者打開它的 prompt

![prompt](/assets/img/post/20201211/anaconda-prompt-screen.png)

首先可以透過以下指令查看 Python 版本

{% highlight bash %}
python -V
{% endhighlight %}

以下指令可以查看 conda 目前安裝的套件

{% highlight bash %}
conda list
{% endhighlight %}

![commandline_screen](/assets/img/post/20201211/commandline-screen.png)

可以看到 conda 已經幫我們安裝了一些常用的套件, 這樣我們就不必自行下載了, 真是方便啊~

---

## 建立虛擬環境

接著來看看怎麼建立一個乾淨的虛擬環境吧!

首先來看看總共有哪些環境

{% highlight bash %}
conda env list
{% endhighlight %}

![env_list](/assets/img/post/20201211/env_list.png)

可以看到我們只有一個叫 `(base)` 的環境, 而星號則是我們所在的環境

接下來透過以下指令來建立一個叫做 `my_env_1` 的環境, 後面的 python 版本可以自行指定

{% highlight bash %}
conda create my_env_1 python=3.8.5
{% endhighlight %}

![create_env](/assets/img/post/20201211/create_env.png)

輸入 y 來確認建立環境

完成後如下圖

![create_done](/assets/img/post/20201211/create_done.png)

可以看到 conda 很貼心的提醒我們如何啟用新建的環境

activate 吧!

{% highlight bash %}
conda activate my_env_1
{% endhighlight %}

![env_diff](/assets/img/post/20201211/diff_env.png)

使用 `conda list` 來看看跟原本的套件有沒有差別

![env_conda_list](/assets/img/post/20201211/env_conda_list.png)

可以看到只有乾淨的 python 3.8.5 不像之前有一堆套件了, 這樣就不怕會弄亂作業系統了, 終於整理完了, 好多圖, 好累...等等來玩個 OSU, XD
