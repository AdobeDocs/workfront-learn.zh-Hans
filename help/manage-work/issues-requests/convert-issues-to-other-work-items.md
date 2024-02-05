---
title: 将问题/请求转化为任务
description: 了解如何将问题转化为其他工作项目。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: 060ceb14d274e8b2ad080c1f58290a2c5769e007
workflow-type: ht
source-wordcount: '460'
ht-degree: 100%

---

# 将问题/请求转化为任务

某个问题可能非常重要，需要在项目时间表中计入解决该问题的时间和精力并分配适当的资源。在这种情况下，可以将问题转化为任务。

![图像：[!UICONTROL Workfront] 中某个问题的 [!UICONTROL Convert to Task] 选项。](assets/15-convert-issue-to-task-menu-option.png)

1. 导航到记录该问题的项目或任务的 [!UICONTROL Issues] 部分。或者在您有权访问的报告中找到该问题。
1. 单击问题名称将其打开。
1. 从问题名称右侧的三点菜单中，选择 **[!UICONTROL Convert to task]**。
1. 填写 [!UICONTROL Convert to task] 表单。首先为新任务指定名称和描述。
1. 如果新任务属于不同项目，请更改 [!UICONTROL Destination Project] 名称。
1. 在 [!UICONTROL Options] 部分，选中相关的复选框以保留原始问题、允许访问新任务并维护完成日期。进行这些选择时请遵循您组织的工作流。
1. 如果您想要将自定义表单数据从问题传输到任务，请附加自定义表单。（问题表单和任务表单中存在的所有字段都会自动转移到任务表单。）
1. 单击 **[!UICONTROL Convert to task]** 以完成。

![图像：[!UICONTROL Workfront] 中某个问题的 [!UICONTROL Convert to Task] 表单。](assets/16-convert-to-task-options.png)

根据您所在组织的 [!DNL Workfront] 系统设置，在转换任务时，您可能无法更改“选项”部分中的设置。这些选项会影响原始问题和新任务。

* **保留原始问题并将其解决方案与此任务联系起来**&#x200B;保留原始的问题和相关信息（小时数、文件等）。选择此选项后，当任务完成时，该问题会被标记为已解决。如果&#x200B;**未**&#x200B;选择该选项，则原始问题会在任务创建时删除。这可能会影响您的组织跟踪和报告问题的方式。
* **允许（用户名）访问此任务**&#x200B;选项将会允许创建问题的人员访问此新任务。
* **保留问题的规划完成日期**&#x200B;选项允许您保留问题上已设置的规划完成日期。这会将任务限制设置为 [!UICONTROL Finish No Later Than]。如果未选中该框，则会设置任务日期，就像在项目中创建新任务一样。

新任务将会被放置在项目任务列表的底部。将任务移动到所需位置、为工作分配用户或团队、添加规划小时数和持续时间等。

>[!NOTE]
>
>您不能将问题添加到项目时间表中，因为它们代表“规划外的工作”。项目时间线用于“规划的工作”，即任务。


