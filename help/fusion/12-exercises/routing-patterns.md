---
title: 路由模式
description: 强化路由和备用路由的概念，而无需实际处理任何其他API。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 路由模式

强化路由和备用路由的概念，而无需实际处理任何其他API。

## 练习概述

使用Set Variable模块通过多个路径发送一个数字，以了解筛选器和回退在路由时的行为。

![路由模式图像1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 要遵循的步骤

1. 创建一个新方案，并将其命名为“路由模式和回退”。
1. 对于触发器，添加设置变量工具模块。 为变量名称输入“My Number”，将变量生命周期保留为一个周期，并将变量字段设置为“75”。

   ![路由模式图像2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 添加另一个模块，然后选择路由器模块。 对于这两个路径，选择“增量函数”工具，然后单击“确定”，而不对每个路径进行任何更改。

   + 对于第一个路径，请创建一个过滤器，将其命名为“Less than 100”，并将条件设置为 [我的号码] 少于100人。

   + 对于第二个路径，请创建一个过滤器，将其命名为“Less than 1000”，并将条件设置为 [我的号码] 少于1000。 请确保对两者都使用数值运算符。

   ![路由模式图像3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![路由模式图像4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 单击运行一次，然后观看包沿着“小于100”路径依次传递。
1. 然后，将设置变量模块字段更改为950并再次运行。 看着它沿着第二条路跑。
1. 单击路由器并添加一条路径。 添加增量函数工具模块。 对于过滤器，单击“后备路由”复选框。 请注意指向该路径的箭头如何更改为脱字符号，指示它是回退路由。

   ![路由模式图像5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 将Set variable编号更改为9500并运行一次。 由于该数字不小于100或小于1000，因此该捆绑包将沿回退路由传输。

如果使用“递增”函数工具模块再添加一个路径，但未设置过滤器，则再次单击“运行”时会出现什么情况？ 将添加第四个路由后，是否将捆绑包沿备援路由下传？

+ 不需要，因为没有设置过滤器，每个包将始终沿此路径而不是回退路径向下传送。
