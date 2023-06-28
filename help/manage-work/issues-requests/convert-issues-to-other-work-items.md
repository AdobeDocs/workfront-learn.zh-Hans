---
title: 将问题转换为其他工作项
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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 0%

---

# 将问题转换为其他工作项

## 将问题转换为任务

一个问题可能非常重大，需要把解决该问题的时间和精力计入项目时间表，并分配适当的资源。 在这种情况下，问题可以转换为任务。

![的图像 [!UICONTROL Convert to Task] 中的问题选项 [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. 导航到 [!UICONTROL Issues] 问题登录的项目或任务的部分。 或者在您有权访问的报告中查找问题。
1. 单击问题名称以将其打开。
1. 从问题名称右侧的3点菜单中，选择 **[!UICONTROL Convert to task]**.
1. 填写 [!UICONTROL Convert to task] 表单。 首先，为新任务指定名称和描述。
1. 如果新任务应属于其他项目，请输入项目名称。
1. 在 [!UICONTROL Options] 部分，选中方框以保留原始问题、允许访问新任务并保持完成日期。 进行这些选择时，请遵循组织的工作流。 如果要将自定义表单数据从问题传输到任务，请附加自定义表单。 （问题表单和任务表单中存在的所有字段将自动转移到任务表单。）
1. 填写自定义表单（如果已附加）。
1. 单击 **[!UICONTROL Convert to task]** 完成。

![的图像 [!UICONTROL Convert to Task] 中的问题形式 [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

取决于您组织的 [!DNL Workfront] 系统设置，则在转换任务时，您可能无法更改“选项”部分中的设置。 这些选项同时影响原始问题和新任务。

* **“保留原来的问题，并将其解决方案与此任务绑定”** 保留原始问题和相关信息（小时、文档等）。 选中此选项后，任务完成后，问题将被标记为已解决。 如果未选择此选项，则将在任务完成时删除原始问题。 这可能会影响贵组织跟踪和报告问题的方式。
* 此 **“允许（用户名）访问此任务”** 选项将允许创建问题的人员访问此新任务。
* 此 **“保留问题的计划完成日期”** 选项允许您保留已在问题中设置的规划完成日期。 这会将任务限制设置为 [!UICONTROL Finish No Later Than]. 如果未选中该框，则将设置任务的日期，就像在项目中创建新任务一样。

新任务被放置在项目任务列表的底部。 将任务移动到所需位置，将用户或团队分配给工作，添加计划小时数和持续时间等。

>[!NOTE]
>
>您无法将问题添加到项目时间线，因为它们代表“计划外工作”。 项目时间线是指“计划工作”，即任务。

## 将问题转化为项目

有时候，解决问题本身或将问题转化为任务并不能解决问题，因为解决问题的过程需要更加复杂的协调。 在这种情况下，您可以将问题转化为项目。

1. 导航到问题登录的项目或任务的问题部分。 或者在您有权访问的报告中查找问题。
1. 单击问题名称以将其打开。
1. 单击问题名称右侧的3点菜单，以显示“更多”菜单。
1. 然后，选择是要创建一个完全空白的新项目还是使用项目模板，该项目模板将预填任务和时间线信息。
1. 在转换为项目窗口中填写信息，从项目的名称开始。
1. 根据您的团队或组织的要求，填写其他项目详细信息。
1. 在选项部分，选中方框以保留原始问题并允许访问新项目。 进行这些选择时，请遵循组织的工作流。
1. 填写自定义表单（如果已附加）。 如果要将自定义表单数据从问题传输到项目，请附加自定义表单。 （问题表单和项目表单中存在的所有字段将自动转移到项目表单。）
1. 单击 **转换为项目** 完成。

“转换为项目”窗口中显示的项目详细信息字段取决于您用于创建项目的方法。 如果您使用从模板转换为项目选项，您将在左侧菜单中看到更多信息。

>[!NOTE]
>
>某些部分（例如选项部分）尽管可见，但根据您组织的Workfront系统设置，可能无法访问。

![显示转换选项的项目屏幕图像](assets/conversion-options.png)

* 单击“”**保留原来的问题，并将其解决方案与此项目绑定**”选项。 此选项保留原始问题和相关信息（小时、文档等）。 当新项目完成时，问题将标记为已解决。 如果未选择此选项，则原始问题将在项目完成时删除。 这可能会影响贵组织跟踪和报告问题的方式。
* “**允许（用户名）访问此项目**“ ”选项允许创建问题的人员访问正在创建的项目。

## 在转换过程中维护信息

<!-- Need link to wf one doc article below 

To learn about what information transfers when you convert an issue to a task or project, we recommend you read through the conversion considerations in the article, Convert issues. This lists what information is kept when converting issues and what isn’t. Workfront recommends you become familiar with these considerations so you don’t lose important information when converting issues to tasks or projects.

-->

传输自定义表单数据需要：

* 同一自定义表单的多个副本 — 一个用于问题，一个用于任务或项目。 这些自定义表单上的字段应该是完全匹配的，因此信息可以从一个自定义表单转移到另一个自定义表单。

* 或选择问题、任务和/或项目对象的单个自定义表单。 使用此方法，您只需在单个自定义表单中创建和维护自定义字段即可。 这是最近的一项增强功能，比拥有同一表单的多个副本要容易得多，但两种方法都可以使用。



<!-- Need link to wf one doc article below

Learn more in the article, Transfer custom form data to a larger work item.

-->

<!-- Pro tips graphic -->

如果在项目模板中包含自定义表单，则在转换过程中选择该模板时，将自动为其分配该表单。

<!-- Learn more graphic and documentation article links 

* Convert issues
* Transfer custom form data to a larger work item
* Overview of resolving and resolvable objects
* Understanding resolving and resolvable objects
* Unlink issues from their resolvable objects

-->

## 从任何问题列表将问题转换为任务或项目

为了提高工作效率，并使问题在快节奏环境中更易于转化，您可以从项目、报告或仪表板中的任何问题列表将问题转化为任务或项目。 只需选择一个问题，然后单击出现的3点菜单。

![显示问题转换选项的项目屏幕图像](assets/convert-from-a-list.png)

