---
title: 最佳实践 - API 资源管理器
description: 探索 Adobe Workfront 专家提供的有关设置、管理和使用 Workfront API 资源管理器的最佳实践建议。
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
TQID: https://experienceleague.adobe.com/RUQeNzEb0eg9DKSKepugb0HD4O2ODql-0mWBn-ptgxk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: bb1dd007-4a34-496d-9d3b-2278fdaadac1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 75%

---

# 最佳实践 - API 资源管理器

## 什么是 Adobe Workfront 的“最佳实践”？

最佳实践是代表有效、高效行动方针的指南；您和您公司的用户很容易采用；并且可以在您的组织中成功复制的实践。

当您审阅这些建议时，请记住，一些 Workfront 最佳实践是通用的，而其他最佳实践可能更特定于相关主题。 使用这些最佳实践作为框架来帮助指导您对 Workfront 系统的设置和使用。

## 浏览此页面

当您滚动浏览此页面时，首先您将找到该主题的所有最佳实践的概括列表。 通过该列表，您可以审阅建议，而无需深入了解有关“原因”的细节。

在高级列表后面的“为什么这些是最佳实践？”区域提供了有关一些最佳实践的更多详细信息，以及为什么将它们视为流程、工具等，您应考虑使用Workfront实例进行实施。

</br>
</br>

## API 资源管理器最佳实践

* 为与第三方系统集成一起使用的自定义字段建立命名约定。

* 使用 Workfront 项目来跟踪在集成中使用的所有自定义字段。

* 将对象 ID 字段添加到系统管理员使用的报告中。

</br>
</br>

## 这些为什么是最佳实践？

**最佳实践**

为与第三方系统集成一起使用的自定义字段建立命名约定。

**原因如下**

确保创建自定义表单的每个人都了解该命名约定，这样他们就不会意外使用为集成保留的字段。 根据您的集成和工作流，以多种方式使用同一字段可能会导致数据被修改或覆盖，从而可能会导致报告中的数据不正确。

</br>
</br>


**最佳实践**

使用 Workfront 项目来跟踪在集成中使用的所有自定义字段。

**原因如下**

项目是记录自定义字段名称、与它们一起使用的集成等的理想位置。这将帮助您避免创建多余的自定义字段，或避免将同一自定义字段与多个集成一起使用。

</br>
</br>


**最佳实践**

将对象 ID 字段添加到系统管理员使用的报告中。

**原因如下**

在使用 API 或其他集成时，系统管理员通常需要通过 ID 号来引用 Workfront 中的对象。 在视图中纳入您处理的对象（项目、任务、问题、模板、自定义表单等）的ID字段 以便于访问和复制。
