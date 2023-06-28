---
title: 数据存储
description: 了解如何在两个系统之间同步公司名称。 （应为60至160个字符，但实为59个字符）
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# 数据存储

了解如何在两个系统之间同步公司名称。

## 练习概述

这是Workfront和另一种体系中的公司单向同步的第一部分。 目前，它仅在Fusion数据存储区和Workfront之间同步。 数据存储中的表会跟踪每个公司的CSV文件(CID)中的Workfront ID (WFID)和公司ID。 这允许在未来某个时间点进行双向同步。

![数据存储图像1](../12-exercises/assets/data-stores-walkthrough-1.png)

## 要遵循的步骤

**从Workfront下载文件。**

1. 在Workfront“Fusion Experience Files”文件夹中，选择“_Companies.csv”，然后单击“文档详细信息”。
1. 从URL地址复制第一个ID号。
1. 在Fusion中，创建一个名为“使用数据存储同步数据”的新方案。
1. 对于trigger模块，选择Workfront Document模块。
1. 设置您的Workfront连接，并包括从Workfront URL复制的文档ID。
1. 将此模块命名为“获取公司文件”。
1. 现在添加解析CSV模块。
1. 对于“列数”字段，键入2。
1. 在CSV字段中映射下载文档模块中的数据。
1. 将此模块命名为“Parse companies file”。
1. 保存方案，然后单击运行一次。

   **创建数据存储和数据结构。**

1. 添加数据存储搜索记录模块。
1. 创建一个名为“公司同步”的新数据存储。
1. 在数据存储中，创建一个名为“公司同步(struc)”的数据结构。
1. 创建四个字段。

   + cid - CSV文件中的公司ID
   + 公司名称
   + WFID - Workfront公司ID
   + 创建日期 — 确保数据类型为日期

   ![数据存储图像2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. 在数据结构上单击保存，然后将数据存储大小设置为1并保存数据存储。
1. 继续在“数据存储”模块中，设置一个筛选器，其中CID等于解析CSV模块中的公司ID（列1）。
1. 单击显示高级设置并选择选项以“即使此模块返回时没有结果，也继续执行方案或路由”。

   ![数据存储图像3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. 将此模块重命名为“匹配公司”。
1. 添加“Workfront搜索记录”模块。
1. 选择公司作为记录类型。
1. 搜索标准是Workfront中的公司名称等于CSV文件中的公司名称。
1. 对于输出，选择公司名称和ID。

   ![数据存储图像4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. 单击“确定”并将此模块重命名为“匹配公司”。

   **根据公司存在于Workfront中还是数据存储中创建不同的路径。**

   **路由路径1 — 创建公司。**

1. 在“Workfront搜索记录”模块的右侧添加一个路由器模块。
1. 将Workfront创建记录模块添加到顶部路径。
1. 将记录类型设置为公司。
1. 从要映射的字段中选择名称。 将name字段映射到Parse CSV模块（列2）的输出。
1. 将此模块重命名为“创建公司”。

   ![数据存储图像5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. 在路由器后添加过滤器，以便仅在Workfront中尚未创建公司时创建公司。 将其命名为“Not in Workfront”。
1. 将条件设置为Workfront Search模块中的ID，该ID不存在。

   ![数据存储图像6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **准备更新下一个路径中的数据存储。**

1. 在顶部路径的末尾添加Set变量模块。
1. 将变量名称设置为“Workfront ID”。
1. 将变量值设置为创建公司模块中的ID。
1. 将此模块重命名为“设置Workfront ID”。

   **路由路径2 — 更新数据存储。**

1. 在路由路径2上创建过滤器。 将其命名为“Not in data store”。

1. 将Condition设置为Data store模块中的Key且不存在。

   ![数据存储图像7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. 此路径中的第一个模块是Get variable模块。
1. 将变量名称设置为“Workfront ID”。
1. 将此模块重命名为“获取Workfront ID”。
1. 从数据存储应用添加另一个模块，添加/替换记录。
1. 在“数据存储”字段中，选择“公司同步”。 这是您之前创建的数据存储。
1. 将“Key（密钥）”字段留空。
1. 在解析CSV模块中，映射列1中的CID字段。
1. 在“分析CSV ”模块中，映射列2中的公司名称字段。
1. 从获取Workfront ID模块映射WFID字段。
1. 对于“创建日期”字段，请使用“日期和时间”选项卡中的formatDate函数，将当前日期的格式设置为MM/DD/YYYY。

   ![数据存储图像8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. 单击“确定”并将此模块重命名为“创建公司条目”。

   **路由路径3 — 同步系统之间的数据存储。**

1. 首先，在路由路径3上创建过滤器。 将其命名为“Company exists， not in data store”。
1. 将条件设置为数据存储搜索记录模块中的键，并且该键不存在。
1. 单击“添加AND规则”按钮，并指定CSV文件中的公司名称（第2列）等于“Workfront搜索”模块中找到的公司名称。

   ![数据存储图像9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. 现在，通过克隆路由路径2末尾的记录模块来添加另一个添加/替换记录模块。
1. 将克隆的模块拖动到路由路径3末尾的位置。 删除存在的空模块。
1. 单击克隆的模块。 除WFID字段外，所有字段都应保持不变。 从“匹配公司搜索”模块对其进行映射。

   ![数据存储图像10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. 单击“确定”并将此模块重命名为“创建公司条目”。
