---
title: Webhook
description: 了解如何创建、触发和管理webhook启动的场景。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Webhook

了解如何创建、触发和管理webhook启动的场景。

## 练习概述

此方案的目的是创建一个应用程序，以便向便利店销售，以便他们能够轻松确定客户是否达到购买酒精的年龄。 出纳只需将客户的姓名和出生日期发布到他们提供的URL即可。 该帖子将触发场景，该场景将计算答案并将其返回给请求者。

1. 场景包含三个Webhook。
1. 触发器模块是一个自定义webhook，用于侦听帖子。
1. 当它收到帖子时，会将其输出到下一个模块之一。
1. 下一个模块将返回对请求者的响应。

   ![Webhook图像1](../12-exercises/assets/webhooks-walkthrough-1.png)

## 要遵循的步骤

**设置触发器webhook。**

1. 创建一个新方案，并将其命名为“使用Webhook”。
1. 对于触发器，从Webhook应用程序添加自定义webhook模块。
1. 单击“添加”创建新的Webhook。
1. 输入“饮酒年龄应用程序”的Webhook名称。
1. 将IP限制保留为空，这意味着任何人都可以将数据发送到其中。
1. 单击保存。


   ![Webhook图像2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. 返回Webhook映射面板，已为此特定webhook创建URL。 单击“将地址复制到剪贴板”以复制该URL。
1. 单击“确定”。
1. 单击运行一次。
1. 使用Postman中的URL向您的自定义webhook发送名称和出生日期。 有关设置Postman的说明，请参阅 [Webhook演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) 教程。

   **Webhooks模块面板应如下所示：**

   ![Webhook图像3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **webhook现在处于一种状态，它正在侦听数据以确定数据结构。**

1. 您可以定义预期获得的有效负载的数据结构（稍后将讨论数据结构）。 如果您未定义数据结构，Fusion将在发送帖子时自动确定数据结构。
1. 在Postman端，您希望发送到复制的URL。 帖子应包含基本表单数据。 对于此示例，您需要三个字段：Name、Birthdate和clientToken。

   ![Webhooks图像4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. 单击从Postman发送后，您应该会看到帖子已被接受的指示。
1. 此时，您的方案将显示已成功确定数据结构。
1. 通过打开执行检查器，您可以看到已收到数据。

   ![Webhooks图像5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **设置客户端令牌的路由。**

1. 将路由器添加到触发器模块。
1. 在上部路径中，添加Webhook响应模块。 当客户端令牌不匹配时，这是我们的路径。
1. 将状态设置为401。
1. 将正文设置为{&quot;error&quot;： &quot;Failed to authenticate request. 请检查您的clientToken“}。

   ![Webhooks图像6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. 在路由器和Webhook响应模块之间创建一个过滤器。 将其命名为“Client token not match”。
1. 对于Condition ，使用触发器模块的clientToken字段，并与数字5121933进行数字“不等于”比较。

   ![Webhooks图像7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. 在底部路径中，添加另一个Webhook响应模块。 当客户端令牌匹配时，这是我们的路径。
1. 将状态设置为200。
1. 在设置正文时，使用映射面板功能进行测试，以查看人员是否为21岁或以上。 如果是，则返回“您够大可以喝酒！”，否则返回“您不走运……”

   ![Webhooks图像9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. 在路由器与下路径的Webhook响应模块之间创建一个过滤器。 将其命名为“Client token does match”。
1. 对于Condition ，使用触发器模块的clientToken字段，并与数字5121933进行数字“等于”比较。


   ![Webhooks图像8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. 单击“运行一次”下的“计划”按钮可激活场景，以便每当有新帖子发布时，系统都会收到该帖子，然后沿着任一路径浏览并生成响应。
