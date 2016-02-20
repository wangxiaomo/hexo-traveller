layout: post
title: osx defaults 以及 Prefs Editor
date: 2016-02-19 19:57:20
tags:
  - osx
  - code
---

晚上提示要更新到iTerm Beta3,自然是要升级的,然而升级之后iTerm就不听使唤了。一开始估计可能是自己的profile中的login command设置出错了,既然iTerm启动不起来，没法在偏好设置里面修改，于是打算通过defaults强制更新。

```bash
defaults read com.googlecode.iterm2
```

发现要修改的选项是domain key下的字典键值,google了半天没什么好的方法。于是寻找`defaults editor`,找到了`Prefs Editor`.修改之后启动iTerm确实成功了,但iTerm依然崩溃不断。

懒得降级版本了,还是给宝宝洗尿布吧。

<!-- more -->
