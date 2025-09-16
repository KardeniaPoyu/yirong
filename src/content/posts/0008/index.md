---
title: computer architecture (4) ROM
published: 2025-09-16 00:00:01
description: "王道计组 第三章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: false
lang: cn 
---
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100441468&p=36" crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

- ### ROM
    - MROM
    - PROM
    - EPROM
    - 闪存
    - SSD

![我的截图](/images/26.png)

由于开机的时候主存里面完全没有数据，CPU需要从主板上面的一块ROM芯片上读取开机所需指令，需要用到**BIOS芯片**，它存储了**自举装入程序**，属于ROM，负责引导装入操作系统（开机）。

我们重装电脑时用的那个蓝色程序就是BIOS程序。

:::note
虽然BIOS芯片通常在主板上，但是逻辑上把它看作是主存的一部分。也就是说，当我们提到主存的时候，除了内存条之外，还应加上BIOS芯片。
:::

![我的截图](/images/28.png)

通常CPU会给RAM和ROM进行统一编址，即主存中RAM的地址会延续ROM的地址。

 



---

###  知识回顾

---

![我的截图](/images/27.png)

:::important
很多ROM芯片虽然名字是“Read-Only”，但很多ROM也可以“写”，即EPROM，闪存，SSD。

闪存的写速度一般比读速度更慢，因为写入前要先擦除。  

RAM芯片是易失性的，ROM是非易失性的。

很多ROM也具有“随机存取”的特性，意味着速度快慢不受地址的影响。
:::