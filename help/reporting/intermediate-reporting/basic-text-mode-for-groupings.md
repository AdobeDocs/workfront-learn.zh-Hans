---
title: 了解分组的基本文本模式
description: 了解什么是文本模式、驼峰式大小写，以及在Workfront中的分组中可以使用的一些基本的“即插即用”文本模式。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
source-git-commit: 21fb81fcb4b1468059e571a87e201fa48fb64ff7
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# 了解分组的基本文本模式

>[!IMPORTANT]
>
>先决条件：
>
>* 了解报表元素
>* 了解报表组件
>* 创建基本分组


在此视频中，您将学习：

* 什么是文本模式
* 骆驼的病是什么
* 您可以在分组中使用一些基本的“即插即用”文本模式

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12)

## 任务 — 4个父代分组

以下文本模式将根据多达四个级别的父代对任务进行分组，并将不存在的父代留空。

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![显示按4个父项分组的项目任务的屏幕图像](assets/4-parents-grouping.png)


## 任务 — 完成百分比分组

以下文本模式将根据任务完成百分比对任务进行分组。 分组后，任务将分为以下类别之一：

* 0%
* 1%至25%
* 26%至50%
* 51%至75%
* 76%至99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![显示按完成百分比分组的项目任务的屏幕图像](assets/percent-complete-grouping.png)

## 任务 — statusEqualsWith，然后是status

以下文本模式将按statusEqualsWith，然后按status对任务进行分组。

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![显示按statusEqualsWith分组的项目任务的屏幕图像](assets/status-equates-with.png)


## 校样批准 — 按项目名称分组

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![显示按项目名称分组的校样批准的屏幕图像](assets/proof-approvals-grouped-by-project-name.png)

