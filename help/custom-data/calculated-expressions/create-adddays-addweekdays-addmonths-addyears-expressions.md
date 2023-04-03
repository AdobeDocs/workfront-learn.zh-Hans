---
title: 创建ADDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS表达式
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
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 创建ADDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS表达式

在此视频中，您将学习：

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR表达式的计算结果
* 如何在计算字段中创建ADDWEEKDAYS数据表达式

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## 其他示例

以下是Adobe Workfront客户创建的其他一些ADDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR表达式。

**本该由**

客户希望了解任务应何时根据实际起始日期和计划持续时间完成。 在这种情况下，预计完成日期将不起作用，因为如果任务延迟，它可以移动；如果先前任务存在延迟，计划完成日期将不起作用。

创建的表达式为ADDAYS({actualStartDate},{durationMinutes}/480)

“持续时间”字段中的时间以分钟为单位进行存储。 因此，在此表达式中，如果时间要以天为单位反映，则持续时间字段不能处于孤立状态。 要实现此目的，持续时间必须除以480分钟（480分钟= 8小时= 1天）

这就是第二个值插槽包含的原因（持续时间/480）。


**发票完成日期**

此示例不仅使用ADDAYS表达式，而且还包含以自定义表单预先创建和保存的自定义字段。

客户通过标题为“发票提交日期”的自定义日期字段获取发票提交日期。

发票一经提交，必须在30日内填妥并填报。 要自动生成完成日期和归档日期，将使用ADDAYS计算字段和“发票提交日期”自定义字段。 表达式如下所示：

ADDDAYS（{DE：发票提交日期},30）
