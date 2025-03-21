---
layout: post
title: 十三、异常与异常捕获
abbrlink: 0eeb7f0dbf9143689cecdab6f7f7decf
tags: []
categories:
  - 3.编程学习
  - Python Study-2022/9
date: 1665325636484
updated: 1722330540684
---

# 1.基本语法：

![0858c77a1a2bbefecb456b7d77bf90a6.png](/resources/e0f6e4a8e657460b92af6e1a147634d2.png)
![2172744d28515c6d7b18a7c52e70fa65.png](/resources/f61a2f32ee9b4bf5899a0f87aa44c2a5.png)

***

# 2.捕获指定异常

![116630397bf207aedd15a29edde9a238.png](/resources/bdfec52dee4c4bd8a9f9742055a233ff.png)

***

# 3.捕获多个异常

![84a01edd2df4dfb7e06af76bd4ce9aea.png](/resources/3fdb5cad916746588dab1da153d7120f.png)

***

# 4.捕获所有异常

用基础语法不指定异常，或者用如下的exception
![ee5bd1f8d571b85bf338954ec8379ac7.png](/resources/3631b92a3b814a4daa258e2ebb768f6b.png)

***

# 5.else和finally语句

![3deb862df496f1919cfed6c97d4b648e.png](/resources/a5627266afdc4938a43897ae842c5885.png)
else表示无异常就做的事，finally表示无论如何都要做的事。
![6ce0c69b421430311f7e3dfde9a729ae.png](/resources/65718725dbca42aa918a7e32099aa6d5.png)

***

# 6.异常的传递

会一层层往调用它的函数里传，直到最高层级。
![6e9bdb2d86bcfe84f56efb1799bac16c.png](/resources/a767a862d5f14535a2ff31fd85046a48.png)

# 7.with 语法糖

[with\_菜鸟教程](https://www.runoob.com/python3/python-with.html)
Python 中的 with 语句用于异常处理，封装了 `try…except…finally` 编码范式，提高了易用性。
with 语句使代码更清晰、更具可读性， 它<mark style="background: #5fb236">简化了文件流等公共资源的管理</mark>。
在处理文件对象时使用 with 关键字是一种很好的做法。

<mark style="background: #ff6666">**专用于文件的处理**</mark>

使用 with 关键字系统会自动调用 `f.close()` 方法， `with` 的作用等效于 `try/finally` 语句是一样的。
