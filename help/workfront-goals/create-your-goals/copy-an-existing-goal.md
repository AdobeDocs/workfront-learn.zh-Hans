---
title: 复制现有目标
description: 了解如何在中复制现有目标 [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 复制现有目标

假设现在是季度末，并且您希望为下一期间重新创建现有目标。 或者，您可能没有完成目标，需要扩展到下一个时间段。 创建该目标的最佳选项是什么？ 您需要复制和修改现有目标。

如果多个团队成员具有相似的目标，并且您需要为每个成员创建一个目标，则复制现有目标也很有用。

<!--
Pro-tips graphic
-->

在复制目标之前，需要注意以下几点：

* 将复制原始目标中的所有信息，但目标期间除外（因为该目标期间是过去的）。
* 您可以复制现有目标的结果，这些结果将转移到新目标。
* 默认情况下，复制的结果会分配给同一所有者。
* 您无法将现有目标的进度复制到新目标。
* 复制目标时，无法复制目标的活动。

## 如何复制目标

1. 单击目标名称以打开 **[!UICONTROL Goal Details]** 面板。
1. 单击3点图标，然后选择 **[!UICONTROL Copy]**.
1. 为复制的目标更新以下任何信息：
   * **新建目标** — 这是新目标的名称。 默认值为原始目标的名称。
   * **期间** — 您希望实现目标的时段。 从下拉菜单中选择一个时间段，或单击定义自定义日期以指示一个自定义时间段。 默认期间始终为当前季度。
   * **所有者** — 目标的所有者。 这可以是用户、团队、组或公司。 默认值为原始目标的所有者。
   * **描述** — 有关目标的其他信息。

1. 查看 **[!UICONTROL Copy results]** 框（如果原始目标已添加结果，而您希望将它们复制到新目标）。 复制的目标结果与原始目标的结果具有相同的所有者、名称和测量值。

1. 单击 **[!UICONTROL Save]**. 复制的目标将以“草稿”状态保存。

   ![的图像 [!UICONTROL Goal Details] 面板位于 [!DNL Workfront Goals] 使用 [!UICONTROL Copy] option](assets/03-workfront-goals-copy-a-goal.png)

1. 单击 **[!UICONTROL Activate]**，会将目标状态更新为“活动”。 目标必须具有关联的活动或结果才能“激活”。

1. 单击 **X** 右上角 [!UICONTROL Goal Details] 面板将其关闭。

如果复制的目标未在上一时间段内完成，并且希望在下一时间段内继续处理该目标，请执行以下操作：

1. 转到中的原始目标 **[!UICONTROL Goal List]**， **[!UICONTROL Check-in]** 区域，或 **[!UICONTROL Pulse]** 部分。
1. 对目标的注释，以指示已复制该目标并创建了更当前的目标。
1. 关闭原始目标以保留在原始时间段内取得的进展。 单击 **[!UICONTROL Goal Details]** 面板并选择 **[!UICONTROL Close]** 从菜单中。
1. 更新 [!UICONTROL Initial] 要匹配的新结果的值 **[!UICONTROL Target]** 上次结果的值，这样您的新目标进度将从上次达到的时间点开始计算。
