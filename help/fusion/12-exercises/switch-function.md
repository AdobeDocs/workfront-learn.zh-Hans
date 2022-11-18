---
title: 切换函数
description: 了解如何使用交换机功能。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 切换函数

了解如何使用交换机功能。

## 练习概述

要进行简单的数据更改，请使用Switch函数在模块字段中将一个值转换为另一个值。 在本练习中，将双字母键更改为要通过电子邮件发送的项目进度状态的实际名称。

![切换功能图1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 要遵循的步骤

1. 克隆名为“在路由路径之间共享变量”的方案。
1. 将新方案命名为“在路由路径之间共享变量 — 切换”。
1. 单击触发器模块，并向“输出”部分添加“进度状态”。
1. 在发送电子邮件模块中，将进度状态添加到内容字段。

   + 如果只映射来自搜索模块的值，则会有一个用于显示进度状态的双字母代码。
   + 要“切换”代码以表示每个可能的进度状态的完整名称，请使用“常规函数”选项卡中的“切换”函数。

1. 开关函数使用进度状态值或表达式作为键，然后根据该键返回输出值。

   + 键值在进度状态(“LT”)之后的第一个位置定义，并在第二个位置(“Late”)中定义相应的输出。
   + 下一个键值在第三位置定义，并在第四位置等为所需数目的键定义相应的输出。

      ![切换功能图2](../12-exercises/assets/switch-function-walkthrough-2.png)
