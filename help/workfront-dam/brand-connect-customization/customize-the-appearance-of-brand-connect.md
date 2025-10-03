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
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 100%

---

# 自定义 [!UICONTROL Brand Connect] 的外观

在本视频中，您将学习如何：

* 自定义导航栏和页脚
* 自定义主页和登录页面

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on&enablevpops=1)

## 其他 [!UICONTROL Appearance] 设置

[!UICONTROL Appearance] 菜单下的 [!UICONTROL Font] 选项以所选字体设置 [!UICONTROL Brand Portal] 中所有文本的样式。超过 800 种 Google 字体均受到支持。

![[!UICONTROL Appearance] 菜单样式下的 [!UICONTROL Font] 选项，位于 [!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## 主页小组件

定制您 [!UICONTROL Brand Connect] 主页的外观，使其与您的组织相匹配。通过使用小组件，您可以添加文件夹和图像滑块等元素。如果您的组织有多个 [!UICONTROL Brand Connects]，则每个都会有自己的主页，您可以给与它们不同的外观。

![[!UICONTROL Brand Connect] 主页可用小组件的屏幕快照](assets/03-brand-connect-home-page-widgets.png)

以下是可用的小组件：

**A. 轮播**——在图像滑块中显示多个资源。您可以为每个资源添加描述。单击“添加”图标来选择要在轮播中显示的图像。

**B. 文件夹**——显示包含选定资源的文件夹。单击“添加”图标打开 [!UICONTROL Asset Chooser]，以选择一个文件夹。[!UICONTROL Brand Connect] 用户可以看到文件夹中的资源，但只有具有许可权限的人才能下载。

**C. Lightbox**——显示现有的 [!UICONTROL Lightbox]。[!UICONTROL Brand Connect] 用户可以看到 [!UICONTROL Lightbox] 中的资源，但只有获得许可权限的人才能下载。

**D. 品牌指南**——在主页上显示品牌指南，而不是在顶部导航栏中显示。

**E. 描述**——用于显示短文本。

**F. 填充的描述**——输入要在灰色背景上显示的文本复制块。

**G. HTML**——使用 HTML 和 CSS 创建自定义内容。例如，您可以嵌入视频链接。有一些 [HTML 标记需要避免使用。](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html)

## 添加搜索栏

如果您为您组织的 [!UICONTROL Brand Connect] 设计了自定义主页，用户必须单击进入 [!UICONTROL Assets] 区域来运行搜索。

但系统管理员可以使用 HTML 小组件和以下 HTML 标记创建搜索栏：

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
