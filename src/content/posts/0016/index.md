---
title: computer architecture (10) キャッシュ・メモリと主記憶のマッピング方式
published: 2025-09-19 00:00:06
description: "王道计组 第三章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: false
lang: cn
---
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100443254&p=42"  crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>


- ## Cache-主存映射方式
    - Cache中存储的信息
    - 全相联映射
    - 直接映射
    - 组相联映射

![alt text](image.png)


### 全相联映射（随意放）
![alt text](image-1.png)
![alt text](image-2.png)

### 直接映射（只能放固定位置）

![alt text](image-3.png)

优化：根据位置=主存块号%Cache总块数，能保存在0号Cache块的数据，对应的主存块的地址末三位也一定是000，因此不需要保存，其他位同理。

![alt text](image-4.png)

### 组相连映射（可放到特定分组）
![alt text](image-5.png)
![alt text](image-8.png)



---

###  知识回顾

---

![alt text](image-7.png)