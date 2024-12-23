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
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '229'
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
1. 在“条件”字段中，映射“项目颜色”字段（CSV 文件中的第 3 列）。选择“等于”（不区分大小写）运算符，然后键入“红色”。
1. 单击“确定”。

   ![过滤器图像 3](../12-exercises/assets/filters-walkthrough-3.png)

   **测试过滤器并验证结果。**

1. 单击“保存”来保存场景，然后单击“运行一次”。
1. 单击过滤器的执行检查器，查看过滤器如何检查每个捆绑包，以及是否使用“通过”或“失败”转到“创建 Workfront 项目”模块。

   ![过滤器图像 4](../12-exercises/assets/filters-walkthrough-4.png)

1. 查找在您的 Workfront 实例中创建的项目。
