---
title: 创建矩阵报告
description: 了解矩阵报告何时有用，以及如何在 Workfront 中创建矩阵报告。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: 6afb57b983b094f9bc0c082a160453ecb394ca8e
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 75%

---

# 创建矩阵报告

在本视频中，您将了解到：

* 矩阵报告何时有用
* 以及如何创建矩阵报告

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on)

## 创建矩阵报表活动

[单击此处](/help/assets/create-matrix-report-activities.pdf)下载此页面的 PDF。

### 活动1：创建矩阵报表

创建一个矩阵报告，其中显示每个状态中有多少请求，并按请求队列排序。这可以让您快速了解投入的工作量以及您跟进工作的情况。

建议在行分组上显示请求队列。状态显示为列分组。将报表命名为“按状态请求和请求队列”。

### 答案1

1. 从 **[!UICONTROL Main Menu]** 中选择 **[!UICONTROL Reports]**。
1. 单击 **[!UICONTROL New Report]** 选项，并选择 **[!UICONTROL Issue]**。
1. 转到 **[!UICONTROL Groupings]** 选项卡，并单击 **[!UICONTROL Switch to Matrix Grouping]**。
1. 对于 [!UICONTROL Row Groupings]，选择 **[!UICONTROL Project]** > **[!UICONTROL Name]**。
1. 对于 [!UICONTROL Column Grouping]，选择 **[!UICONTROL Issue]** > **[!UICONTROL Status]**。

   ![创建新的问题报告分组的屏幕图像](assets/matrix-report-groupings.png)

1. 转到 **[!UICONTROL Filters]** 选项卡。
1. 为了确保您只会看到活跃的请求队列中的请求，请添加以下过滤规则：

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Equal] > [!UICONTROL Current]
   * [!UICONTROL Queue Definition] > [!UICONTROL Is Public] > [!UICONTROL Not Equal] > [!UICONTROL None]（这就是我们通过将“队列定义”分配给一个公共选项来知道某个项目实际上是一个请求队列的方式。）

1. 单击 **[!UICONTROL Save + Close]**。在系统提示输入报表名称时，键入“按状态请求和请求队列”。

   ![创建新的问题报告过滤器的屏幕图像](assets/matrix-report-filters.png)
