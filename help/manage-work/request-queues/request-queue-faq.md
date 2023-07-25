---
title: 有关请求队列的常见问题解答
description: 获取有关中请求队列的常见问题解答 [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner, Intermediate
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ce2aad1cd0ecb7d568ed9a01d97147cbd126ca05
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 有关请求队列的常见问题

**为什么我可以看到请求队列，但我的用户却不能？**

在 [!UICONTROL Queue Details] 选项卡中，确保您的用户符合“谁可以将请求添加到此队列？”的标准。 字段。

**我授予了用户访问队列的权限，但现在他们也可以查看请求队列项目。 为什么?**

这与您如何授予他们访问请求队列的权限有关。

如果您使用 [!UICONTROL Sharing] 工具从请求队列项目登陆页面，然后您已授予这些用户访问项目列表中的项目的权限。

但是，如果您希望授予他们仅向队列提交请求的访问权限，请转到队列设置，并在“谁可以将请求添加到此项目”下选择相应的选项。

**我可以将请求转换为项目吗？**

是. 您可以将问题转化为任务或项目，具体取决于需要。

有关更多信息，请参阅本文： [转换问题](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=en).

**可在何处找到要进行编辑的请求队列？**

您可以使用 [!UICONTROL Search] 字段，或查找列在 [!UICONTROL Projects] 区域。

如果从请求队列中打开请求，则可以在痕迹导航区域中单击项目名称。

**能否将信息从请求自定义表单传输到项目自定义表单？**

是. 创建自定义表单时，选择两者 [!UICONTROL Project] 和 [!UICONTROL Issue] 作为对象类型。 将自定义表单附加到请求。 将请求转换为项目时，自定义表单将自动附加到新项目，并且任何字段中包含的值将显示在请求和项目自定义表单中。

**我在查看项目或任务报告。 如何才能找到此对象源自哪个请求？**

您可以访问 **[!UICONTROL Converted Issue]** 和 **[!UICONTROL Converted Issue Originator]** 字段源，以将该信息添加到您的项目和任务报表。

**筛选报告中的请求队列的最佳方法是什么？**

如果您的项目筛选器包括 **队列>>为公用>>等于>>无** 您的报表将仅显示以下项目 **NOT** 请求队列。

如果您的项目筛选器包括 **队列>>为公用>>不等于>>无** 您的报表将仅显示满足以下条件的项目 **是** 请求队列。
