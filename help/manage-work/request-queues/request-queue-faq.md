---
title: 有关请求队列的常见问题解答
description: 获取有关  [!DNL  Workfront] 中请求队列的常见问题的解答。
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ec82cd0aafb89df7b3c46eb716faf3a25cd438a2
workflow-type: ht
source-wordcount: '394'
ht-degree: 100%

---

# 有关请求队列的常见问题解答

**为什么我可以看到请求队列，但我的用户看不到？**

在您的请求队列/项目的 [!UICONTROL Queue Details] 选项卡中，确保您的用户符合“谁可以向该队列添加请求？”字段的标准。

**我授予了用户访问队列的权限，但现在他们还可以看到请求队列项目。为什么？**

这与您如何授予他们访问请求队列的权限有关。

如果您使用了请求队列项目登陆页面中的 [!UICONTROL Sharing] 工具，则您授予了这些用户在项目列表中查看项目的权限。

但是，如果您只想授予他们向队列提交请求的访问权限，请转到“队列设置”，并在“谁可以向该项目添加请求”下选择相应的选项。

**我可以将请求转化为项目吗？**

可以。您可以根据需要将问题转换为任务或项目。

请查看这篇文章以获取更多信息：[转化问题。](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=zh-Hans)

**在哪里可以找到要进行编辑的请求队列？**

您可以使用导航栏中的 [!UICONTROL Search] 字段或在 [!UICONTROL Projects] 区域中找到它。

如果您从请求队列中打开一项请求，则可以在痕迹导航区域中单击项目名称。

**我可以将信息从请求自定义表单传输到项目自定义表单吗？**

可以。创建自定义表单时，请同时选择 [!UICONTROL Project] 和 [!UICONTROL Issue] 作为对象类型。在请求中附加自定义表单。当您将请求转化为项目时，自定义表单会自动附加到新项目中，并且所有字段中包含的值都会同时显示在请求自定义表单和项目自定义表单中。

**我正在查看一份项目或任务报告。我如何找出该对象源自哪个请求？**

您可以访问 **[!UICONTROL Converted Issue]** 和 **[!UICONTROL Converted Issue Originator]** 字段源中的字段，以将这些信息添加到项目和任务报告中。

**在报告中过滤请求队列的最佳方法是什么？**

如果您的项目过滤器包括&#x200B;**队列>>为公共>>等于>>无**，则您的报告仅会显示属于&#x200B;**非**&#x200B;请求队列的项目。

如果您的项目过滤器包括&#x200B;**队列>>为公共>>不等于>>无**，则您的报告仅会显示&#x200B;**属于**&#x200B;请求队列的项目。
