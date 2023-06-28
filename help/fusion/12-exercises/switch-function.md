---
title: Switch函数
description: 了解如何使用Switch功能使用交换机功能。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Switch函数

了解如何使用Switch功能使用交换机功能。

## 练习概述

对于简单的数据更改，请使用Switch函数在模块字段中将一个值转换为另一个值。 在本练习中，将两个字母的键更改为要在电子邮件中发送的项目进度状态的实际名称。

![切换函数图像1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 要遵循的步骤

1. 克隆名为“在路由路径之间共享变量”的方案。
1. 将新方案命名为“在路由路径之间共享变量 — 交换机”。
1. 单击触发器模块，然后将进度状态添加到输出部分。
1. 在发送电子邮件模块中，将进度状态添加到内容字段。

   + 如果只映射来自搜索模块的值，则进度状态代码为两个字母。
   + 要“切换”每个可能进度状态的完整名称代码，请使用“常规函数”选项卡中的“切换”函数。

1. switch函数使用Progress Status值或表达式作为键，然后根据该键返回输出值。

   + 在进度状态(“LT”)之后的第一个位置定义键值，并在第二个位置(“Late”)定义相应的输出。
   + 对于所需数量的键，下一个键值在第三位置定义，相应的输出在第四位置等定义。

     ![切换函数图像2](../12-exercises/assets/switch-function-walkthrough-2.png)
