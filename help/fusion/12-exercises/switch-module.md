---
title: 交换机模块
description: 了解在需要执行更复杂或动态的数据转换时如何使用Switch模块。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# 交换机模块

了解在需要执行更复杂或动态的数据转换时如何使用Switch模块。

## 练习概述

在您的试用中搜索直邮项目，然后根据在附加到项目的自定义字段中选择的值更改每个项目的名称。

![交换机模块图像1](../12-exercises/assets/switch-module-walkthrough-1.png)

## 要遵循的步骤

1. 创建一个新方案，并将其命名为“使用交换机模块”。
1. 对于trigger模块，请使用Workfront Search模块。
1. 设置Workfront连接，并将记录类型设置为“项目”。
1. 在搜索条件中，指定您只想在渠道自定义字段中查看具有值的项目。
1. 对于输出，选择ID、名称、参考编号和渠道自定义字段。

   ![交换机模块图像2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. 从“工具”添加“交换机”模块。
1. 对于输入字段，映射搜索模块中的渠道自定义字段。

   ![交换机模块图像3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. 接下来，为来自渠道自定义字段的每个可能值添加案例。 可能的值将放在“模式”字段中。 您希望输出字段包含特定的3个字母的代码，后跟项目参考编号，然后是项目名称。

   **您的映射面板应如下所示：**

   ![交换机模块图像4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. 您可以根据需要添加任意数量的其他用例。 请注意底部的Else字段。 如果输入值不匹配任何大小写，则将使用此值。

   **更新Workfront中的项目名称。**

   ![交换机模块图像5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. 添加Workfront更新记录模块。
1. 在ID字段中，将映射到触发器模块中的ID。
1. 将“记录类型”设置为“项目”。
1. 从选择要映射的字段部分中选择名称字段，并将其映射到交换机模块的输出。
1. 保存方案并运行一次。 在测试驱动器中查看更新的项目名称。
