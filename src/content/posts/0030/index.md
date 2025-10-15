---
title: computer architecture (17) x86 AT&T v.s. Intel
published: 2025-10-11 00:00:10
description: "王道计组 第四章"
image: "./cover.jpg"
tags: ["院試 / Grad Prep","基礎 / Fundamentals", "日本語 / Japanese","中国語 / Chinese"]
category: ノート / Notes
draft: false
lang: cn
---
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=995248168&bvid=BV1ps4y1d73V&cid=1100486140&p=53" crolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

![alt text](image.png)

上一篇博客中我们学习了x86的Intel格式，这篇我们来看看AT&T格式有什么不同。

![alt text](image-1.png)

最大的不同：d和s的位置相反！

比例因子意味着结构体的存储大小，变址意味着结构体的索引index，以此可以找到某个结构体中的某个变量。

![alt text](image-2.png)

:::tip
看到$，%，小括号( )，这些符号时应该想到这是AT&T格式。
:::

