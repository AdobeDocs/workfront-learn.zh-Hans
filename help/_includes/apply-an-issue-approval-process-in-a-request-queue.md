---
source-git-commit: b150105844a42e06f5e96f787ad62a1b62185f91
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 18%

---
# 在请求队列中应用问题批准流程 — 已共享

>[!PREREQUISITES]
>
>* [在Workfront中创建请求流](https://experienceleague.adobe.com/zh-hans/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [创建和管理审批流程](https://experienceleague.adobe.com/zh-hans/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


此视频介绍创建请求队列时应用默认审批流程的过程。 创建请求&#x200B;后，其最初的状态为“新建 — 未决批准”，并且会向指定的批准者发送批准通知。 如&#x200B;果获得批准，状态将更改为“新”，允许已分配人员开始工作。 如&#x200B;果被拒绝，由于审批流程设置中的常见错误，状态可能会错误地恢复为“新”。 &#x200B;
视频重点介绍当状态设置为“新建”（新请求的默认设置）时会触发审批流程。 如&#x200B;果被拒绝，系统默认将状态更改回前一个状态，这对于新请求并不理想。 相反&#x200B;，应选择其他状态，如“将不会解析”。 视频&#x200B;还指出，默认情况下不提供“已拒绝”状态，但系统管理员可以根据需要创建状态。 &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455034/?captions=chi_hans&quality=12&learn=on&enablevpops=1)

## 关键要点

* **默认审批流程：**&#x200B;创建请求队列时，您可以应用默认审批流程，自动将审批工作流分配给每个请求。
* **批准时状态更改：**&#x200B;已批准的请求将其状态从“新 — 未决批准”更改为“新”，从而允许已分配的个人开始处理这些请求。
* **拒绝处理中的常见错误：**&#x200B;如果请求被拒绝，由于审批流程中的默认系统设置，状态将恢复为“新”。
* **已拒绝请求的建议状态：**&#x200B;最好选择其他状态（如“将不会解决”），而不是恢复到以前的状态（“新”），以避免混淆。
* **自定义状态选项：**&#x200B;默认情况下不提供“已拒绝”状态，但系统管理员可以根据需要创建一个状态，以便在审批流程中更加清晰明了。


## 有关此主题的推荐教程

* [有效地委派任务、问题和审批](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [了解特定于组的审批流程](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [在Workfront中创建请求流](/help/manage-work/request-queues/create-a-request-flow.md)
* [创建和管理审批流程](https://experienceleague.adobe.com/zh-hans/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)

