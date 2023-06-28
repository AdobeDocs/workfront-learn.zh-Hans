---
title: 使用JSON
description: 了解如何在场景中创建和分析JSON以支持您的设计需求。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 使用JSON

了解如何在场景中创建和分析JSON以支持您的设计需求。

## 练习概述

本练习的目的是，从概念上展示如何以JSON格式利用发送到场景的信息，并将其解析为可在整个场景中映射的字段和项。 然后，您可以从这些映射的数组中获取信息，也可以将信息聚合到JSON中，然后将其发送到预期JSON作为接收输入的另一个系统。

![使用json图像1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## 要遵循的步骤

**创建数据结构并解析JSON。**

1. 创建一个新方案，并将其命名为“使用JSON圆环数据”。
1. 对于触发器模块，请使用Set变量模块。
1. 对于变量名称，请键入“Donut data”。
1. 对于变量值，复制并粘贴在测试驱动器的Fusion Experience Files文件夹中找到的“_Donut Data - Sample JSON.rtf”文档的内容。

   ![使用json图像2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. 将此模块重命名为“来自其他连接器的JSON”。
1. 添加解析JSON模块。
1. 单击“数据结构”字段的“添加”。
1. 选择生成器并粘贴您复制到示例数据字段中的Donut Data - Sample JSON数据。

   ![使用json图像3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. 单击保存，将数据结构命名为“圆环图数据”。 然后单击“保存”。
1. 将圆环图数据从Set变量模块映射到JSON字符串字段。

   ![使用json图像4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. 保存场景，然后单击运行一次以查看输出。

   **解析JSON模块的输出应如下所示：**

   ![使用json图像5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **映射到特定的数组变量。**

1. 在Parse JSON模块后添加路由器。
1. 在顶部路径中，添加一个Set变量模块。
1. 在变量名称中，键入“Batter types by donut”。
1. 对于Variable值，请使用map函数从电池阵列中获取电池类型。

   ![使用json图像6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. 单击“确定”，然后单击“运行一次”。
1. 打开执行检查器以查看三个操作中每个操作的输出包，并显示每个操作的批次类型。

   ![使用json图像7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **将方案数据聚合到JSON。**

1. 在下方路由路径中，添加聚合到JSON模块。
1. 对于源模块，选择迭代器 — Parse JSON模块。
1. 对于数据结构，请创建或选择任意数据结构。 对于此示例，使用圆环数据。
1. 继续并直接将字段映射到此示例中，如下所示。
1. 当您进入击球和击球时，请注意这些是数组，因此您需要单击“添加项目”来映射它们。

   ![使用json图像8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. 保存方案并单击运行一次。

查看聚合到JSON模块的执行检查器，并注意如何将三个捆绑包聚合到单个JSON字符串中。 然后，您可以将此字符串发送到预期JSON的其他系统。

![使用json图像9](../12-exercises/assets/working-with-json-walkthrough-9.png)
