---
title: 过滤器
description: 了解如何在模块之间使用过滤器，以仅允许特定类型的捆绑包通过。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 过滤器

了解如何在模块之间使用过滤器，以仅允许特定类型的捆绑包通过。

## 练习概述

在“超出基本映射”场景的两个模块之间添加过滤器，以仅创建在CSV文件中具有“红色”项目颜色的项目。

![滤镜图像1](../12-exercises/assets/filters-walkthrough-1.png)

## 要遵循的步骤

1. 创建“超出基本映射”方案的克隆，并将其命名为“使用强大过滤器”。

   **在创建Workfront项目模块之前添加过滤器，以仅允许创建红色项目。**

   ![滤镜图像2](../12-exercises/assets/filters-walkthrough-2.png)

1. 通过单击连接模块的虚线或单击扳手并选择设置过滤器来添加过滤器。
1. 使用“标签”字段将过滤器命名为“仅限红色项目”。
1. 在“条件”字段中，映射“项目颜色”字段（CSV文件中的列3）。 选择等于（不区分大小写）运算符，然后键入“红色”。
1. 单击“确定”。

   ![滤镜图像3](../12-exercises/assets/filters-walkthrough-3.png)

   **测试过滤器并验证结果。**

1. 单击保存以保存方案，然后单击运行一次。
1. 单击筛选器的执行检查器，以查看筛选器的执行检查每个包的方式，以及传递或未能转至创建Workfront项目模块的方式。

   ![滤镜图像4](../12-exercises/assets/filters-walkthrough-4.png)

1. 查找在您的Workfront实例中创建的项目。
