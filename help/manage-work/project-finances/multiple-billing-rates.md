---
title: 了解多个计费费率
description: 在Workfront中，项目经理能够覆盖特定项目中的系统计费费率。
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 了解多个计费费率

在 [!DNL Workfront]，项目经理便能够覆盖特定项目中的系统计费费率。 以前，当将新计费率应用于项目时，它不仅会影响将来的小时数，还会影响已登录项目的小时数。

使用 [!DNL Workfront]由于新增了多计费费率功能，项目经理能够决定应用计费费率的时间段。 这样，如果已协商或更改了某个费率，项目经理就可以确定该费率何时生效。

## 更改开单费率

1. 转到项目的登录页面。 选择 **[!UICONTROL Billing Rates]** 中。

   ![选择的图像 [!UICONTROL Billing Rates] in [!DNL Workfront]](assets/project-finances-1.png)

1. 从 **[!UICONTROL Billing Rates]** ，单击 **[!UICONTROL Add Billing Rate]** 按钮。 选择 **[!UICONTROL New Billing Rate]** 从下拉菜单中。

   ![选择的图像 [!UICONTROL New Billing Rate] in [!DNL Workfront]](assets/project-finances-2.png)

1. 的 [!UICONTROL New Billing Rate] 对话框。 从 **[!UICONTROL Job Role]** 下拉列表，选择要应用新开单费率的作业角色。

   ![在新计费费率中选择作业角色的图像 [!DNL Workfront]](assets/project-finances-3.png)

1. 选择作业角色后， [!UICONTROL Default Billing Rate] 和 [!UICONTROL Billing Rate 1] 字段。 在 [!UICONTROL Billing Rate 1] 字段。 如果该计费费率适用于整个项目（已记录的过去、现在和将来的小时数），请单击 **[!UICONTROL Save]** 按钮。

   ![保存适用于 [!DNL Workfront]](assets/project-finances-5.png)

1. 如果新计费率仅适用于特定时间段，请单击 **[!UICONTROL Add Rate]** 按钮。 的 [!UICONTROL Billing Rate 1 End Date] 和 [!UICONTROL Billing Rate 2] 字段。 输入的结束日期 [!UICONTROL Billing Rate 1]. 您不能输入的开始日期 [!UICONTROL Billing Rate 1] 因为系统假定它在项目开始时启动。

   ![一种图像，用于创建适用于特定时段的新计费费率，从 [!DNL Workfront]](assets/project-finances-6.png)

1. 如果情况并非如此：

   * 输入的默认开单费率 [!UICONTROL Billing Rate 1].
   * 选择的结束日期 [!UICONTROL Billing Rate 1] ([!UICONTROL Default Billing Rate])。
   * 的开始日期 [!UICONTROL Billing Rate 2] 将自动设置为 [!UICONTROL Billing Rate 1] 结束。
   * 在 [!UICONTROL Billing Rate 2] 中。
   * 根据需要，通过单击 **[!UICONTROL Add Rate]** 按钮。
   * 完成后，单击 **[!UICONTROL Save]**.
   * 所有账单费率都将显示在 [!UICONTROL Billing Rates] 选项卡。
   ![创建适用于 [!DNL Workfront]](assets/project-finances-7.png)
