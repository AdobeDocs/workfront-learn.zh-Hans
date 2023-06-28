---
title: 数据结构
description: 将数据从源文件转换为目标文件。 （应为60至160个字符，但实为58个字符）
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11054
thumbnail: KT11054.png
exl-id: 06a39a87-23f3-4d4a-995e-d32fb9c5f50d
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# 数据结构

将数据从源文件转换为目标文件。

## 练习概述

打开包含时间条目列表的CSV文件。 这些时间条目表示多个用户在某些天中记录的分钟数。 目标是获取此信息并生成一个新的CSV，其中显示每个用户每天记录的总时间（小时）。

![数据结构图像1](../12-exercises/assets/data-structures-walkthrough-1.png)

![数据结构图像2](../12-exercises/assets/data-structures-walkthrough-2.png)


在此方案中，您将打开一个文件，其中包含工作分钟数的时间条目列表，包括日期和时间、输入分钟数以及输入该条目的用户的电子邮件地址。 共有100个时间条目，其中一些由同一人创建，其中一些条目与其他条目在同一天创建。

要生成一个显示每人每天工作总时间（小时）的文件，您将按照以下步骤操作：

1. 在触发器模块中，从Workfront文件夹获取文件。 下载文件。
1. 在第一个CSV模块中，解析时间条目数据以便为每个时间条目输出一个捆绑。 这是一个迭代器。
1. 第一个“工具”模块是一个数值汇总。 这将计算所有分钟数的总和，并按电子邮件地址、然后按日期对行分组。 结果按电子邮件地址显示每天的总工作分钟数。
1. 第二个Tools模块是Set Variable模块。 使用此项可设置分钟数除以60的格式，并舍入为2位小数。
1. 在第二个CSV模块中，设置输出文件。
1. 在最后一个模块中，将CSV文件上传到Workfront。

## 要遵循的步骤

**从Workfront下载文件。**

1. 在Workfront“Fusion Experience Files”文件夹中，选择“_Fusion1.0JanTime.csv”，然后单击“文档详细信息”。
1. 从URL地址复制第一个ID号。
1. 创建新方案。 将其命名为“创建和使用数据结构”。
1. 从Workfront应用程序中的“下载文档”模块开始。
1. 设置您的Workfront连接，并包括从Workfront URL复制的文档ID。

   ![数据结构图像3](../12-exercises/assets/data-structures-walkthrough-3.png)

   **解析时间条目数据。**

1. 选择解析CSV ，添加另一个模块。
1. 为7列设置分析CSV 。 选中CSV包含标头框。 选择逗号分隔符类型并将数据放入CSV字段中。

   ![数据结构图像4](../12-exercises/assets/data-structures-walkthrough-4.png)

1. 单击运行一次以查看输出。
1. 打开执行检查器以查看“解析CSV”模块的输入和输出。 有一个捆绑（一个CSV文件）作为输入，多个捆绑作为输出（CSV文件中的每行一个捆绑）。 它应该看起来像这样：

   ![数据结构图像5](../12-exercises/assets/data-structures-walkthrough-5.png)

   **接下来，将数据转换为所需的输出表单，聚合时间总计以小时而不是分钟表示。**

1. 添加数值聚合工具模块。
1. 选择源模块，即解析CSV模块。
1. 为聚合函数选择SUM。
1. “值”字段是CSV文件中的第7列。 这是每个用户记录的分钟数。
1. 要按组对字段求和，请单击“高级设置”，并将“分组依据”设置为“电子邮件”（列4）、“日期”（列5）。

   + 这会对电子邮件和日期的每种组合进行求和。 请确保在列4和列5之间放置逗号。 稍后将用作分隔符。

   **您的映射面板应如下所示：**

   ![数据结构图像6](../12-exercises/assets/data-structures-walkthrough-6.png)

1. 单击运行一次以检查聚合输出。

   **输出捆绑包应如下所示：**

   ![数据结构图像7](../12-exercises/assets/data-structures-walkthrough-7.png)

   **现在将汇总分钟数转换为小时数。**

1. 添加另一个工具模块，选择“设置变量”。
1. 将变量命名为“Hours”。
1. 将变量值设置为formatNumber(result/60；2；。；，)

   **您的映射面板应如下所示：**

   ![数据结构图像8](../12-exercises/assets/data-structures-walkthrough-8.png)

   **接下来，获取为输出文件设置的值。 您希望用户ID和日期值用于分组。 您还需要已计算的小时数。**

1. 使用聚合器创建CSV（高级）添加另一个模块 — CSV模块。
1. 源模块是工具 — 数值汇总。
1. 单击Data structure字段添加并将我们的数据结构命名为“Time Logged Daily Sum”。
1. 单击“添加项目”以创建第一个项目。
1. 将项目命名为“UserID”并将类型设置为“Text”。 单击“添加”。
1. 再次单击添加项目以创建第二个项目。
1. 将项目命名为“日期”，将类型设置为“日期”，然后单击“添加”。
1. 再次单击“添加项目”。
1. 将项目命名为“小时”，将类型设置为“数字”，然后单击“添加”。

   **您的数据结构应如下所示：**

   ![数据结构图像9](../12-exercises/assets/data-structures-walkthrough-9.png)

1. 单击“保存”以完成“每日总计记录时间”数据结构。

   **现在，您提供刚刚创建的三个字段的值。 您应会在CSV映射面板中看到这三个字段。**

1. 单击UserID字段，然后从常规函数选项卡中选择GET。 在第一个参数中，将SPLIT放置在text和binary函数选项卡中。 SPLIT函数的第一个参数是Key字段。 添加逗号作为分隔符，添加1作为索引。 这表示您希望GET检索键数组中的第一个字段。
1. 将此表达式复制到“日期”字段中。 将索引从1更改为2，以GET数组中的第二个值。
1. 对于小时字段，添加设置变量工具中的小时字段。

   **您的CSV映射面板应如下所示：**

   ![数据结构图像10](../12-exercises/assets/data-structures-walkthrough-10.png)

   **如果现在运行该方案，您应会看到以下输出：**

   ![数据结构图像11](../12-exercises/assets/data-structures-walkthrough-11.png)

   **现在，添加一个模块以获取此输出，并将其作为文档上传到Workfront中的现有项目。**

1. 在Workfront中打开项目，并从URL中复制项目ID。
1. 返回到Fusion中的场景，然后从Workfront应用程序添加另一个模块 — “上传文档”模块。
1. 将项目ID粘贴到“相关记录ID”字段中。
1. 为相关记录类型选择“项目”。
1. 为源文件选择映射选项。
1. 对于“文档名称”，使用您下载的文件名，在其前面添加“已更新”。
1. 对于文件内容，使用创建CSV模块的文本输出。

   **您的映射面板应如下所示：**

   ![数据结构图像12](../12-exercises/assets/data-structures-walkthrough-12.png)

1. 单击确定并保存方案。
1. 单击运行一次以运行方案。

   **检查“上传文档”模块中的执行检查器，确认文档已上传。**

   ![数据结构图像13](../12-exercises/assets/data-structures-walkthrough-13.png)
