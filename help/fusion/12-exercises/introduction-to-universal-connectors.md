---
title: 通用连接器简介
description: 扩展您对使用REST通用连接器和使用返回的数据的理解。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# 通用连接器简介

扩展您对使用REST通用连接器和使用返回的数据的理解。

## 练习概述

在电子表格中使用“精灵宝可梦”字符，通过HTTP连接器调用Poke API以收集和发布有关该字符的更多信息。

![通用连接器简介（图1）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## 要遵循的步骤

**从Workfront下载CSV文件。**

1. 在Workfront“Fusion练习文件”文件夹中，选择“_Fusion2020_Shipping Manifest.csv”，然后单击“文档详细信息”。
1. 从URL地址复制第一个ID号。
1. 在Workfront Fusion中创建新方案。 将其命名为“Using universal connectors”。
1. 从Workfront应用程序中的“下载文档”模块开始。
1. 设置您的Workfront连接，并包括从Workfront URL复制的文档ID。
1. 将此模块重命名为“Download shipping manifest”。

   ![通用连接器简介（图9）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **解析装运清单数据。**

1. 选择解析CSV ，添加另一个模块。
1. 为11列设置分析CSV 。 选中CSV包含标头框。 选择逗号分隔符类型，并将下载文档模块中的数据放入CSV字段中。

   ![通用连接器简介（图2）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. 将此模块重命名为“Parse shipping manifest”。
1. 保存场景并单击运行一次，以便您可以在后续步骤中查看CSV文件中的数据。

   **使用通用连接器获取“神奇宝贝”数据。**

1. 添加HTTP发出请求模块。
1. 在URL字段中，使用 `https://pokeapi.co/api/v2/pokemon/[Character]`，其中 [字符] 从“分析CSV ”模块映射到“列3”。
1. 选中Parse response复选框。
1. 选择显示高级设置，然后选中“将所有状态评估为错误”旁边的框。
1. 单击“确定”并将模块重命名为“获取Pokémon信息”。

   **您的映射面板应如下所示：**

   ![通用连接器简介（图3）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **在本练习的这一部分中，您只想处理CSV文件中的行1。**

1. 在“获取Pokémon信息”模块之前添加过滤器。 将其命名为“Only row 1.”
1. 将条件设置为仅允许ID编号1通过。 ID编号1位于行1中，而ID字段位于CSV文件中的列1中。

   ![通用连接器简介（图4）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. 保存方案。
1. 单击运行一次，并观察您在HTTP发出请求模块中收到的错误消息。

   >[!IMPORTANT]
   >
   >请注意，在输入数据URL字段中，字符名称将大写。 这不适用于进行该API调用，因为字符名称需要小写。

   ![通用连接器简介（图5）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. 使用HTTP发出请求URL字段中的映射面板发出 [字符] 使用字段填写所有小写字母 **lower** 函数。

   ![通用连接器简介（图6）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **使用设置多个变量模块从API映射信息。**

1. 在获取“神奇宝贝”信息后添加设置多个变量模块。 地图名称、高度、重量和功能。
1. 由于Ababilities字段是一个数组，请记住使用map函数来访问数组中每个功能的名称。

   ![通用连接器简介（图7）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **运行没有过滤器的方案以发现其他错误。**

1. 要处理CSV文件中的所有行，请删除名为“仅第1行”的筛选器：

   + 单击过滤器图标以进行编辑。
   + 删除过滤器标签。
   + 删除条件。
   + 单击“确定”。

1. 保存方案并单击运行一次。
1. 获取Pokémon信息模块中出错。 您会看到一个超级英雄角色已被传递到“精灵宝可蒙”API。

   >[!NOTE]
   >
   >在路由器演练中，您将看到如何通过创建单独的路径来处理超级英雄来解决此错误。

   ![通用连接器简介（图8）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
