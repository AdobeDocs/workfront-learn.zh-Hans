---
title: 数据结构
description: 将数据从源文件转换为目标文件。 （应介于60到160个字符之间，但为58个字符）
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11054
thumbnail: KT11054.png
exl-id: 06a39a87-23f3-4d4a-995e-d32fb9c5f50d
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# 数据结构

将数据从源文件转换为目标文件。

## 练习概述

打开包含时间条目列表的CSV文件。 这些时间条目是指多个用户在特定日期内记录的分钟数。 其目标是获取此信息并生成一个新的CSV，以显示每个用户每天记录的总时间（以小时为单位）。

![数据结构图像1](../12-exercises/assets/data-structures-walkthrough-1.png)

![数据结构图2](../12-exercises/assets/data-structures-walkthrough-2.png)


在此方案中，您将打开一个文件，其中包含工作分钟数的时间条目列表，包括日期和时间、输入的分钟数以及输入者的电子邮件地址。 有100个时间条目，有些是由同一个人做的，有些是在同一天做的。

要生成一个文件，其中显示每个人每天工作的总时间（以小时为单位），您将执行以下步骤：

1. 在触发器模块中，从Workfront文件夹获取文件。 下载文件。
1. 在第一个CSV模块中，解析时间条目数据以针对每次条目输出一个包。 这是迭代器。
1. 第一个“工具”模块是数字聚合器。 这将对所有分钟数求和，并按电子邮件地址，然后按日期对行进行分组。 结果是按电子邮件地址每天工作的总分钟数。
1. 第二个“工具”模块是“设置变量”模块。 使用此设置分钟数的格式，以除以60，并四舍五入为2位小数。
1. 在第二个CSV模块中，设置输出文件。
1. 在最终模块中，将CSV文件上传到Workfront。

## 要遵循的步骤

**从Workfront下载文件。**

1. 在Workfront的“Fusion Exercise Files”文件夹中，选择“_Fusion1.0JanTime.csv”，然后单击“文档详细信息”。
1. 从URL地址复制第一个ID号。
1. 创建新方案。 将其命名为“创建和使用数据结构”。
1. 从Workfront应用程序中的下载文档模块开始。
1. 设置您的Workfront连接，并包含您从Workfront URL复制的文档ID。

   ![数据结构图3](../12-exercises/assets/data-structures-walkthrough-3.png)

   **解析时间条目数据。**

1. 添加其他模块，选择解析CSV。
1. 为7列设置解析CSV 。 选中CSV包含标题框。 选择逗号分隔符类型，然后将数据放入CSV字段。

   ![数据结构图像4](../12-exercises/assets/data-structures-walkthrough-4.png)

1. 单击运行一次以查看输出。
1. 打开执行检查器，以查看解析CSV模块的输入和输出。 有一个包（CSV文件）作为输入，多个包作为输出（CSV文件中每行都有一个包）。 它应该如下所示：

   ![数据结构图5](../12-exercises/assets/data-structures-walkthrough-5.png)

   **接下来，将数据转换为所需的输出表单，聚合时间总计以小时而不是分钟表示。**

1. 添加数值聚合工具模块。
1. 选择源模块（即解析CSV模块）。
1. 为聚合函数选择SUM。
1. “值”字段是CSV文件中的第7列。 这是每个用户记录的分钟数。
1. 要按组汇总字段，请单击高级设置，然后将分组设置为电子邮件（列4）、日期（列5）。

   + 这将对电子邮件和日期的每个组合进行总和。 请务必在第4列和第5列之间加逗号。 以后将使用此分隔符作为分隔符。

   **映射面板应当如下所示：**

   ![数据结构图6](../12-exercises/assets/data-structures-walkthrough-6.png)

1. 单击运行一次以检查聚合输出。

   **输出包应如下所示：**

   ![数据结构图7](../12-exercises/assets/data-structures-walkthrough-7.png)

   **现在，将汇总的分钟数转换为小时。**

1. 添加其他工具模块，选择设置变量。
1. 将变量命名为“小时”。
1. 将变量值设置为formatNumber(result/60;2;.;,)

   **映射面板应当如下所示：**

   ![数据结构图8](../12-exercises/assets/data-structures-walkthrough-8.png)

   **接下来，为输出文件设置值。 您希望使用userID和日期值进行分组。 您还需要计算的小时数。**

1. 使用聚合器创建CSV（高级）添加另一个模块 — CSV模块。
1. 源模块是工具 — 数值聚合器。
1. 单击数据结构字段旁边的添加，并将我们的数据结构命名为“记录时间的每日总和”。
1. 单击添加项目以创建第一个项目。
1. 将项目命名为“UserID”，并将类型设置为“Text”。 单击添加。
1. 再次单击添加项目以创建第二个项目。
1. 将项目命名为“Date”，将类型设置为“Date”，然后单击“Add”。
1. 再次单击添加项目。
1. 将项目命名为“小时”，将类型设置为“数字”，然后单击“添加”。

   **您的数据结构应如下所示：**

   ![数据结构图像9](../12-exercises/assets/data-structures-walkthrough-9.png)

1. 单击保存以完成记录时间的每日总和数据结构。

   **现在，您可以为刚刚创建的三个字段提供值。 您应会在CSV映射面板中看到这三个字段。**

1. 单击“用户ID”字段，然后从“常规函数”选项卡中选择GET。 在第一个参数中，从文本和二进制函数选项卡中放置SPLIT。 SPLIT函数的第一个参数是Key字段。 添加逗号作为分隔符，添加1作为索引。 这表示您希望GET检索键值数组中的第一个字段。
1. 将此表达式复制到“日期”字段。 将索引从1更改为2，以GET数组中的第二个值。
1. 对于“小时”字段，从“设置变量”工具中添加“小时”字段。

   **您的CSV映射面板应当如下所示：**

   ![数据结构图像10](../12-exercises/assets/data-structures-walkthrough-10.png)

   **如果现在运行方案，您应会看到以下输出：**

   ![数据结构图11](../12-exercises/assets/data-structures-walkthrough-11.png)

   **现在，添加一个模块以获取此输出并将其作为文档上传到Workfront中的现有项目。**

1. 在Workfront中打开项目，并从URL复制项目ID。
1. 返回到Fusion中的方案，然后从Workfront应用程序中添加另一个模块 — 上传文档模块。
1. 将项目ID粘贴到“相关记录ID”字段中。
1. 为相关记录类型选择项目。
1. 为源文件选择映射选项。
1. 对于“文档名称”，请使用您下载的文件名，并在其前面添加“已更新”。
1. 对于文件内容，请使用创建CSV模块中的文本输出。

   **映射面板应当如下所示：**

   ![数据结构图12](../12-exercises/assets/data-structures-walkthrough-12.png)

1. 单击确定并保存方案。
1. 单击运行一次以运行方案。

   **检查“上载文档”模块中的执行检查器，以确认文档已上载。**

   ![数据结构图13](../12-exercises/assets/data-structures-walkthrough-13.png)
