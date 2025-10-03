---
title: 在请求队列中应用问题批准流程
description: 实施默认审批流程以简化请求工作流，确保已批准的请求将其状态适当地更改为“新”。 通过选择状态更改为“将不会解决”来解决被拒绝请求的混淆。
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 11%

---

# 在请求队列中应用问题批准流程

>[!PREREQUISITES]
>
>* [创建请求流](https://experienceleague.adobe.com/zh-hans/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [创建全局和一次性审批流程](https://experienceleague.adobe.com/zh-hans/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


此视频介绍创建请求队列时应用默认审批流程的过程。&#x200B;AEM 创建请求后，其最初的状态为“新建 — 未决批准”，并且会向指定的批准者发送批准通知。&#x200B;AEM 如果获得批准，状态将更改为“新建”，允许已分配人员开始工作。&#x200B;AEM 如果被拒绝，由于审批流程设置中的常见错误，状态可能会错误地恢复为“新”。&#x200B;AEM
视频重点介绍当状态设置为“新建”（新请求的默认设置）时会触发审批流程。&#x200B;AEM 如果被拒绝，系统默认将状态更改回前一个状态，这对于新请求并不理想。&#x200B;AEM 相反，应选择其他状态，如“将不会解析”。&#x200B;AEM 该视频还指出，默认情况下不提供“已拒绝”状态，但系统管理员可以根据需要创建一个状态。&#x200B;AEM

>[!VIDEO](https://video.tv.adobe.com/v/3455034/?quality=12&learn=on&enablevpops=1&captions=chi_hans)

## 要点

* **默认审批流程：**&#x200B;创建请求队列时，您可以应用默认审批流程，自动将审批工作流分配给每个请求。
* **批准时状态更改：**&#x200B;已批准的请求将其状态从“新 — 未决批准”更改为“新”，从而允许已分配的个人开始处理这些请求。
* **拒绝处理中的常见错误：**&#x200B;如果请求被拒绝，由于审批流程中的默认系统设置，状态将恢复为“新”。
* **已拒绝请求的建议状态：**&#x200B;最好选择其他状态（如“将不会解决”），而不是恢复到以前的状态（“新”），以避免混淆。
* **自定义状态选项：**&#x200B;默认情况下不提供“已拒绝”状态，但系统管理员可以根据需要创建一个状态，以便在审批流程中更加清晰明了。


## 有关此主题的推荐教程

* [委派任务、问题和审批](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [了解特定于群组的审批流程](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [创建请求流](/help/manage-work/request-queues/create-a-request-flow.md)
* [创建全局和一次性审批流程](https://experienceleague.adobe.com/zh-hans/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
