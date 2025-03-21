---
layout: post
title: 二十、多态
abbrlink: dbc420cd9bc14ea59b1cbcb2e15afbf0
tags: []
categories:
  - 3.编程学习
  - Python Study-2022/9
date: 1665804375620
updated: 1665838070485
---

1.多态
同样的行为，使用不同的运行对象（不同的子类），实现不同的运行结果。
![d1c0338436c1a41c0be9e697bad0f2d5.png](/resources/7aaa0e1127fa435f953352300309a7fe.png)
主体功能中只调用animal，细节再通过嵌套调用dog还是cat进行区分，当需要修改时，只需修改细节分支，主体几乎不用变动，可以减少代码改动，降低耦合。
方便后续更改。

```
多态的好处：
1.可替换性（substitutability）。
	多态对已存在代码具有可替换性。例如，多态对圆Circle类工作，对其他任何圆形几何体，如圆环，也同样工作。
2.可扩充性（extensibility）。
	多态对代码具有可扩充性。增加新的子类不影响已存在类的多态性、继承性，以及其他特性的运行和操作。实际上新加子类更容易获得多态功能。例如，在实现了圆锥、半圆锥以及半球体的多态基础上，很容易增添球体类的多态性。
3.接口性（interface-ability）。
	多态是超类通过方法签名，向子类提供了一个共同接口，由子类来完善或者覆盖它而实现的。如图8.3 所示。图中超类Shape规定了两个实现多态的接口方法，computeArea()以及computeVolume()。子类，如Circle和Sphere为了实现多态，完善或者覆盖这两个接口方法。
4.灵活性（flexibility）。
	它在应用中体现了灵活多样的操作，提高了使用效率。
5.简化性（simplicity）。
	多态简化对应用软件的代码编写和修改过程，尤其在处理大量对象的运算和操作时，这个特点尤为突出和重要。
```

![045213bdbb6b389bcf7b990842596863.png](/resources/3a169077f2174ed1a619c52ee0619ede.png)
2.抽象类
=====

多态也常用在抽象类方法上
![e658f191ff5a7cb303b823bd21461331.png](/resources/5a87d99279dc43d4baded4f4a11c2502.png)
![806c9cf0798481808a735b3ff830b763.png](/resources/30e6b9cd68fe4a07af17432564f1cf0c.png)

总结：
![566ae73d0606c1c1f21153789057f8a6.png](/resources/61986b34e7d94f459cbdfe7cecbfe4fa.png)
