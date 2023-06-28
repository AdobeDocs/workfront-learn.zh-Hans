---
title: 了解性能指标
description: 了解如何使用性能量度 —  [!UICONTROL Performance Index Method] ([!UICONTROL PIM])和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# 了解性能指标

项目经理使用的两个绩效指标包括 [!UICONTROL Performance Index Method] ([!UICONTROL PIM])和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。 系统范围的默认值可以在以下位置设置 [!DNL Workfront] 并应用于新创建的项目。 [!UICONTROL PIM] 之后，可以在单个项目上修改。

**[!UICONTROL PIM]**

的设置 [!UICONTROL PIM] 控制方式 [!DNL Workfront] 计算其他项目绩效指标，例如 [!UICONTROL Cost Performance Index] ([!UICONTROL CPI])， [!UICONTROL Cost Schedule Performance Index] ([!UICONTROL CSI])， [!UICONTROL Schedule Performance Index] ([!UICONTROL SPI])，以及 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。

的选项 [!UICONTROL PIM] 基于小时和基于成本。

* **基于小时** — Workfront在计算项目的CPI和EAC时使用计划小时数。 项目的EAC显示为以小时为单位的数字。
* **基于成本** — Workfront在计算项目CPI和EAC时使用计划劳力成本。 EAC显示为货币值。 使用此选项时，请确保任务被分配人（用户和/或工作角色）与成本费率相关联。

**[!UICONTROL EAC]**

[!UICONTROL EAC] 表示任务或项目完成时的预计总成本。 选项在项目级别进行计算，并从任务/子任务汇总。

* **在项目级别计算** — [!UICONTROL EAC] 对于父任务和项目，使用中的实际小时数/实际人工成本确定 [!UICONTROL EAC] 公式。 该计算包括直接添加到父任务或项目的实际小时数/成本和费用。
* R **从任务/子任务向上滚动** — [!UICONTROL EAC] 父任务和项目的URL值由将 [!UICONTROL EAC] 每个子任务。 此计算不包括直接添加到父任务或项目的实际小时数/成本。

此 [!UICONTROL EAC] 计算列于 [计算完工估算(EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**性能量度：设置**

要设置 [!UICONTROL PIM] 和 [!UICONTROL EAC] 系统默认值：

1. 选择 **[!UICONTROL Setup]** 从主菜单。
1. 单击 **[!UICONTROL Project Preferences]** 在左侧面板菜单中，然后单击 **[!UICONTROL Projects]**
1. 在 [!UICONTROL Project Status] 部分，查找 [!UICONTROL Performance Index Method]. 选择基于小时数或基于成本。
1. 对象 [!UICONTROL Estimate at Completion]，选择在项目层计算或从任务/子任务汇总。
1. 单击 **[!UICONTROL Save]** 在窗口底部。

![的图像 [!UICONTROL Project Preferences] screen](assets/setting-up-finances-1.png)

**设置 [!UICONTROL PIM] 在单个项目中**

1. 转到项目的登陆页面。
1. 单击 **[!UICONTROL Project Details]** 从左侧面板中。
1. 打开 **[!UICONTROL Finance]** 部分。
1. 双击下面的文本 **[!UICONTROL Performance Index Method]** 以编辑它。
1. 选择基于小时数或基于成本。
1. 单击 **[!UICONTROL Save]** 更改以完成。

![的图像 [!UICONTROL Project Details] screen](assets/setting-up-finances-2.png)

[!UICONTROL PIM] 可以在项目模板中设置 [!UICONTROL Finance] 部分模板详细信息。
