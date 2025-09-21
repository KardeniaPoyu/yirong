---
title: computer architecture (13) 命令の基本形式
published: 2025-09-19 00:00:09
description: "王道计组 第三章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: false
lang: cn
---
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100480292&p=45"crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>


- ## 指令格式
    - 操作码、地址码的概念
    - 根据地址码数目不同分类
    - 根据指令长度分类
    - 根据操作码的长度不同分类
    - 根据操作类型分类

![alt text](image-10.png)
![alt text](image-11.png)

:::note
这一章主要探讨控制器相关的指令如何设计。
:::
![alt text](image-12.png)
![alt text](image.png)

###  指令-按地址码数目分类


![alt text](image-4.png)

#### 零地址指令

![alt text](image-1.png)

#### 一地址指令

![alt text](image-2.png)

#### 二、三地址指令

![alt text](image-3.png)

#### 四地址指令
 
###  指令-按指令长度分类

指令长度指是机器字长的多少倍。

![alt text](image-5.png)


###  指令-按操作码长度分类

![alt text](image-6.png)

###  指令-按操作类型分类

![alt text](image-7.png)


---

###  知识回顾

---

![alt text](image-8.png)




###  扩展操作码指令格式

![alt text](image-9.png)

![alt text](image-13.png)

![alt text](image-14.png)

:::note
编码部分可以和哈夫曼树“前缀编码”进行对比学习。
:::

![alt text](image-15.png)

![alt text](image-16.png)

:::warning
短的操作码不能是长的操作码的前缀，否则在译码阶段容易出现歧义
::: 