---
title: 了解多个记帐费率
description: 了解如何在项目中覆盖系统记帐费率。
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
ht-degree: 0%

---

# 了解多个记帐费率

范围 [!DNL Workfront]，项目经理能够覆盖特定项目中的系统记帐费率。 以前，当将新记帐费率应用于项目时，它不仅会影响未来的小时数，还会影响项目中已记录的小时数。

替换为 [!DNL Workfront]的新多计费率功能中，项目经理能够决定应应用计费率的时段。 这样一来，如果费率已经议定或更改，项目经理可以确定费率何时生效。

## 更改记帐费率

1. 转到项目的登陆页面。 选择 **[!UICONTROL Billing Rates]** 从左侧面板中。

   ![选择的图像 [!UICONTROL Billing Rates] 在 [!DNL Workfront]](assets/project-finances-1.png)

1. 从 **[!UICONTROL Billing Rates]** 选项卡，单击 **[!UICONTROL Add Billing Rate]** 按钮。 选择 **[!UICONTROL New Billing Rate]** 从下拉菜单中查找。

   ![选择的图像 [!UICONTROL New Billing Rate] 在 [!DNL Workfront]](assets/project-finances-2.png)

1. 此 [!UICONTROL New Billing Rate] 对话框。 从 **[!UICONTROL Job Role]** 在下拉列表中，选择要应用新计费率的工作角色。

   ![在中为新记帐费率选择工作角色的图像 [!DNL Workfront]](assets/project-finances-3.png)

1. 选择工作角色后， [!UICONTROL Default Billing Rate] 和 [!UICONTROL Billing Rate 1] 字段。 在中输入新的计费率 [!UICONTROL Billing Rate 1] 字段。 如果该记帐费率适用于整个项目（记录的过去、现在和未来小时数），请单击 **[!UICONTROL Save]** 按钮。

   ![保存适用于整个项目的新记帐费率的图像 [!DNL Workfront]](assets/project-finances-5.png)

1. 如果新的记帐费率仅适用于特定时段，请单击 **[!UICONTROL Add Rate]** 按钮。 此 [!UICONTROL Billing Rate 1 End Date] 和 [!UICONTROL Billing Rate 2] 将显示字段。 输入结束日期 [!UICONTROL Billing Rate 1]. 不能输入开始日期 [!UICONTROL Billing Rate 1] 因为系统假定它在项目开始时启动。

   ![创建适用于特定时段的新计费率的图像，从项目的开头开始 [!DNL Workfront]](assets/project-finances-6.png)

1. 如果不是这种情况：

   * 输入默认记帐费率 [!UICONTROL Billing Rate 1].
   * 选择结束日期 [!UICONTROL Billing Rate 1] ([!UICONTROL Default Billing Rate])。
   * 开始日期 [!UICONTROL Billing Rate 2] 将自动设置为之后的第二天 [!UICONTROL Billing Rate 1] 结束。
   * 在中输入所需的计费率 [!UICONTROL Billing Rate 2] 部分。
   * 根据需要继续添加记帐费率，方法是单击 **[!UICONTROL Add Rate]** 按钮。
   * 完成后，单击 **[!UICONTROL Save]**.
   * 所有记帐费率将显示在 [!UICONTROL Billing Rates] 选项卡。

   ![创建适用于中不同时段的新记帐费率的图像 [!DNL Workfront]](assets/project-finances-7.png)
