---
title: 超越基本映射练习
description: 了解如何使用映射面板公式来操作或转换发送到模块的字段。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,catalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '314'
ht-degree: 100%

---

# 超越基本映射练习

了解如何使用映射面板公式来操作或转换发送到模块的字段。

## 练习概述

使用映射面板公式更改“超越基本映射”演练练习中的项目名称、规划开始日期和优先级。

![超越基本映射图像 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## 应遵循的步骤

**克隆您的初始场景设计场景。**

1. 在场景部分选择初始场景设计右侧的“克隆”选项，如下所示。将其命名为“超越基本映射”。

   ![超越基本映射图像 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **现在，我们将会使用“创建 Workfront 项目”模块中的映射面板来配置项目名称、规划开始日期和优先级字段。**

1. 单击“创建 Workfront 项目”模块以编辑设置。使用映射面板，将“名称”字段更改为“[我的项目名称]/[赞助商]”。

   + [我的项目名称]是解析 CSV 模块的第 1 列，而[赞助商]是第 6 列。“/”这个符号只是在两者之间键入的。

1. 接下来转到“规划开始日期”，并使用 addDays 公式向该字段添加 15 天，如“超越基本映射”演练视频中所述。
1. 找到“优先级”字段，并切换该字段右上角的“映射”按钮。拾取列表菜单将更改为数字。如果 CSV 文件置信度低于 100，则创建 if 语句将项目标记为高 (4) 优先级，否则可以标记为正常 (2)。

   + 置信度评级见第 4 列。

   **此时，您的映射面板应该如下所示：**

   ![超越基本映射图像 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. 单击“确定”，然后单击“运行一次”。
1. 在您的 Workfront 实例中查找该项目，以确保所有内容都已正确映射。
1. 保存您的场景。
