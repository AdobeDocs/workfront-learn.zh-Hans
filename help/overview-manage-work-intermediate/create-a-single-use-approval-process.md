---
title: 创建全局和一次性审批流程
description: 了解如何为项目、任务或问题创建全局和单次使用的审批流程。
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
hide: true
doc-type: video
exl-id: e80dd36f-7aab-4cf1-873c-92dba684c13c
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 100%

---

# 创建全局和一次性审批流程

项目、任务和问题的审批流程有助于项目经理能够在继续推动工作之前获得专业人员的确认，确定工作已经按照恰当的方式完成。项目经理可以为每种情况创建一个审批流程（这称为一次性审批流程），或者从先前为满足常见需求而创建的可能具有多个审批流程的列表中进行选择（这些称为全局或现有审批流程）。

在任一情况下，当对象状态更改为审批流程中指定的状态时，审批人都会收到各种方式的通知，以便审查该项工作并审批或拒绝它。鉴于整个项目在等待审批时可能会暂停，审批人应提前意识到他们可能会被要求进行审批。如果审批人因任何原因不在办公室，他们可以将审批工作委托给符合资格的替代者。请参阅[委派任务、问题和审批](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)，以了解详情。

在本视频中，您将会了解到如何针对项目、任务或问题创建全局审批流程和一次性审批流程。

>[!VIDEO](https://video.tv.adobe.com/v/3434697/?quality=12&learn=on&enablevpops&captions=chi_hans)

>[!TIP]
>
>您可以将项目或任务的一次性审批流程添加到项目模板中。

>[!NOTE]
>
>您可以按照视频中对任务所述的相同方式，对项目和问题设置一次性审批。

## 如何在请求队列中应用自动审批问题功能

如果要在请求队列中设置自动审批问题功能，则只能使用全局问题审批流程并在 [!UICONTROL Queue topic] 中应用该流程。

创建或编辑 [!UICONTROL Queue topic] 时，在 **[!UICONTROL Default Approval]** 字段中选择全局审批流程。

![该图显示了如何在队列主题中选择默认审批流程](assets/automatic-issue-approval-1.png)

您可能需要编辑问题审批流程，从而确保 **[!UICONTROL Previous status]** 不是审批被拒绝时设置的问题。这是因为之前的状态是 **[!UICONTROL New]**，并且这也是触发审批流程的状态，所以它是审批通过后将会被设置为的状态。为了避免问题审批被拒绝时产生混淆，最好将该状态设置为 **[!UICONTROL Won't Resolve]** 之类的状态，或者为此目的创建的自定义状态。

![该图显示了在问题被拒绝时更改使用状态](assets/automatic-issue-approval-2.png)


## 有关此主题的推荐教程

* [委派任务、问题和审批](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [了解特定于群组的审批流程](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [创建请求流](/help/manage-work/request-queues/create-a-request-flow.md)

