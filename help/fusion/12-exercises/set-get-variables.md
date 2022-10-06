---
title: 设置/获取变量
description: 了解如何使用设置和获取变量模块来使用不同路径中一个路径中可用的字段。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11045
thumbnail: KT11045.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---


# 设置/获取变量

了解如何使用设置和获取变量模块来使用不同路径中一个路径中可用的字段。

## 练习概述

在Workfront中查找有关项目的信息，并发送一封包含相关信息的电子邮件。

![设置获取变量图像1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## 要遵循的步骤

1. 创建新方案并将其命名为“在路由路径之间共享变量”。
1. 对于触发器，在Workfront应用程序中选择搜索模块。

   + 将记录类型设置为“项目”。
   + 对于结果集，选择“所有匹配记录”。
   + 对于“搜索”标准，将其设置为“状态等于CUR”。
   + 对于“输出”，选择“ID”、“名称”、“描述”和“赞助商ID”。

   ![设置获取变量图像2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![设置获取变量图像3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. 单击“确定”并将此模块重命名为“查找当前项目”。
1. 添加其他模块，然后选择Workfront读取记录模块。

   + 对于“记录类型”，选择“用户”。
   + 对于“输出”，选择“名称”。
   + 将赞助商ID从搜索模块映射到ID字段。

1. 单击确定。
1. 重命名模块“查找赞助商名称”。

   ![设置获取变量图像4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. 保存方案，然后单击运行一次。

   如果您在“读取记录”模块中收到错误，则可能是因为“搜索”模块在没有列出赞助商的情况下查找项目。

   **要避免出现此错误，请创建两个路径：一个用于具有赞助商ID的项目，另一个用于没有赞助商ID的项目。**

1. 单击路由器与读取记录模块之间的扳手图标，在两个模块之间添加路由器。 设置名为“赞助商存在”的过滤器，并将条件设置为“赞助商ID存在”。

   ![设置获取变量图像5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. 单击路由器以创建另一条路径。 从电子邮件应用程序添加发送电子邮件模块。

   + 在“收件人”字段中放置您自己的电子邮件地址。
   + 在“主题”字段中，键入“当前项目信息”。
   + 在“内容”字段中，输入项目名称、描述和赞助商。
   + 您无法从读取记录模块中提取赞助商名称输出。 您只能在路由器之前从搜索模块访问赞助商ID。 您需要找到从其他路由器路径访问赞助商名称的方法。

   ![设置获取变量图像6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. 现在单击确定，并将此模块重命名为“发送项目信息”

   **使用设置/获取变量在不同路径之间共享数据。**

1. 在“查找赞助商名称”模块之后，添加“设置变量”工具模块。

   + 将“赞助商名称”作为变量名称。
   + 将变量生命周期保留为一个周期。
   + 将字段映射到查找赞助商名称模块中的名称输出。

1. 单击“确定”，然后重命名“设置赞助商名称”模块。

   ![设置获取变量图像7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. 接下来，在路由器和发送电子邮件模块之间右键单击以添加获取变量工具模块。 在变量名称字段中输入“赞助商名称”。
1. 单击确定。 重命名模块“获取赞助商名称”。

   ![设置获取变量图像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. 返回“发送电子邮件”模块，并将“获取赞助商名称”模块中的值映射到内容字段。 单击确定。

   ![设置获取变量图像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >在测试此方案之前，我们建议限制您处理的项目数量，以避免收到大量电子邮件。

1. 转到您的Workfront试车，找到北星时尚参展商展位项目。 这是一个有赞助商的项目。 从URL复制项目ID。

   ![设置获取变量图像10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. 在方案中，单击查找当前项目模块。 通过单击绿色的“添加与规则”按钮，向搜索标准添加其他条件。 指定ID必须等于您复制的项目ID。 单击确定。
1. 保存方案并单击运行一次。
1. 检查执行检查员和您收到的电子邮件。

   ![设置获取变量图像11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
