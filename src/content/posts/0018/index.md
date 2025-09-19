---
title: computer architecture (12) キャッシュの書き込み方式
published: 2025-09-19 00:00:09
description: "王道计组 第三章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: false
lang: cn
---
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100444195&p=44"crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

- ## Cache写策略
    - 写命中（全写法和写回法）
    - 写不命中（写分配法和非写分配法）

:::note
为何不讨论读命中、读不命中的情况？

**读操作不会导致Cache和主存的数据不一致**
:::


###  写命中
#### 写回法

![alt text](image.png)

#### 全写法（写直通法）

![alt text](image-1.png)
 
###  写不命中
#### 写分配法

搭配写回法使用。

![alt text](image-2.png)

#### 非写分配法


搭配全写法使用。
![alt text](image-5.png)

###  多级Cache

![alt text](image-4.png)


---

###  知识回顾

---

![alt text](image-3.png)