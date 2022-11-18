---
title: 超出基本映射
description: 了解如何使用映射面板公式处理或转换发送到模块的字段。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 超出基本映射

了解如何使用映射面板公式处理或转换发送到模块的字段。

## 练习概述

使用映射面板公式，从“超出基本映射”演练中更改项目名称、计划开始日期和优先级。

![超出基本映射图像1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## 要遵循的步骤

**克隆初始方案设计方案。**

1. 在方案部分中选择初始方案设计右侧的克隆选项，如下所示。 将其命名为“超出基本映射”。

   ![超出基本映射图像2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **现在，我们将使用创建Workfront项目模块中的映射面板来配置项目名称、计划开始日期和优先级字段。**

1. 单击创建Workfront项目模块以编辑设置。 使用映射面板，将Name字段更改为“[我的项目名称] by [赞助商].&quot;

   + 的 [我的项目名称] 是解析CSV模块中的第1列， [赞助商] 列6。 “by”一词只是在两者之间输入。

1. 接下来转到计划的开始日期，然后使用addDays公式向字段添加15天，如Beyond basic映射演练视频中所述。
1. 找到“优先级”字段，然后切换该字段右上方的“地图”按钮。 “选取列表”(picklist)菜单更改为数字。 如果CSV文件置信度评级小于100，请创建一个if语句，以将项目标记为高(4)优先级，否则可以为普通(2)。

   + 置信度评级在第4列中。

   **此时，映射面板应如下所示：**

   ![超出基本映射图像3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. 单击确定，然后单击运行一次。
1. 在Workfront实例中查找项目，以确保所有内容均已正确映射。
1. 保存方案。
