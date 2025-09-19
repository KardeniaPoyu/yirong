---
title: computer architecture (11) キャッシュ置換アルゴリズム
published: 2025-09-19 00:00:08
description: "王道计组 第三章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: false
lang: cn
---
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100443570&p=43"crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

- ## 替换算法
    - 随机算法（RAND）
    - 先进先出算法（FIFO）
    - 近期最少使用（LRU）
    - 最近不经常使用（LFU）

###  随机算法（RAND）

![alt text](image.png)
 
###  先进先出算法（FIFO）

![alt text](image-1.png)

###  近期最少使用算法（LRU）
![alt text](image-2.png)
  
:::warning
Cache命中时，只需要比命中行低的计数器+1，其余不变。

好处是保证了计数器只需n位。
:::
![alt text](image-4.png)


###  最不经常使用算法（LFU）

 ![alt text](image-3.png)

---

###  知识回顾

---
![alt text](image-5.png)