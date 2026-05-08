---
title: 过滤器练习
description: 了解如何在模块之间使用过滤器以仅允许某些类型的捆绑包通过。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# 过滤器练习

了解如何在模块之间使用过滤器以仅允许某些类型的捆绑包通过。

## 练习概述

在“超越基本映射”场景中的两个模块之间添加一个过滤器，以仅创建 CSV 文件中项目颜色为“红色”的项目。

![过滤器图像 1](../12-exercises/assets/filters-walkthrough-1.png)

## 应遵循的步骤

1. 克隆“超越基本映射”场景，并将其命名为“使用强大的过滤器”。

   **在创建 Workfront 项目模块之前添加一个过滤器，以仅允许创建红色项目。**

   ![过滤器图像 2](../12-exercises/assets/filters-walkthrough-2.png)

1. 通过单击连接模块的虚线或单击扳手图标并选择“设置过滤器”来添加过滤器。
1. 使用标签字段将过滤器命名为“仅红色项目”。
1. 在“条件”字段中，映射“项目颜色”字段（CSV 文件中的第 3 列）。 选择“等于”（不区分大小写）运算符，然后键入“红色”。
1. 单击“确定”。

   ![过滤器图像 3](../12-exercises/assets/filters-walkthrough-3.png)

   **测试过滤器并验证结果。**

1. 单击“保存”来保存场景，然后单击“运行一次”。
1. 单击过滤器的执行检查器，查看过滤器如何检查每个捆绑包，以及是否使用“通过”或“失败”转到“创建 Workfront 项目”模块。

   ![过滤器图像 4](../12-exercises/assets/filters-walkthrough-4.png)

1. 查找在您的 Workfront 实例中创建的项目。
