---
title: 路由模式练习
description: 强化路由和回退路由的概念，而无需实际处理任何其他 API。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,noCatalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '361'
ht-degree: 100%

---

# 路由模式练习

强化路由和回退路由的概念，而无需实际处理任何其他 API。

## 练习概述

使用“设置变量”模块，通过多个路径发送数字，以了解过滤器和回退项目在路由时的行为。

![路由模式图像 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 应遵循的步骤

1. 创建一个新场景并将其命名为“路由模式和回退”。
1. 对于触发器，添加“设置变量”工具模块。将“我的号码”作为变量名称，将“变量存留期”保留为“一个”周期，并将“变量”字段设置为“75”。

   ![路由模式图像 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 添加另一个模块并选择路由器模块。对于这两条路径，选择增量函数工具，然后单击“确定”，而不对每条路径进行任何更改。

   + 对于第一条路径，创建一个过滤器，将其命名为“小于 100”，并将条件设置为[我的号码]少于 100。

   + 对于第二条路径，创建一个过滤器，将其命名为“小于 1000”，并将条件设置为[我的数量]少于 1000。确保对两者都使用数字运算符。

   ![路由模式图像 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![路由模式图像 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 单击“运行一次”，然后观察捆绑包沿着“小于 100”路径传递。
1. 然后将“设置变量”模块字段更改为 950 并再运行一次。观察它沿着第二条路径传递。
1. 单击该路由器并再添加一条路径。添加增量功能工具模块。对于过滤器，单击“回退路由”复选框。请注意指向该路径的箭头如何变为插入符号，这表明它是回退路径。

   ![路由模式图像 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 将“设置变量”数值更改为 9500 并运行一次。由于该数量既不小于 100，也不小于 1000，因此该捆绑包会沿着回退路径传递。

如果您使用增量功能工具模块再添加一条路径，但没有设置过滤器，那么当您再次单击“运行一次”时会发生什么情况？在添加第四条路径后，捆绑包是否会沿着回退路径传递？

+ 不会，因为如果没有设置过滤器，每个捆绑包都会始终沿着这条路径传递，而不是回退路径。
