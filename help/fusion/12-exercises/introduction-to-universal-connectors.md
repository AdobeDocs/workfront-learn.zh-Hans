---
title: 通用连接器简介练习
description: 加深您对如何使用 REST 通用连接器和处理返回的数据的理解。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
recommendations: noDisplay,noCatalog
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '602'
ht-degree: 100%

---

# 通用连接器简介练习

加深您对如何使用 REST 通用连接器和处理返回的数据的理解。

## 练习概述

使用电子表格中的宠物小精灵角色，通过 HTTP 连接器调用 Poke API 来收集并发布有关该角色的更多信息。

![通用连接器简介图像 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## 应遵循的步骤

**从 Workfront 下载 CSV 文件。**

1. 在 Workfront“Fusion 练习文件”文件夹中，选择 &quot;_Fusion2020_Shipping Manifest.csv&quot; 并单击“文档详细信息”。
1. 复制 URL 地址中的第一个 ID 号。
1. 在 Workfront Fusion 中创建新场景。将其命名为“使用通用连接器”。
1. 从 Workfront 应用程序中的“下载文档”模块开始。
1. 设置您的 Workfront 连接，并包含从 Workfront URL 复制的文档 ID。
1. 将此模块重命名为“下载装运清单”。

   ![通用连接器简介图像 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **解析装运清单数据。**

1. 添加另一个模块，选择“解析 CSV”。
1. 为 11 列设置解析 CSV。选中“CSV 包含标题”框。选择逗号分隔符类型，并将下载文档模块中的数据放入 CSV 字段中。

   ![通用连接器简介图像 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. 将此模块重命名为“解析装运清单”。
1. 保存该场景，并单击“运行一次”，以便您可以在后续步骤中看到 CSV 文件中的数据。

   **使用通用连接器获取宠物小精灵数据。**

1. 添加 HTTP 发出请求模块。
1. 在 URL 字段中使用 `https://pokeapi.co/api/v2/pokemon/[Character]`，其中[字符]会被映射到解析 CSV 模块的第 3 列。
1. 选中“解析响应”复选框。
1. 选择“显示高级设置”，然后选中“将所有状态评估为错误”旁边的框。
1. 单击“确定”并将该模块重命名为“获取宠物小精灵信息”。

   **您的映射面板应如下所示：**

   ![通用连接器简介图像 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **在该练习的这一部分中，您只需要处理 CSV 文件中的第 1 行。**

1. 在获取宠物小精灵信息模块之前添加一个过滤器。将其命名为“仅第 1 行”。
1. 将条件设置为只允许 1 号 ID 通过。1 号 ID 位于 CSV 文件的第 1 行，ID 字段位于第 1 列。

   ![通用连接器简介图像 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. 保存该场景。
1. 单击“运行一次”，并观察您在 HTTP 发出请求模块中收到的错误消息。

   >[!IMPORTANT]
   >
   >请注意，在输入数据 URL 字段中，角色名称是大写的。这不适用于 API 调用，因为角色名称需要小写。

   ![通用连接器简介图像 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. 使用 HTTP 发出请求 URL 字段中的映射面板，利用 **lower** 函数使[角色]字段全部为小写字母。

   ![通用连接器简介图像 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **使用设置多个变量模块从 API 映射信息。**

1. 在获取宠物小精灵信息后添加设置多个变量模块。映射名称、高度、体重和能力。
1. 由于“能力”字段是一个数组，因此请记住使用映射函数来访问数组中每个能力的名称。

   ![通用连接器简介图像 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **在不使用过滤器的情况下运行该场景以发现另一个错误。**

1. 要处理 CSV 文件中的所有行，请删除名为“仅第 1 行”的过滤器：

   + 单击过滤器图标进行编辑。
   + 删除过滤器标签。
   + 删除条件。
   + 单击“确定”。

1. 保存该场景并单击“运行一次”。
1. 获取宠物小精灵信息模块发生错误。您会看到一个超级英雄角色已传递给宠物小精灵 API。

   >[!NOTE]
   >
   >在路由器演练中，您将会了解到如何通过创建单独的路径来处理超级英雄，以此来解决此错误。

   ![通用连接器简介图像 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
