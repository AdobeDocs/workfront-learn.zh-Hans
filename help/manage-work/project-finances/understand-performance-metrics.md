---
title: 了解性能量度
description: 性能量度包括 [!UICONTROL Performance Index Method] ([!UICONTROL PIM])和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 了解性能量度

项目经理使用的两个绩效指标包括 [!UICONTROL Performance Index Method] ([!UICONTROL PIM])和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。 系统范围的默认值可在 [!DNL Workfront] 并应用于新创建的项目。 [!UICONTROL PIM] 之后，便可在单个项目中修改。

**[!UICONTROL PIM]**

的设置 [!UICONTROL PIM] 控制方式 [!DNL Workfront] 计算其他项目性能量度，例如 [!UICONTROL Cost Performance Index] ([!UICONTROL CPI])、 [!UICONTROL Cost Schedule Performance Index] ([!UICONTROL CSI])、 [!UICONTROL Schedule Performance Index] ([!UICONTROL SPI])和 [!UICONTROL Estimate at Completion] ([!UICONTROL EAC])。

选项 [!UICONTROL PIM] 基于小时和基于成本。

* **基于小时** —Workfront在计算项目的CPI和EAC时，使用计划时间。 项目的EAC以小时为单位显示为一个数字。
* **基于成本** -Workfront在计算项目的消费物价指数和东共体时，使用计划的人工成本。 EAC显示为货币值。 使用此选项时，请确保任务分配人（用户和/或任务角色）与成本费率关联。

**[!UICONTROL EAC]**

[!UICONTROL EAC] 表示任务或项目完成时的预计总成本。 选项在项目级别计算，并从任务/子任务中汇总。

* **在项目级别计算** — [!UICONTROL EAC] 对于父任务和项目，使用 [!UICONTROL EAC] 公式。 此计算包括直接添加到父任务或项目的实际小时数/成本和费用。
* R **从任务/子任务中调用** — [!UICONTROL EAC] 对于父任务和项目，通过将 [!UICONTROL EAC] 每个子任务。 此计算不包括直接添加到父任务或项目的实际小时数/成本。

的 [!UICONTROL EAC] 计算列在“完成时计算估计(EAC)”中 <!-- link to article -->文章 [!UICONTROL [!DNL Workfront] One].

**性能量度：设置**

要设置 [!UICONTROL PIM] 和 [!UICONTROL EAC] 系统默认值：

1. 选择 **[!UICONTROL Setup]** 中。
1. 单击 **[!UICONTROL Project Preferences]** 在左侧面板菜单中，单击 **[!UICONTROL Projects]**
1. 在 [!UICONTROL Project Status] 部分，查找 [!UICONTROL Performance Index Method]. 选择基于小时或基于成本。
1. 对于 [!UICONTROL Estimate at Completion]，选择在项目级别计算或从任务/子任务中汇总。
1. 单击 **[!UICONTROL Save]** 在窗口底部。

![图像 [!UICONTROL Project Preferences] 屏幕](assets/setting-up-finances-1.png)

**已设置 [!UICONTROL PIM] 在单个项目上**

1. 转到项目的登陆页面。
1. 单击 **[!UICONTROL Project Details]** 中。
1. 打开 **[!UICONTROL Finance]** 中。
1. 双击下面的文本 **[!UICONTROL Performance Index Method]** 来编辑。
1. 选择基于小时或基于成本。
1. 单击 **[!UICONTROL Save]** 更改以完成。

![图像 [!UICONTROL Project Details] 屏幕](assets/setting-up-finances-2.png)

[!UICONTROL PIM] 可以在项目模板中， [!UICONTROL Finance] 部分。
