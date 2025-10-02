---
title: 了解报告组件
description: Workfront的报表组件通过基于对象的筛选器、动态视图、结构化分组和通配符功能来优化数据可视化，以提供量身定制的见解。
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
last-substantial-update: 2025-04-28T00:00:00Z
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 44%

---

# 了解报告组件

此视频介绍Workfront中报表组件的概念，这些组件对于创建筛选器、视图和分组至关重要。 关键组件包括：

* **对象类型：**&#x200B;指定正在处理的Workfront对象，如项目、任务或小时条目。&#x200B;AEM 筛选器、视图和分组特定于对象类型。&#x200B;AEM
* **字段Source和字段名称：**&#x200B;字段源是Workfront中附加了信息的项，字段名称是特定信息（例如，项目的“描述”）。&#x200B;AEM
* **值字段：**&#x200B;表示优先级的字段内容，如“低”、“正常”、“高”或“紧急”。&#x200B;AEM
* **筛选器限定符：**&#x200B;定义要在报告中包含或排除的值，例如显示优先级为“高”的任务&#x200B;。


>[!VIDEO](https://video.tv.adobe.com/v/3447031/?quality=12&learn=on&captions=chi_hans)

## 要点

* **报表组件：** Workfront的报表组件包括对象类型、字段源、字段名称、筛选器限定符和值字段，这些对于创建筛选器、视图和分组至关重要。&#x200B;AEM
* **对象类型特殊性：**&#x200B;筛选器、视图和分组绑定到特定的对象类型，如项目、任务或小时条目，确保报告根据相关数据定制。&#x200B;AEM
* **筛选器规则：**&#x200B;筛选器使用字段源、字段名称、限定符和值来定义条件。&#x200B;AEM 例如，“我的项目”过滤器仅显示登录用户属于项目团队的当前项目。&#x200B;AEM
* **视图和分组：**&#x200B;视图以列形式显示字段源和字段名称组合（如“所有者名称”），而分组根据特定条件（如“公司名称”）组织数据&#x200B;。
* **通配符用法：**&#x200B;筛选器中的通配符允许动态匹配，例如，识别项目团队中的登录用户，增强报告中的个性化。&#x200B;AEM

## 报告组件快速参考

![创建过滤器的屏幕图像](assets/reporting-components-1.png)

**A - 字段源**

字段源选项取决于所选的对象类型。通常情况下，字段源是 Workfront 中特定信息（也称为字段名称）所属的项目。有时，字段源与对象类型相同。
字段源决定了哪些字段名称可用。

示例：[!UICONTROL Project]、[!UICONTROL Task]、[!UICONTROL Issue]、[!UICONTROL Assigned To]

**B - 字段名称**

字段名称是关于您选择的字段源的可用信息。

它们可以是您填写的 Workfront 字段、自定义表单中的字段或 Workfront 自动捕获的信息。

字段名称会驱动值字段选项。

示例：[!UICONTROL Progress Status]、[!UICONTROL Description]、[!UICONTROL Planned Completion Date]、自定义表单字段

**C - 过滤器限定符**

过滤器限定符有助于缩小在所选字段源和字段名称下可查看的潜在结果的范围。

它们指定字段源和字段名称与值字段的关系。

示例：等于、包含、空、小于

**D - 值**

该值是在字段名称指定的字段中输入的信息。

值的选项由字段源和字段名称决定。

值中可以使用用户和日期的通配符，也可以使用自由形式的文本。

示例：新的、当前的、$$TODAYbw、描述

>[!TIP]
>
>如需帮助理解 Workfront 中的特定字段名称，请参阅 [Adobe Workfront 术语表](https://experienceleague.adobe.com/docs/workfront/using/basics/workfront-terminology-glossary.html?lang=zh-Hans)。

