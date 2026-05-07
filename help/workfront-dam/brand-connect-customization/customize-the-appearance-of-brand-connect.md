---
title: 自定义 [!UICONTROL Brand Connect] 的外观
description: 了解如何自定义导航栏和页脚，以及如何为 [!UICONTROL Workfront DAM] 自定义 [!UICONTROL Brand Connect] 中的主页和登录页。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T02:02:56.632Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 97%

---

# 自定义 [!UICONTROL Brand Connect] 的外观

在本视频中，您将学习如何：

* 自定义导航栏和页脚
* 自定义主页和登录页面

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on&enablevpops=1)

## 其他 [!UICONTROL Appearance] 设置

[!UICONTROL Appearance] 菜单下的 [!UICONTROL Font] 选项以所选字体设置 [!UICONTROL Brand Portal] 中所有文本的样式。 超过 800 种 Google 字体均受到支持。

![[!UICONTROL Appearance] 菜单样式下的 [!UICONTROL Font] 选项，位于 [!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## 主页小组件

定制您 [!UICONTROL Brand Connect] 主页的外观，使其与您的组织相匹配。 通过使用小组件，您可以添加文件夹和图像滑块等元素。 如果您的组织有多个 [!UICONTROL Brand Connects]，则每个都会有自己的主页，您可以给与它们不同的外观。

![[!UICONTROL Brand Connect] 主页可用小组件的屏幕快照](assets/03-brand-connect-home-page-widgets.png)

以下是可用的小组件：

**A. 轮播**——在图像滑块中显示多个资源。 您可以为每个资源添加描述。 单击“添加”图标来选择要在轮播中显示的图像。

**B. 文件夹**——显示包含选定资源的文件夹。 单击“添加”图标打开 [!UICONTROL Asset Chooser]，以选择一个文件夹。 [!UICONTROL Brand Connect] 用户可以看到文件夹中的资源，但只有具有许可权限的人才能下载。

**C. Lightbox**——显示现有的 [!UICONTROL Lightbox]。 [!UICONTROL Brand Connect] 用户可以看到 [!UICONTROL Lightbox] 中的资源，但只有获得许可权限的人才能下载。

**D. 品牌指南**——在主页上显示品牌指南，而不是在顶部导航栏中显示。

**E. 描述**——用于显示短文本。

**F. 填充的描述**——输入要在灰色背景上显示的文本复制块。

**G。 HTML** — 使用HTML和CSS创建自定义内容。 例如，您可以嵌入视频链接。 有一些 [HTML 标记需要避免使用。](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html)

## 添加搜索栏

如果您为您组织的 [!UICONTROL Brand Connect] 设计了自定义主页，用户必须单击进入 [!UICONTROL Assets] 区域来运行搜索。

但系统管理员可以使用 HTML 小组件和以下 HTML 标记创建搜索栏：

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
