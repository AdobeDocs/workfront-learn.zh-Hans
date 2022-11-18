---
title: 数据存储
description: 了解如何在两个系统之间同步公司名称。 （应介于60到160个字符之间，但为59个字符）
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# 数据存储

了解如何在两个系统之间同步公司名称。

## 练习概述

这是Workfront和另一个系统公司单向同步的第一部分。 目前，它仅在Fusion数据存储与Workfront之间同步。 数据存储中的表会跟踪每个公司的Workfront ID(WFID)和CSV文件(CID)中的公司ID。 这允许在将来的某个点进行双向同步。

![数据存储图像1](../12-exercises/assets/data-stores-walkthrough-1.png)

## 要遵循的步骤

**从Workfront下载文件。**

1. 在Workfront的“Fusion Exercise Files”文件夹中，选择“_Companies.csv”并单击“文档详细信息”。
1. 从URL地址复制第一个ID号。
1. 在Fusion中，创建一个名为“使用数据存储来同步数据”的新方案。
1. 对于触发器模块，选择Workfront下载文档模块。
1. 设置您的Workfront连接并包含从Workfront URL复制的文档ID。
1. 将此模块命名为“获取公司文件”。
1. 现在，添加解析CSV模块。
1. 对于列数字段，键入2。
1. 在CSV字段中映射“下载”文档模块中的数据。
1. 将此模块命名为“解析公司文件”。
1. 保存方案并单击运行一次。

   **创建数据存储和数据结构。**

1. 添加数据存储搜索记录模块。
1. 创建名为“公司同步”的新数据存储。
1. 在数据存储中，创建名为“公司同步(struc)”的数据结构。
1. 创建四个字段。

   + CID - CSV文件中的公司ID
   + 公司名称
   + WFID -Workfront公司ID
   + 创建日期 — 确保数据类型为日期

   ![数据存储图像2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. 单击数据结构上的保存，然后将数据存储大小设置为1并保存数据存储。
1. 继续在数据存储模块中，设置一个过滤器，其中CID等于解析CSV模块中公司的ID（列1）。
1. 单击显示高级设置，然后选择选项以“继续执行方案或路由，即使此模块返回时没有结果。”

   ![数据存储图像3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. 将此模块重命名为“匹配的公司”。
1. 添加Workfront搜索记录模块。
1. 选择“公司”作为记录类型。
1. 搜索条件是Workfront中的公司名称等于CSV文件中的公司名称。
1. 对于输出，请选择公司名称和ID。

   ![数据存储图像4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. 单击“确定”并将此模块重命名为“匹配公司”。

   **根据公司是存在于Workfront中还是数据存储中，创建不同的路径。**

   **路径1 — 创建公司。**

1. 在Workfront搜索记录模块的右侧添加路由器模块。
1. 将Workfront创建记录模块添加到顶部路径。
1. 将记录类型设置为“公司”。
1. 从要映射的字段中选择名称。 将名称字段映射到解析CSV模块的输出(Column 2)。
1. 将此模块重命名为“创建公司”。

   ![数据存储图像5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. 在路由器后面添加一个过滤器，以仅在公司不在Workfront时创建。 将其命名为“不在Workfront”。
1. 从Workfront搜索模块将条件设置为ID，但该条件不存在。

   ![数据存储图像6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **准备在下一个路径中更新数据存储。**

1. 在顶部路径的末尾添加设置变量模块。
1. 将变量名称设置为“Workfront ID”。
1. 从创建公司模块将变量值设置为ID。
1. 将此模块重命名为“Set Workfront ID”。

   **路由路径2 — 更新数据存储。**

1. 在路由路径2上创建过滤器。 将其命名为“不在数据存储中”。

1. 将Condition（条件）设置为Data store模块中的Key（键），且不存在。

   ![数据存储图像7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. 此路径中的第一个模块是获取变量模块。
1. 将变量名称设置为“Workfront ID”。
1. 将此模块重命名为“获取Workfront ID”。
1. 从数据存储应用程序添加其他模块，添加/替换记录。
1. 在数据存储字段中，选择公司同步。 这是您之前创建的数据存储。
1. 将Key字段留空。
1. 在解析CSV模块中映射第1列中的CID字段。
1. 在解析CSV模块中，映射第2列中的公司名称字段。
1. 从获取Workfront ID模块映射WFID字段。
1. 对于“创建的日期”字段，使用“日期和时间”选项卡中的formatDate函数，将当前日期格式化为YYYY/MM/DD。

   ![数据存储图像8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. 单击确定，并将此模块重命名为“创建公司条目”。

   **路由路径3 — 在系统之间同步数据存储。**

1. 首先，在路由路径3上创建过滤器。 将其命名为“公司存在，而不是在数据存储中”。
1. 在数据存储搜索记录模块中将条件设置为键值，且不存在。
1. 单击添加和规则按钮，并指定CSV文件（第2列）中的公司名称等于在Workfront搜索模块中找到的公司名称。

   ![数据存储图像9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. 现在，通过克隆路径2末尾的记录模块来添加另一个添加/替换记录模块。
1. 将克隆的模块拖到路由路径3的末尾处。 删除原有的空模块。
1. 单击克隆的模块。 除WFID字段外，所有字段都应保持相同。 从匹配公司搜索模块中映射它。

   ![数据存储图像10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. 单击确定，并将此模块重命名为“创建公司条目”。
