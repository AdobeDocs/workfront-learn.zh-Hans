---
title: 路由模式
description: 强化您的路由和回退路由概念，而无需实际处理任何其他API。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 路由模式

强化您的路由和回退路由概念，而无需实际处理任何其他API。

## 练习概述

使用“设置变量”模块通过多个路径发送一个数字，以了解过滤器和回退在路由时的行为。

![路由模式图1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 要遵循的步骤

1. 创建新方案并将其命名为“路由模式和回退”。
1. 对于触发器，添加设置变量工具模块。 将“My Number”（我的数字）放在变量名称中，将变量生命周期保留为One个周期，然后将“Variable”（变量）字段设置为“75”。

   ![路由模式图2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 添加另一个模块，然后选择路由器模块。 对于这两个路径，选择“增量”函数工具，然后单击“确定”(OK)，而不对每个路径进行任何更改。

   + 对于第一个路径，创建一个过滤器，将其命名为“小于100”，然后将条件设置为 [我的号码] 少于100。

   + 对于第二个路径，创建一个过滤器，将其命名为“小于1000”，然后将条件设置为 [我的号码] 少于1000。 确保同时使用数值运算符。

   ![路由模式图3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![路由模式图4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 单击运行一次，并观看包向下传递“小于100”路径。
1. 然后，将“Set Variable”模块字段更改为950，并再次运行。 看着它沿着第二条路走。
1. 单击路由器并添加一条路径。 添加Increment函数工具模块。 对于过滤器，单击“回退路由”复选框。 请注意指向该路径的箭头如何变为尖角，表示它是回退路由。

   ![路由模式图5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 将Set variable number更改为9500，然后运行一次。 由于该数字不小于100或小于1000，因此包将沿回退路线传输。

如果您使用Increment函数工具模块再添加一个路径，但未设置过滤器，那么当您再次单击Run（运行）时会发生什么情况？ 包是否会在后退路由中添加第四条路由？

+ 不会，因为没有设置过滤器，每个包将始终沿此路径运行，而不是沿回退路由运行。
