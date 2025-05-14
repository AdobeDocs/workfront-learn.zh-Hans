---
title: 了解过滤器的基本文本模式
description: 了解什么是文本模式、什么是驼峰式拼写以及可在 Workfront 的报告过滤器中使用的一些基本的“即插即用”文本模式。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2024-10-04T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: f03518b568cc24ad39b32f6dbfd763400529cf0f
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 100%

---

# 了解过滤器的基本文本模式

>[!PREREQUISITES]
>
>* [了解报告要素](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=zh-hans)
>* [了解报告组件](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=zh-hans)
>* [创建基本过滤器](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=zh-hans)


>[!TIP]
>
>* 为了更深入地了解文本模式，我们建议观看录制的网络研讨会活动[咨询专家 - 文本模式报告简介](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=zh-hans)，时长为一小时。
>* 要了解有关文本模式的更多信息，我们建议观看[高级报告](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=zh-hans)教程，总共为五个半小时。
>* 单击此处以访问 [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)


在本视频中，您将了解到：

* 什么是文本模式
* 什么是驼峰式拼写
* 您可以在报告过滤器中使用一些基本的“即插即用”文本模式

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)

## “了解过滤器的基本文本模式”活动


### 任务 - 过滤掉我标记为“已完成我负责的部分”的任务

以下文本模式将会排除用户标记为“已完成我负责的部分”的任务。您所要做的就是创建一个任务过滤器，添加所需的任何过滤规则，然后切换到文本模式，并将下面的代码粘贴到您在过滤器中看到的任何文本模式之后。


>[!WARNING]
>
> 这不适用于日程表过滤器。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### 任务 - 显示所有等待我审批的任务

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### 任务 - 显示我已审批的所有任务

使用所需的任何过滤器创建任务报告，然后转到“过滤器”选项卡并单击“切换到文本模式”。将此代码添加到现有代码中：

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### 任务 - 显示至少有一个跨项目前置任务的所有任务

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### 任务 - 显示我分配给其他人的所有任务

使用所需的任何过滤器创建任务报告，然后转到“过滤器”选项卡并单击“切换到文本模式”。将此代码添加到现有代码中：

>[!WARNING]
> 
> 这不适用于日程表过滤器。

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

这将显示登录用户指派了至少一个当前受指派者的所有任务。如果受指派者是由多人指派的，则只有第一个指派者的姓名才会在任务登陆页面上显示为“请求者”。

### 任务 - 显示所有“已完成 - 待审批”的任务

```
status=CPL:A
status_Mod=in
```


### 问题 - 显示所有“已完成 - 待审批”的问题

```
status=CPL:A
status_Mod=in
```


### 项目 - 显示所有“已完成 - 待审批”的项目

```
status=CPL:A
status_Mod=in
```


### 注释 - 显示我被标记的所有评论

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### 参数/自定义字段报告 - 显示未附加到自定义表单的自定义字段（在清理工作中非常有用）

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
