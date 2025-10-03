---
title: 了解现有的过滤器
description: 了解什么是 EXISTS 过滤器、它能为您带来哪些作用，以及如何从零开始构建一个。此外，还可以查看多个有用的 EXISTS 过滤器示例。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 4%

---

# 了解现有的过滤器

EXISTS过滤器是高级的文本模式过滤器，这使我们能够绕过标准Report Builder中2个表/字段跳转限制。 或者，它们可用于通过NOTEXISTS识别系统中缺少特定关系条件的对象。

在本视频中，您将了解如何创建存在过滤器以在验证审批报告中查看“当前项目的验证审批”。

有关EXISTS函数的更深入演练，请参阅[使用EXISTS语句创建复杂的文本模式筛选器](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements)文档。

>[!VIDEO](https://video.tv.adobe.com/v/3471213/?quality=12&learn=on&enablevpops=1&captions=chi_hans)

## EXISTS过滤器示例

### 项目报告存在

这会将任务用作链接对象，方法是比较在任务级别找到的projectID并将其与项目级别ID字段匹配。 这样，我们就可以将任务中的任务用户与$$USER.ID通配符进行比较。 这会导致仅返回其查看用户被分配到的项目
任务，无论他们是否是主要被分配人。

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


此标头使用问题(optask)作为链接对象，同时也比较在问题(optask)级别找到的项目ID并将其与项目级别ID字段匹配。 然后，会检查是否存在任何这些问题(optasks)的条目日期在指定的范围内。 在这种情况下，它将返回具有
由于NOTEXISTS，在最近的30天内未记录问题(optask)。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### 存在模板报告

此过滤器将显示所有未用于创建项目的模板，或在上一年中附加到项目的模板。 需要注意的是，为了确定模板是否被用作附件，它依赖于模板中带有任务。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### 任务报告存在

这会使用“用户”表作为链接对象，通过工作总揽taskID和任务ID进行连接。 然后，会将ID的团队集合检查为用户团队ID，如果有任何被分配者与正在查看的用户属于同一团队，则会返回任务。

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### 存在用户报告

这将返回过去3周内未发布更新的所有用户。 这会使用note对象来弥合差距，并将ownerID与用户ID进行比较。 然后，如果用户拥有的便笺的输入日期不大于3周前，则返回该用户。

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

这将返回上周未记录小时数的所有用户。 此标头使用与上述示例非常类似的方法，实际使用的却是小时所有者信息和小时输入日期来构建其返回的用户基础。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

在用户报表中，显示与项目的“人员”选项卡匹配的用户列表。

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### 类别（自定义表单）报表存在

此文本将为您提供一个列表，其中包含所有从未在项目中使用的项目表单。 这应当与指定我们关注的表单的对象类型结合使用。 所以本例的焦点是PROJ，所以我们应该将注解包含在objTypes行中。 可以使用此项
对于其他对象类型，可通过更改对象代码相关部分来实现。 这将检查附加表单的项目集合，如与所列的表单不匹配，则将返回。

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### 存在参数（自定义字段）报表

这会返回当前未附加到系统中自定义表单的任何自定义字段。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### 报告存在

这将返回任何在其过滤器中使用特定值的报表。

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

这将返回附加到任何仪表板的任何报告。

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### 存在校对审批报告

这将只返回对处于当前状态的项目的验证审批。 这使用Document对象通过选中currentVersionID到documentVersionID来弥合从验证审批到项目的差距，从那里我们跳转到项目状态。

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
