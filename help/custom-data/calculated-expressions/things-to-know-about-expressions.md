---
title: 关于计算字段表达式的须知事项
description: 大致了解在  [!DNL Workfront] 中使用自定义计算字段时需要了解的概念列表。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: ht
source-wordcount: '959'
ht-degree: 100%

---

# 关于计算字段表达式的须知事项

这里是在 Workfront 中使用自定义计算字段时需要了解的概念列表。

## 表达式名称中大小写很重要

当涉及到表达式名称时，大小写很重要。最初编写表达式名称时，可以使用大写、小写或两者的混合。

![表达式名称中没有大写的错误消息](assets/T2K01.png)

但是，表达式必须全部写为大写字母，系统才能识别表达式并保存字段。



## 小时数以分钟为单位存储

Workfront 数据库中的小时数以分钟为单位存储。如果您引用“规划小时数”或“实际小时数”等字段，请除以 60 以显示以小时而不是分钟为单位的时间。

## 间距不影响表达式

编写表达式的推荐方法是每个表达式之间几乎没有间距。

* IF(ISBLANK({description}),&quot;No Description&quot;,&quot;Has Description&quot;)

![字段之间没有空格的表达式](assets/T2K02.png)

但是，如果间距可以帮助您了解正在发生的情况，则可以在表达式中添加一些间距。额外的空格不应阻止表达式收集或计算 [!DNL Workfront] 中的值。

* IF (ISBLANK ({description}), &quot;No Description&quot; , &quot;Has Description&quot; )

![字段之间有空格的表达式](assets/T2K03.png)

唯一不能在它们之间有空格的是字段和大括号。否则，您将收到错误消息，并且无法保存字段或自定义表单。

![字段名称和大括号之间的间距错误](assets/T2K04.png)

## 引号必须是直的

在表达式中使用引号时，请确保引号是直引号 (&quot;)。如果引号是弯曲的 (&quot;)，则 [!DNL Workfront] 系统将会继续显示“自定义表达式无效”消息。

![弯曲引号错误](assets/T2K05.png)

## 表单保存和对象编辑时的计算更新

这是需要理解的计算字段的一个重要方面。

除非重新计算自定义表单，否则计算字段中显示的信息将保持不变并会变得过时。

可以使用对象的“更多”菜单中的“重新计算表达式”选项来刷新表达式。

您想要查看问题已开放的天数。使用表达式 DATEDIFF 创建一个名为“Days Open”的计算字段。

* 字段名称 = 开放天数
* 表达式 = DATEDIFF({entryDate},$$TODAY)

保存后，问题首次创建或在 Workfront 中输入的时间与今天的日期之间的天数可以显示在对象的详细信息页面或报告视图中。

当第二天查看相同的详细信息页面或报告视图时，您预计该数字会增加 1。如果今天的数字是 5，那么明天应该是 6。接下类的一天应该是 7，然后是 8，等等。

然而，该字段仍将每天显示 5。该字段必须“重新运行”或重新计算以刷新信息。

要使用重新计算表达式选项更新字段：

* 单击对象的名称将其打开。
* 单击“更多”菜单。
* 从列表中选择重新计算表达式。

![重新计算对象中的表达式选项](assets/T2K06.png)

您还可以使用列表或报告中的“批量编辑”功能同时重新计算多个表达式。假设您创建了一个报告，其中显示了一个问题列表，其中“开放天数”计算显示在一列中。如果您想一次重新计算所有问题：

* 选择报告中的所有问题。
* 选择编辑选项可批量编辑所有选定的问题。
* 单击左侧的“自定义表单”标签，向下滚动到自定义表单部分。
* 选中“自定义表单”部分底部的“重新计算自定义表达式”框。
* 单击“保存更改”。

![重新计算多个对象的表达式选项](assets/T2K07.png)

屏幕刷新以显示计算字段中的更新信息。

**注释**：尽管还有其他方法可以更新或重新计算计算字段中的表达式，但这是最快、最简单的方法。

## 同一字段中不同形式的计算可能有所不同

将计算字段保存在自定义表单上并保存自定义表单后，计算字段就会添加到字段库中，以便可以在其他自定义表单上使用。

但是，如果表单 A 上有一个计算字段，并且表单 B 上有相同的计算字段，则最初可能会认为这些计算完全相同。情况并非总是如此。表单 A 上的计算字段可能会以完全不同的方式在表单 B 上进行计算。

从字段库中选择计算的自定义字段并将其添加到自定义表单时，会添加该字段，但计算结果为空。发生这种情况的一个原因是计算可能引用了其他对象类型不存在的字段。

例如，您创建了一个计算字段“完成天数”来确定完成项目中的任务所需的时间。

* WEEKDAYDIFF({actualStartDate},{actualCompletionDate})

您希望在迭代中执行相同的操作。您可以使用相同的表达式；但是，可用于任务对象的字段并不总是可用于迭代对象。所以，[!DNL Workfront] 为您提供了使用正确对象字段构建计算的机会。

**专家提示**：创建自定义字段时，将计算表达式从“计算”框复制到“说明”字段。当计算的自定义字段从字段库添加到自定义表单时，该字段不会被删除。

根据需要，自定义表单中的计算字段可以非常简单或非常复杂。表达式可以嵌入或嵌套其他表达式和值，以提供所需的详细程度，以便更好地了解组织中正在进行的工作的进展情况。

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you're ready to start building your own calculated custom fields.-->
