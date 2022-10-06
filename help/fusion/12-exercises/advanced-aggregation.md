---
title: 高级聚合
description: 了解如何在聚合时使用分组。 （应介于60到160个字符之间，但为49个字符）
feature: Workfront Fusion
role: User
level: Beginner
kt: 11048
thumbnail: KT11048.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---


# 高级聚合

了解如何在聚合时使用分组。

## 练习概述

可通过网络服务返回有关多个国家的详细信息，并确定按分区域分组的所有国家总人口。

![高级聚合映像1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## 要遵循的步骤

**获取国家/地区详细信息。**

![高级聚合映像2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. 创建新方案并将其命名为“高级聚合”。
1. 将触发器模块设置为HTTP — 发出请求模块。
1. 使用此URL https://restcountries.eu/rest/v2/ lang/es ，它为您提供了所有使用西班牙语的国家/地区的列表。
1. 将方法保留为Get。
1. 单击Parse响应复选框。
1. 将此模块重命名为“获取国家/地区”。
1. 单击保存并运行一次。

   **输出是单个捆绑包，但是它是一个数组，包含24个集合，每个西班牙语国家一个。**

   ![高级聚合映像3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **您需要为每个国家/地区收集分区域信息，因此您需要发起额外的HTTP请求。**

1. 添加另一个请求以获取分区域信息。 它只会返回第一个国家，但是现在没问题。 添加其他HTTP发出请求模块，然后使用URL https://restcountries.eu/rest/v2/name/ 。
1. 要获取第一个国家/地区的名称，请转到映射面板，单击数据，然后单击数组中的名称。 的 [1] 在“数据”字段中，表示它将返回数组中的第一个项目。

   + 单击数字并根据需要更改索引，但在这种情况下，您只需要第一个项目。

   ![高级聚合映像4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. 在映射面板中选中解析响应，然后单击确定。
1. 重命名此“获取国家/地区详细信息”。
1. 单击保存，然后单击运行一次。

   + 产出是单个国家/地区的信息。

1. 要访问其他国家/地区，您需要遍历该阵列。 添加迭代器，该迭代器获取一个事项列表，并为列表上的每个项目输出一个包。

   **添加迭代器和聚合器。**

1. 在HTTP模块之间右键单击并添加迭代器流量控制模块。
1. 在数组字段中，从获取国家/地区模块中选择数据。

   ![高级聚合映像5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. 在获取国家/地区详细信息模块中，更新URL字段，以从迭代器中获取名称字段，而不是从获取国家/地区模块获取名称字段。

   ![高级聚合映像6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. 现在，在获取国家/地区详细信息后添加一个数字聚合器，以对群体进行分组和求和。
1. 源模块是迭代器模块。
1. 聚合函数为SUM。
1. 值为 [数据：群体] 从获取国家/地区详细信息模块。
1. 单击底部的显示高级设置选项，并按 [数据：分区] 从获取国家/地区详细信息模块。

   ![高级聚合映像7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **使用文本聚合器完成，以聚合您在数字聚合器中分组的内容。**

1. 向末尾添加文本聚合器。
1. 源模块是数值聚合器。
1. 在文本区域中，插入“ [键] is [结果].&quot;

   ![高级聚合映像8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. 保存并运行一次。

   + 查看最终模块的输出。
