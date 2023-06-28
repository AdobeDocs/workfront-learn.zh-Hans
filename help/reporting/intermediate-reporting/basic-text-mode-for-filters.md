---
title: 了解筛选器的基本文本模式
description: 了解什么是文本模式、什么是驼峰式拼写以及可以在Workfront的报告过滤器中使用的一些基本“即插即用”文本模式。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 了解筛选器的基本文本模式

>[!IMPORTANT]
>
>先决条件：
>
>* 了解报表元素
>* 了解报表组件
>* 创建基本过滤器

>[!TIP]
>
>* 要更深入地了解文本模式，我们建议您观看录制的网络研讨会活动 [咨询专家 — 文本模式报告简介](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en)，时长为一小时。
>* 要进一步了解文本模式，我们建议您查看 [高级报告](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) 教程，总时长为5.5小时。


在本视频中，您将了解：

* 什么是文本模式
* 什么是驼峰式的
* 您可以在报表过滤器中使用的一些基本“即插即用”文本模式

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## 任务 — 筛选出我已标记“已完成我的部分”的任务

以下文本模式将排除用户已标记“已完成我的部件”的任务。 您只需创建一个任务过滤器，添加所需的任何过滤器规则，然后切换到文本模式，并将代码粘贴到您在过滤器中看到的任何文本模式之后。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## 任务 — 显示等待我批准的所有任务

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## 任务 — 显示我已批准的所有任务

创建包含所需过滤器的任务报告，然后转到“过滤器”选项卡，并单击“切换到文本模式”。 将此代码添加到已有的任何代码中：

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## 任务 — 显示至少具有一个跨项目前置任务的所有任务

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## 任务 — 显示我分配给其他人的所有任务

创建包含所需过滤器的任务报告，然后转到“过滤器”选项卡，并单击“切换到文本模式”。 将此代码添加到已有的任何代码中：

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

这将显示登录用户至少分配了一个当前被分配人的所有任务。 如果被分配人是由多个人员分配的，则仅分配人员的第一个人员的姓名将在任务登陆页面上显示为“请求者”。

## 任务 — 显示已完成 — 未决批准的所有任务

```
status=CPL:A
status_Mod=in
```


## 问题 — 显示所有已完成的问题 — 未决批准

```
status=CPL:A
status_Mod=in
```


## 项目 — 显示所有已完成 — 未决批准的项目

```
status=CPL:A
status_Mod=in
```


## 注意 — 显示我已标记的所有评论

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## 参数/自定义字段报告 — 显示未附加到自定义表单的自定义字段（在清理工作中非常有用）

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
