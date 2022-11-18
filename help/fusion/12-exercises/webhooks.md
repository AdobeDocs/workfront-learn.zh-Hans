---
title: Webhooks
description: 了解如何创建、触发和管理Webhook启动的方案。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Webhooks

了解如何创建、触发和管理Webhook启动的方案。

## 练习概述

此方案的目的是创建一个应用程序，将其销售到便利店，以便他们能够轻松确定客户是否年龄足够大，可以购买酒精。 收银员只需将客户的姓名和出生日期发布到他们提供的URL即可。 该帖子将触发情景，该情景将计算答案并将其返回给请求者。

1. 方案由三个Web挂接组成。
1. 触发器模块是一个自定义WebHook，用于侦听帖子。
1. 当它收到帖子时，会将其输出到下一个模块之一。
1. 下一个模块返回对请求者的响应。

   ![Webhooks图像1](../12-exercises/assets/webhooks-walkthrough-1.png)

## 要遵循的步骤

**设置触发器网页钩。**

1. 创建新方案并将其命名为“Using webhooks”。
1. 对于触发器，从Webhooks应用程序中添加自定义Webhook模块。
1. 单击添加以创建新的Webhook。
1. 输入“饮用年龄应用程序”的Webhook名称。
1. 将IP限制留空，这意味着任何人都可以向其发送数据。
1. 单击保存。


   ![Webhooks图像2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. 返回到Webhooks映射面板中，已为此特定Webhook创建URL。 单击“将地址复制到剪贴板”以复制该URL。
1. 单击确定。
1. 单击运行一次。
1. 使用Postman中的URL将名称和出生日期发送到您的自定义WebHook。 有关设置Postman的说明，请参阅 [Webhooks演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) 教程。

   **Webhooks模块面板应当如下所示：**

   ![Webhooks图像3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **Webhook现在处于侦听数据以确定数据结构的状态。**

1. 您可以定义期望获得的有效负载的数据结构（稍后将讨论数据结构）。 如果您未定义数据结构，则Fusion将在发送帖子时自动确定数据结构。
1. 在Postman端，您希望发送到复制的URL。 帖子应包含基本的表单数据。 在本例中，您需要三个字段：名称、胎日期和clientToken。

   ![Webhooks图像4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. 单击从Postman发送后，您应会收到一个指示，表示已接受该帖子。
1. 这是您的方案将显示数据结构已成功确定的位置。
1. 通过打开执行检查器，可以看到已收到数据。

   ![Webhooks图像5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **设置客户端令牌的路由。**

1. 将路由器添加到触发模块。
1. 在上方路径中，添加Webhook响应模块。 当客户端令牌不匹配时，这将是我们的路径。
1. 将状态设置为401。
1. 将Body设置为{&quot;error&quot;:&quot;无法验证请求。 请检查您的clientToken&quot;}。

   ![Webhooks图像6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. 在路由器和Webhook响应模块之间创建过滤器。 将其命名为“客户端令牌不匹配”。
1. 对于条件，使用触发器模块中的clientToken字段，并与数字5121933进行数字“不等于”比较。

   ![Webhooks图像7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. 在底部路径中，添加另一个Webhook响应模块。 这将是客户端令牌匹配时的路径。
1. 将状态设置为200。
1. 在设置主体时，使用映射面板函数来测试人员是21岁还是21岁。 如果是，则返回“你够大喝的！”，否则返回“你不走运……”

   ![Webhooks图像9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. 在路由器和Webhook响应模块之间在下路径上创建过滤器。 将其命名为“客户端令牌匹配”。
1. 对于条件，使用触发器模块中的clientToken字段，并与数字5121933进行数字“等于”比较。


   ![Webhooks图像8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. 单击运行一次下的计划按钮以激活您的方案，以便每当有新帖子时都会收到该帖子，向下任一路径并生成响应。
