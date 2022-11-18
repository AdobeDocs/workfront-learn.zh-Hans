---
title: 复制现有目标
description: 了解如何在 [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
kt: 10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 复制现有目标

假设季度末，您希望为下一时段重新创建现有目标。 或者，您可能没有完成目标，需要延长到下一个时间段。 创建该目标的最佳选项是什么？ 您将需要复制和修改现有目标。

如果多个团队成员具有相似的目标并且您需要为每个目标创建一个目标，则复制现有目标也会非常有用。

<!--
Pro-tips graphic
-->

在复制目标之前，需要考虑以下事项：

* 将复制来自原始目标的所有信息，但目标期限除外（因为它是过去的）。
* 您可以复制现有目标的结果，并且这些结果将转移到新目标。
* 默认情况下，复制的结果会分配给同一所有者。
* 您无法将现有目标的进度复制到新目标。
* 在复制目标时，您无法复制目标的活动。

## 如何复制目标

1. 单击目标名称以打开 **[!UICONTROL Goal Details]** 的上界。
1. 单击3个圆点图标，然后选择 **[!UICONTROL Copy]**.
1. 更新已复制目标的以下任何信息：
   * **新目标** — 这是新目标的名称。 默认为原始目标的名称。
   * **句点** — 要实现目标的时间段。 从下拉菜单中选择一个时间段，或单击定义自定义日期以指示自定义时间段。 默认时段始终为当前季度。
   * **所有者** — 目标的所有者。 这可以是用户、团队、组或公司。 默认为原始目标的所有者。
   * **描述** — 有关目标的其他信息。

1. 检查 **[!UICONTROL Copy results]** 框。 复制目标的结果与原始目标的结果具有相同的所有者、名称和测量值。

1. 单击 **[!UICONTROL Save]**. 复制的目标将保存为“草稿”状态。

   ![图像 [!UICONTROL Goal Details] 面板 [!DNL Workfront Goals] 和 [!UICONTROL Copy] 选项](assets/03-workfront-goals-copy-a-goal.png)

1. 单击 **[!UICONTROL Activate]**，可将目标状态更新为“活动”。 目标必须具有关联的活动或结果才能“激活”。

1. 单击 **X** 的右上角 [!UICONTROL Goal Details] 面板来关闭它。

如果您复制的目标在上一时间段内未完成，并且希望在下一时间段内继续处理该目标，请执行以下操作：

1. 转到 **[!UICONTROL Goal List]**, **[!UICONTROL Check-in]** 或 **[!UICONTROL Pulse]** 中。
1. 对目标的注释，以指示该目标已复制并创建了更新的目标。
1. 关闭原始目标以保留在其原始时间段内取得的进展。 单击 **[!UICONTROL Goal Details]** 面板和选择 **[!UICONTROL Close]** 中。
1. 更新 [!UICONTROL Initial] 匹配 **[!UICONTROL Target]** 值，因此您的新目标进度会从上一时段达到的点开始计算。
