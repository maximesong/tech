---
layout: post
title: "printk学习"
date: 2012-06-07 22:58
comments: true
categories: linux
---

# 查看printk的输出内容
## dmesg
{% codeblock lang:bash %}
dmesg | tail
{% endcodeblock %}

## console (注意，不是terminal)
通过设置日志级别，可以在console中输出printk的内容。这里的*console*并不包扩X Windows下的terminal。linux中用Ctrl+Alt+(F1～F7)切换console和图形界面。

### printk在控制台的日志级别
{% codeblock lang:bash %}
echo 8 > /proc/sys/kernel/printk
{% endcodeblock %}


### virtualbox中切换终端
在virtualbox里没有办法用Ctrl+Alt+(F1～F7)切换，可以用Host(Right-Ctrl)+(F1~F7)替代。


