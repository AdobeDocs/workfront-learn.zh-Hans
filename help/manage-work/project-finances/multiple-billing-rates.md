---
title: 了解多种计费费率
description: 了解如何覆盖项目内的系统计费费率。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 100%

---

# 了解多种计费费率

在 [!DNL Workfront] 中，项目经理能够覆盖特定项目内的系统计费费率。以前，当新的计费费率应用于项目时，它不仅会影响未来的小时数，还会影响到项目中已记录的小时数。

有了 [!DNL Workfront] 新的多种计费费率功能，项目经理能够决定应该应用计费费率的时段。这样，如果费率已经得到协商或更改，项目经理便可以确定该费率应该何时生效。

## 更改计费费率

1. 转到项目的登陆页面。从左侧面板选择 **[!UICONTROL Billing Rates]**。

   ![图像：选择 [!UICONTROL Billing Rates]，位于 [!DNL Workfront]](assets/project-finances-1.png)

1. 在 **[!UICONTROL Billing Rates]** 选项卡中，单击 **[!UICONTROL Add Billing Rate]** 按钮。从下拉列表中选择 **[!UICONTROL New Billing Rate]**。

   ![图像：选择 [!UICONTROL New Billing Rate]，位于 [!DNL Workfront]](assets/project-finances-2.png)

1. 此时会显示 [!UICONTROL New Billing Rate] 对话框。从 **[!UICONTROL Job Role]** 下拉列表中，选择将要应用新计费费率的工作角色。

   ![图像：选择新计费费率的工作角色，位于 [!DNL Workfront]](assets/project-finances-3.png)

1. 选择工作角色后会出现 [!UICONTROL Default Billing Rate] 和 [!UICONTROL Billing Rate 1] 字段。在 [!UICONTROL Billing Rate 1] 字段中输入新的计费费率。如果该计费费率适用于整个项目（记录的过去、现在和未来的小时数），请单击 **[!UICONTROL Save]** 按钮。

   ![图像：保存适用于整个项目的新计费费率，位于 [!DNL Workfront]](assets/project-finances-5.png)

1. 如果新的费率仅适用于特定时段，请单击 **[!UICONTROL Add Rate]** 按钮。此时会出现 [!UICONTROL Billing Rate 1 End Date] 和 [!UICONTROL Billing Rate 2] 字段。输入 [!UICONTROL Billing Rate 1] 的结束日期。您不能为 [!UICONTROL Billing Rate 1] 输入开始日期，因为系统假设它是在项目开始时开始的。

   ![图像：创建应用于特定时段（起始时间为项目开始时）的新计费费率，位于 [!DNL Workfront]](assets/project-finances-6.png)

1. 如果情况并非如此：

   * 输入 [!UICONTROL Billing Rate 1] 的默认计费费率。
   * 选择 [!UICONTROL Billing Rate 1] ([!UICONTROL Default Billing Rate]) 的结束日期。
   * [!UICONTROL Billing Rate 2] 的开始日期将自动设置为 [!UICONTROL Billing Rate 1] 结束后的那天。
   * 在 [!UICONTROL Billing Rate 2] 部分输入所需的计费费率。
   * 单击 **[!UICONTROL Add Rate]** 按钮，根据需要继续添加计费费率。
   * 完成后，单击 **[!UICONTROL Save]**。
   * 所有计费费率均会显示在项目的 [!UICONTROL Billing Rates] 选项卡中。

   ![图像：创建适用于不同时段的新计费费率，位于 [!DNL Workfront]](assets/project-finances-7.png)
