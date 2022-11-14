---
title: 了解过滤器的基本文本模式
description: 了解什么是文本模式、驼峰式大小写以及在 [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 818ee105af32589cb0e297e6f419a4a449a60052
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 了解过滤器的基本文本模式

>[!IMPORTANT]
>
>先决条件：
>
>* 了解报表元素
>* 了解报表组件
>* 创建基本过滤器


>[!TIP]
>
>* 为了更深入地了解文本模式，我们建议您观看录制的网络研讨会活动 [咨询专家 — 文本模式报告简介](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en)，长度为一小时。
>* 要进一步了解文本模式，我们建议您在 [高级报表](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) 教程，总共需要五个半小时。



在此视频中，您将学习：

* 什么是文本模式
* 骆驼的病是什么
* 您可以在报表过滤器中使用一些基本的“即插即用”文本模式

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)


## 任务 — 筛选我标记为“完成部分”的任务

以下文本模式将排除用户标记为“完成我的部件”的任务。 您只需创建一个任务过滤器，添加所需的任何过滤器规则，然后切换到文本模式，并在过滤器中看到的任何文本模式之后粘贴下面的代码。

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

创建包含您想要的任何过滤器的任务报告，然后转到过滤器选项卡并单击切换到文本模式。 将此代码添加到任何已存在的代码中：

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

创建包含您想要的任何过滤器的任务报告，然后转到过滤器选项卡并单击切换到文本模式。 将此代码添加到任何已存在的代码中：

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

这将显示登录用户分配了至少一个当前受分配者的所有任务。 如果受分配人由多个人分配，则任务登录页面上只有分配了某人的第一个人的姓名将显示为“请求者”。

## 任务 — 显示所有已完成的任务 — 待批准

```
status=CPL:A
status_Mod=in
```


## 问题 — 显示所有已完成的问题 — 待批准

```
status=CPL:A
status_Mod=in
```


## 项目 — 显示所有已完成的项目 — 待批准

```
status=CPL:A
status_Mod=in
```


## 注意 — 显示我标记的所有评论

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## 参数/自定义字段报表 — 显示未附加到自定义表单的自定义字段（在清理工作中非常有用）

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
