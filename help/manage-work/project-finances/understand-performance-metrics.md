---
title: 了解绩效指标
description: 了解如何使用绩效指标 - [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) 和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。
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
source-wordcount: '350'
ht-degree: 100%

---

# 了解绩效指标

项目经理使用的两个绩效指标包括 [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) 和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。系统范围的默认值可以在 [!DNL Workfront] 中设置，并会应用于新创建的项目。然后，可以在各个项目上对 [!UICONTROL PIM] 进行修改。

**[!UICONTROL PIM]**

[!UICONTROL PIM] 的设置会控制 [!DNL Workfront] 如何计算其他项目绩效指标，如 [!UICONTROL Cost Performance Index] ([!UICONTROL CPI])、[!UICONTROL Cost Schedule Performance Index] ([!UICONTROL CSI])、[!UICONTROL Schedule Performance Index] ([!UICONTROL SPI]) 和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。

[!UICONTROL PIM] 的选项基于小时和成本。

* **基于小时**—Workfront 使用规划小时数来计算项目的 CPI 和 EAC。项目的 EAC 显示为数字（以小时为单位）。
* **基于成本**—Workfront 使用规划劳动力成本来计算项目的 CPI 和 EAC。EAC 显示为货币值。使用此选项时，请确保任务受让人（用户和/或工作角色）与成本费率相关联。

**[!UICONTROL EAC]**

[!UICONTROL EAC] 表示任务或项目完成后的预计总成本。选项在项目级别计算，并会从任务/子任务汇总。

* **在项目级别计算**—父任务和项目的 [!UICONTROL EAC] 是使用 [!UICONTROL EAC] 公式中的实际小时数/实际劳动力成本确定的。计算包括直接添加到父任务或项目的实际小时数/成本和费用。
* **从任务/子任务中汇总**—父任务和项目的 [!UICONTROL EAC] 是通过将每个子任务的 [!UICONTROL EAC] 相加来确定的。此计算不包括直接添加到父任务或项目的实际小时数/成本。

[!UICONTROL EAC] 计算情况列在[完工估算 (EAC) ](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=zh-Hans)中。

**绩效指标：设置**

若要设置 [!UICONTROL PIM] 和 [!UICONTROL EAC] 系统默认值：

1. 从主菜单中选择 **[!UICONTROL Setup]**。
1. 单击左侧面板菜单中的 **[!UICONTROL Project Preferences]**，然后单击 **[!UICONTROL Projects]**
1. 在 [!UICONTROL Project Status] 部分，找到 [!UICONTROL Performance Index Method]。选择基于时间或基于成本。
1. 对于 [!UICONTROL Estimate at Completion]，选择在项目级别计算或从任务/子任务中汇总。
1. 单击窗口底部的 **[!UICONTROL Save]**。

![[!UICONTROL Project Preferences] 屏幕的图像](assets/setting-up-finances-1.png)

**在单个项目**&#x200B;上设置 [!UICONTROL PIM]

1. 转到项目的登陆页面。
1. 单击左侧面板中的 **[!UICONTROL Project Details]**。
1. 打开 **[!UICONTROL Finance]** 部分。
1. 双击 **[!UICONTROL Performance Index Method]** 下面的文字来编辑它。
1. 选择基于时间或基于成本。
1. 单击“**[!UICONTROL Save]**&#x200B;更改”以完成。

![[!UICONTROL Project Details] 屏幕的图像](assets/setting-up-finances-2.png)

[!UICONTROL PIM] 可以在项目模板上设置（在模板详细信息的 [!UICONTROL Finance] 部分）。
