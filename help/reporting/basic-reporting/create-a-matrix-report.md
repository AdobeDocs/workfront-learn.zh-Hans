---
title: 创建矩阵报表
description: 了解矩阵报表何时有用，以及如何在Workfront中创建矩阵报表。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 创建矩阵报表

在本视频中，您将了解：

* 矩阵报告何时有用
* 以及如何创建矩阵报告

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## 活动：创建矩阵报表

创建一个矩阵报告，以显示每个状态有多少请求，并按请求队列进行排序。 这可以让您快速了解投入的工作量以及您跟进工作的情况。

您希望请求队列显示在行分组中。 状态显示为列分组。 将报表命名为“按状态列出的请求和请求队列”。

## 答案

1. 选择 **[!UICONTROL Reports]** 从 **[!UICONTROL Main Menu]**.
1. 单击 **[!UICONTROL New Report]** 选项并选择 **[!UICONTROL Issue]**.
1. 转到 **[!UICONTROL Groupings]** 选项卡，然后单击 **[!UICONTROL Switch to Matrix Grouping]**.
1. 对象 [!UICONTROL Row Groupings]，选择 **[!UICONTROL Project]** > **[!UICONTROL Name]**.
1. 对象 [!UICONTROL Column Grouping]，选择 **[!UICONTROL Issue]** > **[!UICONTROL Status]**.

   ![用于创建新问题报告分组的屏幕图像](assets/matrix-report-groupings.png)

1. 转到 **[!UICONTROL Filters]** 选项卡。
1. 要确保只看到活动请求队列中的请求，请添加以下筛选规则：

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Equal] > [!UICONTROL Current]
   * [!UICONTROL Queue Definition] > [!UICONTROL Is Public] > [!UICONTROL Not Equal] > [!UICONTROL None] （通过将“队列定义”分配给某个公共选项，我们可了解项目实际上是请求队列。）

1. 单击 **[!UICONTROL Save + Close]**. 在系统提示输入报表名称时，键入“按状态请求和请求队列”。

   ![用于创建新问题报告过滤器的屏幕图像](assets/matrix-report-filters.png)
