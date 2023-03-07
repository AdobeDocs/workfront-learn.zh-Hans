---
title: 创建ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS表达式
description: 了解如何在Adobe的计算字段中使用和创建ADD表达式 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 创建ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS表达式

在本视频中，您将了解：

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR表达式计算的内容
* 如何在计算字段中创建ADDWEEKDAYS数据表达式

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## 其他示例

以下是Adobe Workfront客户创建的一些其他ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR表达式。

**应该完成日期**

客户希望根据实际开始日期和计划持续时间知道何时应完成任务。 在这种情况下，“预计完成日期”不起作用，因为如果任务延迟，则它可以移动；如果先前任务延迟，则“计划完成日期”不起作用。

创建的表达式为ADDDAYS({actualStartDate}，{durationMinutes}/480)

“持续时间”字段中的时间以分钟为单位存储。 因此，在此表达式中，如果时间要反映在天数中，则Duration字段不能独立显示。 要实现这一点，持续时间必须除以480分钟（480分钟= 8小时= 1天）

这就是第二个值槽包含(Duration/480)的原因。


**发票完成日期**

此示例不仅包括使用ADDDAYS表达式，还包括以前在自定义表单中创建和保存的自定义字段。

客户通过名为“发票提交日期”的自定义日期字段捕获提交发票的日期。

发票一经提交，必须在30天内填妥并归档。 为了自动生成完成日期和提交日期，ADDDAYS计算字段与“发票提交日期”自定义字段一起使用。 表达式如下所示：

ADDDAYS（{DE：发票提交日期}，30）
