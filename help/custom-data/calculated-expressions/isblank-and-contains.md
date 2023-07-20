---
title: 使用ISBLANK和CONTAINS表达式
description: 了解如何在Adobe的计算字段中使用和创建ISBLANK和CONTAINS表达式 [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 使用ISBLANK和CONTAINS表达式

CONTAINS和ISBLANK表达式都用于提供简单的true或false值。 区别在于ISBLANK表达式检查字段是否完全保留值，而CONTAINS文本表达式在字段内查找特定字符串。

例如，要查看某个项目是否有说明，请使用ISBLANK表达式。 如果描述字段为空，则表达式返回值true。 如果描述字段不为空，则返回值false。

![具有利用率报告的工作负载均衡器](assets/isblank01.png)

要在描述中查找特定值（如“慈善事件”），请使用CONTAINS文本表达式。 如果它在描述中找到“慈善事件”，则计算字段显示“true”。 如果找不到“慈善活动”，则显示“false”。

![具有利用率报告的工作负载均衡器](assets/isblank02.png)

## ISBLANK

ISBLANK文本表达式包括表达式的名称和一个数据点。

**ISBLANK({data point})**

![具有利用率报告的工作负载均衡器](assets/isblank03.png)

在上面的示例中（您希望了解项目是否具有说明），表达式将为：

ISBLANK({description})

## CONTAINS

CONTAINS文本表达式包括表达式名称、要查找的单词或短语以及要查找的字段。

**CONTAINS(“短语”，{fields})**

请确保在要查找的单词或短语周围加上引号，否则表达式将无效。

在上述示例中（在项目描述中查找“慈善事件”），表达式将为：

**CONTAINS(“慈善活动”，{description})**

![具有利用率报告的工作负载均衡器](assets/isblank04.png)

**注释**： CONTAINS表达式区分大小写。 例如，如果“Charity Event”在描述字段中大写，则表达式中会将该短语大写。

**CONTAINS(“慈善活动”，{description})**

如果要查看值是否存在，可以使用ISBLANK和CONTAINS表达式。 但是，知道该值是什么、实际查看它或具有某种类型的描述符以提供更好的见解可能更有用。

例如，您不想只是知道项目已从请求转换，而是想知道原始请求的名称。

在这种情况下，可将CONTAINS表达式与IF表达式结合使用。

ISBLANK和CONTAINS文本表达式经常与IF文本表达式一起使用。
