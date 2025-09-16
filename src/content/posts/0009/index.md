---
title: computer architecture (5) デュアルポートRAMとマルチモジュールメモリ
published: 2025-09-16
description: "王道计组 第三章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: true
lang: cn
---
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1179018518&p=37"  crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

- ## 提升主存速度
    - 双端口RAM
    - 多模块存储器
    - 实际应用

![我的截图](/images/29.png)

回顾**存取周期**的概念，如果有多个CPU需要访问，但是上一个CPU还在恢复时间，怎么办？

主存恢复时间太长，又怎么办？

这是这一小节我们要解决的两个问题。 

答案是第一个问题使用双端口RAM解决，第二个问题使用多模块存储器解决。

### 双端口RAM

![alt text](/images/30.png)
:::warning
两个端口不能同时对同一地址进行写或一个写一个读。

解决方法：通过控制电路实现暂时关闭一个端口。
:::


### 多体并行存储器

地址分为体号和体内地址，不同交叉编址时二者顺序不同。


---

###  知识回顾

---
![alt text](image.png)

:::important
很多ROM芯片虽然名字是“Read-Only”，但很多ROM也可以“写”，即EPROM，闪存，SSD。

闪存的写速度一般比读速度更慢，因为写入前要先擦除。  

RAM芯片是易失性的，ROM是非易失性的。

很多ROM也具有“随机存取”的特性，意味着速度快慢不受地址的影响。
:::