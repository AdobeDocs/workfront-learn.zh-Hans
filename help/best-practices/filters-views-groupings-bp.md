---
title: 最佳实践 - 过滤器、视图和分组
description: 探索 Adobe Workfront 专家提供的有关设置、管理和使用 Workfront 过滤器、视图和分组的最佳实践建议。
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 100%

---

# 最佳实践 - 过滤器、视图和分组

## 什么是 Adobe Workfront 的“最佳实践”？

最佳实践是代表有效、高效行动方针的指南；您和您公司的用户很容易采用；并且可以在您的组织中成功复制的实践。

当您查看这些建议时，请记住，一些 Workfront 最佳实践是通用的，而其他最佳实践可能更特定于相关主题。使用这些最佳实践作为框架来帮助指导您对 Workfront 系统的设置和使用。

## 浏览此页面

当您滚动浏览此页面时，首先您将找到该主题的所有最佳实践的概括列表。通过该列表，您可以查看建议，而无需深入了解有关“原因”的细节。

“这些为什么是最佳实践？”概括列表后面的区域提供了一些最佳实践的更多详细信息以及为什么将它们视为应考虑使用 Workfront 实例实施的流程、工具等。

</br>
</br>

## 过滤器、视图和分组最佳实践

* 通过利用对象列表上的过滤器、视图和分组来获取所需的数据，减少您创建的自定义报告的数量。

* 使用布局模板中的列表控件隐藏常用对象（项目、任务、计划等）不需要的过滤器、视图和分组。

* 通过布局模板上的列表控件共享与组织的工作流和流程相关的自定义过滤器、视图和分组。

* 在为项目状态、任务状态或问题状态创建过滤器时，请使用“（对象）>>状态等于”字段源/字段名称以及等于修饰符，而不是“项目>>状态”字段源/字段名称。

</br>
</br>

## 这些为什么是最佳实践？

**最佳实践**

通过利用对象列表上的过滤器、视图和分组来获取所需的数据，减少您创建的自定义报告的数量。

**原因如下**

为您想要查看的每个数据段创建一次性使用的报告非常耗时，并且会使 Workfront 系统变得拥挤不堪。

有关如何创建带提示的报告的说明，请参阅[了解报告设置](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html?lang=zh-Hans)视频中标有“如何设置和使用报告提示”的章节。

有关如何创建带有自定义提示的报告的说明，请参阅[创建自定义提示](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html?lang=zh-Hans)。

</br>
</br>

**最佳实践**

使用布局模板中的列表控件隐藏常用对象（项目、任务、计划等）不需要的过滤器、视图和分组。

**原因如下**

少即是多。隐藏与用户日常工作流无关的过滤器、视图和分组列表选项可以缩小列表范围，从而使用户更容易更快地找到他们需要的内容。

有关如何使用布局模板隐藏过滤器、视图或分组的说明，请参阅[使用布局模板自定义报告列表](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=zh-Hans)。

</br>
</br>

**最佳实践**

通过布局模板上的列表控件共享与组织的工作流和流程相关的自定义过滤器、视图和分组。

**原因如下**

如果您创建了显示特定于用户日常流程的信息的过滤器、视图和分组，则可以轻松地通过布局模板共享这些信息。这可确保分配该布局模板的每个人都具有与其工作流相关的过滤器、视图和分组选项。

通过布局模板自定义您希望用户可以看见的信息也可以节省系统和管理员的时间，因为他们不必单独共享每个过滤器、视图或分组选项。

有关如何使用布局模板分享过滤器、视图或分组的说明，请参阅[使用布局模板自定义报告列表](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=zh-Hans)。

</br>
</br>

**最佳实践**

在为项目状态、任务状态或问题状态创建过滤器时，请使用“（对象）>>状态等于”字段源/字段名称以及等于修饰符，而不是“项目>>状态”字段源/字段名称。

**原因如下**

通过使用“（对象）>>等于”，您会将所有在状态设置的“等于”字段中指定了特定状态的自定义状态包括在内。而将过滤器设置为“（对象）>>状态>等于”则要求您为过滤器选择特定的状态。如果您需要考虑各种过滤器中的这些新状态，这可能会为维护工作带来挑战。每个过滤器都需要打开并更新为新状态。

例如，如果您想查看所有当前项目，您可以将过滤器设置为读取“项目”>>“状态”>“等于”>“当前”。但是，如果有人添加了名为“活动”的自定义状态并将其等同于“当前”，则该过滤器将找不到状态为“活动”的项目。但是，如果您使用“项目”>>“状态等于”>“等于”>“当前”，则过滤器会查找状态为“当前”或“活动”的对象，因为它们的“等于”字段中都具有“当前”。
