---
title: computer architecture (21) CPU
published: 2025-10-15 00:00:14
description: "王道计组 第五章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: true
lang: cn
---


<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100514696&p=61"  crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

- ## 本章总览
    - CPU的功能和结构
    - 指令执行过程
    - 数据通路的功能和基础结构
    - 控制器的功能和工作原理
    - 指令流水线


回忆过去，我们知道CPU由**运算器**和**控制器**两大部件组成。

![alt text](image-2.png)

其中，运算器主要负责对数据进行处理，也就是算术运算和逻辑运算。

![alt text](image-3.png)

控制器由①CU ②IR ③PC，三个部分组成。

除此之外也有其他一些重要的寄存器。

![alt text](image-4.png)

在控制单元的指挥之下，CPU会执行一系列的指令序列。

每一条指令的执行分为①取指令②分析指令③执行指令，这样的三个部分。

:::note
CPU工作的过程，就是执行一条条指令的过程。
:::

![alt text](image-5.png)

![alt text](image-6.png)

## CPU的功能和结构

<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100518079&p=62"  crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

### CPU的功能

![alt text](image-7.png)

### 运算器的基本结构

![alt text](image-9.png)

![alt text](image-10.png)

![alt text](image-11.png)

### 控制器的基本结构

![alt text](image-12.png)


### CPU的基本结构
![alt text](image-13.png)

![alt text](image-14.png)

## 指令执行过程

<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100519299&p=63"  crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

### 指令周期

![alt text](image-15.png)

![alt text](image-16.png)

![alt text](image-17.png)

![alt text](image-18.png)

![alt text](image-19.png)

### 指令周期的数据流-取指周期

![alt text](image-20.png)

### 指令周期的数据流-间址周期

 ![alt text](image-22.png)

### 指令周期的数据流-中断周期
![alt text](image-21.png)

### 本节回顾

![alt text](image-23.png)

## 数据通路-单总线结构

<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100521960&p=64"  crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

一条指令的执行，指令周期会被划分为不同的阶段。

在不同的阶段有可能数据的流向是不一样的，大致分为：

1. 寄存器与寄存器之间的数据流通。
2. 寄存器与主存之间的数据流通。
3. 寄存器与算术逻辑单元（ALU）之间的数据流通。

![alt text](image-24.png)

###