---
title: 创建 ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 表达式
description: 了解如何在Adobe [!DNL Workfront]的计算字段中使用和创建ADD表达式。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
TQID: 'https://experienceleague.adobe.com/22KjuMtDdhm9A6JohWlThfOHwKcegLwT3nuFO--70N4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 91%
---
# 创建 ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 表达式

在本视频中，您将了解到：

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 表达式计算什么
* 如何在计算字段中创建 ADDWEEKDAYS 数据表达式

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on&enablevpops=1)

## 其他示例

以下是 Adobe Workfront 客户创建的一些其他 ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 表达式。

**原本的完成日期**

客户想知道根据实际开始日期和规划持续时间任务应该何时完成。 在这种情况下，预计完成日期不起作用，因为如果任务延迟，它可能会发生变化，而如果之前的任务出现延误，则规划完成日期也没有帮助。

创建的表达式为ADDDAYS({actualStartDate}，{durationMinutes}/480)

持续时间字段中的时间以分钟为单位存储。 因此，在此表达式中，如果要以天为单位反映时间，则“持续时间”字段不能独立。 为此，持续时间必须除以 480 分钟（480 分钟 = 8 小时 = 1 天）

这就是为什么第二个值槽包含（持续时间/480）。


**发票完成日期**

此示例不仅使用 ADDDAYS 表达式，还使用预先创建并保存在自定义表单中的自定义字段。

客户通过标题为“发票提交日期”的自定义日期字段捕获发票提交的日期。

提交后，发票必须在 30 天内填写并归档。 为了自动生成完成和归档日期，ADDDAYS 计算字段与“发票提交日期”自定义字段一起使用。 表达式如下所示：

ADDDAYS({DE:Invoice Submission Date}，30)
