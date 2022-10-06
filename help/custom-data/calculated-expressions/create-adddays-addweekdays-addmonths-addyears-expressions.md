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
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 创建ADDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS表达式

在此视频中，您将学习：

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR表达式的计算结果
* 如何在计算字段中创建ADDWEEKDAYS数据表达式

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## 其他示例

以下是一些额外的ADDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR表达式Adobe [!DNL Workfront] 客户已创建。

**本该由**

客户希望了解任务应何时根据实际起始日期和计划持续时间完成。 在这种情况下，预计完成日期将不起作用，因为如果任务延迟，它可以移动；如果先前任务存在延迟，计划完成日期将不起作用。

创建的表达式为ADDAYS(实际开始日期，（持续时间/480）)

“持续时间”字段中的时间以分钟为单位进行存储。 因此，在此表达式中，如果时间要以天为单位反映，则持续时间字段不能处于孤立状态。 要实现此目的，持续时间必须除以480分钟（480分钟= 8小时= 1天）

这就是第二个值插槽包含的原因（持续时间/480）。


**发票完成日期**

此示例包括表达式中已在系统中创建并保存的另一个计算字段。

客户在自定义表单中通过标题为“发票提交日期”的自定义日期字段获取发票提交日期。 提交后，他们有30天时间完成并提交发票。 要自动生成完成日期和归档日期，他们使用ADDDDAYS和“发票提交日期”字段创建了一个计算字段。 表达式如下所示：

ADDAYS（发票提交日期，30）
