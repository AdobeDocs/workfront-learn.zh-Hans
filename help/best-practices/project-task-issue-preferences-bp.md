---
title: 最佳实践 — 项目、任务和问题首选项
description: 了解Adobe Workfront专家有关设置、管理和使用Workfront项目、任务和问题首选项的最佳实践建议。
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# 最佳实践 — 项目、任务和问题首选项

## 什么是Adobe Workfront“最佳实践”？

最佳做法是代表有效、高效的行动方针的准则；易于您和贵公司用户采用；和可以在您的组织内成功复制。

在您查看这些建议时，请记住，一些Workfront最佳实践是普遍的，而其他一些则可能更具体地介绍该主题。 将这些最佳实践用作框架，以帮助指导Workfront系统的设置和使用。

## 导航此页面

在您浏览此页面时，首先您会找到该主题所有最佳实践的高级列表。 这样，您便可以审核推荐，而无需深入研究“原因”的详细信息。

“为什么这些最佳实践？” 高级列表后找到的区域，详细介绍了一些最佳实践以及它们被视为流程、工具等的原因，您应当考虑使用Workfront实例进行实施。

</br>
</br>

## 项目、任务和问题首选项最佳实践

* 将默认任务持续时间类型设置为“简单”。

* 将新项目状态的首选项设置为“计划”或“构思”，而不是“当前”。

* 在全局项目首选项中启用自动创建基线。

* 在系统项目首选项的“业务案例”部分中选中所有选项。

* 在“问题”首选项中，选中当“解决对象”的状态发生更改时自动更新“可解决的问题”状态的选项。

</br>
</br>


## 为什么是这些最佳实践？

**最佳实践**

将默认任务持续时间类型设置为“简单”。

**原因如下**

持续时间类型定义任务持续时间、计划小时数和分配给任务的人员数量之间的关系。

使用简单作为全局系统默认值，手动创建的所有任务都具有此持续时间类型。 计划小时数在任务分配者之间的持续时间内平均分配。 简单持续时间类型可以简化项目计划，因为它允许您更改任务分配人和计划小时数，而不影响任务的持续时间、计划起始日期或计划完成日期。

</br>
</br>

**最佳实践**

将新项目状态的首选项设置为“计划”或“构思”，而不是“当前”。

**原因如下**

“当前”状态表示项目处于实时状态且正在积极完成工作。 创建项目时，很少需要处于此状态。 即使使用项目模板，在获取任务分配、调整项目的计划完成日期等方面也会涉及一些“计划”。 “计划”状态还禁止向任务分配人和项目团队成员发出通知。 对于涉及的用户而言，在项目开始之前接收通知可能会令他们感到困惑。

</br>
</br>

**最佳实践**

在全局项目首选项中启用自动创建基线。

**原因如下**

每次您将项目状态更改为“当前”时，Workfront都会自动记录项目基线。 项目的此“快照”提供了有关项目计划随时间变化的历史信息。 例如，在向领导层展示转移优先级或范围蠕变如何影响项目的截止时间时，您可以将原始项目计划与当前计划进行比较。

</br>
</br>

**最佳实践**

在系统项目首选项的“业务案例”部分中选中所有选项。

**原因如下**

启用所有五个选项，以允许项目经理、规划人员和其他人员在项目的业务案例中包含这些部分中的任何一个。 如果未启用这些选项，则它们不会显示在业务案例窗口中。 如果该特定项目不需要任何字段，但用户无法在项目级别启用字段，则可以将其中任何字段留空。 这些选项只能在“设置”中全局启用。

</br>
</br>

**最佳实践**

在“问题”首选项中，选中当“解决对象”的状态发生更改时自动更新“可解决的问题”状态的选项。

**原因如下**

将问题转换为项目时，此首选项设置“链接”两个项目的状态。 更新项目状态（解析对象）将自动更新问题状态。 这意味着请求者可以查看在其请求中取得的进展，即使他们无权在Workfront中查看整个项目。