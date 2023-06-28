---
title: Set/Get变量
description: 了解如何使用Set和Get Variable模块，将某个路径中可用的字段用于其他路径。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11045
thumbnail: KT11045.png
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Set/Get变量

了解如何使用Set和Get Variable模块，将某个路径中可用的字段用于其他路径。

## 练习概述

在Workfront中查找有关项目的信息，并发送包含相关信息的电子邮件。

![Set Get variables图像1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## 要遵循的步骤

1. 创建一个新方案，并将其命名为“在路由路径之间共享变量”。
1. 对于触发器，选择Workfront应用程序中的搜索模块。

   + 将“记录类型”设置为“项目”。
   + 对于结果集，选择“所有匹配记录”。
   + 对于“搜索”条件，将其设置为“状态等于CUR”。
   + 对于输出，请选择ID、名称、描述和赞助者ID。

   ![Set Get variables图像2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Set Get variables图像3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. 单击“确定”并将此模块重命名为“查找当前项目”。
1. 添加另一个模块，然后选择Workfront读取记录模块。

   + 对于“记录类型”，选择“用户”。
   + 对于“输出”，选择“名称”。
   + 将发起人ID从搜索模块映射到ID字段。

1. 单击“确定”。
1. 将模块重命名为“查找发起人姓名”。

   ![Set Get variables图像4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. 保存方案并单击运行一次。

   如果您在读取记录模块中收到错误，可能是因为搜索模块查找未列出赞助者的项目。

   **要避免此错误，请创建两个路径：一个用于具有发起人ID的项目，另一个用于没有发起人ID的项目。**

1. 通过单击路由器和读取记录模块之间的扳手图标，在两个模块之间添加路由器。 设置名为“发起人存在”的过滤器，并将条件设置为“发起人ID存在”。

   ![Set Get variables图像5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. 单击路由器以创建另一条路径。 从电子邮件应用程序添加发送电子邮件模块。

   + 在“收件人”字段中输入您自己的电子邮件地址。
   + 在“主题”字段中，键入“当前项目信息”。
   + 在内容字段中，放置项目名称、描述和发起人。
   + 您无法从读取记录模块提取赞助者名称输出。 您只能从位于路由器之前的搜索模块访问发起人ID。 您需要找到一种从另一条路由器路径访问发起人名称的方法。

   ![Set Get variables图像6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. 现在单击“确定”，并将此模块重命名为“发送项目信息”

   **使用Set/Get变量在不同路径之间共享数据。**

1. 在“查找发起人姓名”模块之后，添加一个“设置变量”工具模块。

   + 将“赞助商名称”作为变量名称。
   + 将变量生命周期保留为一个周期。
   + 将字段映射到查找发起人名称模块的名称输出。

1. 单击“确定”，然后将模块重命名为“设置赞助者名称”。

   ![Set Get variables图像7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. 接下来，在路由器和发送电子邮件模块之间单击鼠标右键，以添加“获取变量”工具模块。 在Variable name字段中输入“Sponser name”。
1. 单击“确定”。 将模块重命名为“获取赞助商名称”。

   ![Set Get variables图像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. 返回发送电子邮件模块，并将获取赞助者名称模块中的值映射到内容字段。 单击“确定”。

   ![Set Get variables图像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >在测试场景之前，我们建议限制您处理的项目数量以避免收到大量电子邮件。

1. 转到Workfront试用版，然后找到Northstar Fashion Exhibitors Booth项目。 这是当前项目的一个发起人。 从URL复制项目ID。

   ![Set Get variables图像10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. 在您的场景中，单击查找当前项目模块。 通过单击绿色的“添加AND规则”按钮，将另一个条件添加到搜索条件中。 指定ID必须与复制的项目ID相同。 单击“确定”。
1. 保存方案，然后单击运行一次。
1. 检查执行检查员以及您收到的电子邮件。

   ![Set Get variables图像11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
