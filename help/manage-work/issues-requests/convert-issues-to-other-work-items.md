---
title: 将问题/请求转换为任务
description: 了解如何将问题转化为其他工作项。
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
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# 将问题/请求转换为任务

一个问题可能非常重大，因此解决该问题的时间和努力需要在项目时间表中加以考虑并分配适当的资源。 在这种情况下，问题可以转换为任务。

![的图像 [!UICONTROL Convert to Task] 中的问题选项 [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. 导航至 [!UICONTROL Issues] 问题登录的项目或任务的部分。 或者在您有权访问的报告中查找问题。
1. 单击问题名称以将其打开。
1. 从问题名称右侧的3点菜单中，选择 **[!UICONTROL Convert to task]**.
1. 填写 [!UICONTROL Convert to task] 表单。 首先，为新任务指定名称和描述。
1. 如果新任务应属于其他项目，请更改 [!UICONTROL Destination Project] 名称。
1. 在 [!UICONTROL Options] 部分，选中方框以保留原来的问题，允许对新任务的访问，并保持完成日期。 进行这些选择时，请遵循组织的工作流。
1. 如果要将自定义表单数据从问题传输到任务，请附加自定义表单。 （问题表单和任务表单中存在的所有字段将自动转移到任务表单。）
1. 单击 **[!UICONTROL Convert to task]** 完成。

![的图像 [!UICONTROL Convert to Task] 问题的形式 [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

根据您组织的 [!DNL Workfront] 系统设置，转换任务时，您可能无法更改“选项”部分中的设置。 这些选项会影响原始问题和新任务。

* **保留原来的问题，并将其解决方案与此任务绑定** 保留原始问题和相关信息（小时、文档等）。 选中此选项后，任务完成后，问题将标记为已解决。 如果此选项为 **非** 选择，则创建任务时将删除原始问题。 这可能会影响贵组织跟踪和报告问题的方式。
* 此 **允许（用户名）访问此任务** 选项将允许创建问题的人员访问此新任务。
* 此 **保持问题的计划完成日期** 利用选项，可保留在问题中设置的规划完成日期。 这会将任务限制设置为 [!UICONTROL Finish No Later Than]. 如果未勾选该框，则将设置任务的日期，就像在项目内创建新任务一样。

新任务将置于项目任务列表的底部。 将任务移动到所需位置，将用户或团队分配给工作，添加计划的小时数和持续时间等。

>[!NOTE]
>
>您无法将问题添加到项目时间线，因为它们代表“计划外工作”。 项目时间线是指“计划工作”，即任务。


