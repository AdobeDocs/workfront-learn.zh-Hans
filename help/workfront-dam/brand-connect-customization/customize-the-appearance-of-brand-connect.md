---
title: 自定义外观 [!UICONTROL Brand Connect]
description: 了解如何自定义导航栏和页脚，以及自定义中的主页和登录页面 [!UICONTROL Brand Connect] 对象 [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 自定义的外观 [!UICONTROL Brand Connect]

在本视频中，您将学习如何：

* 自定义导航栏和页脚
* 自定义主页和登录页面

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on)

## 其他 [!UICONTROL Appearance] 设置

此 [!UICONTROL Font] 下的选项 [!UICONTROL Appearance] 菜单设置整个文本样式 [!UICONTROL Brand Portal] 在选定字体中。 支持800多种Google字体。

![此 [!UICONTROL Font] 下的选项 [!UICONTROL Appearance] 菜单样式 [!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## 主页小组件

自定义您的外观 [!UICONTROL Brand Connect] 主页以匹配您的组织。 使用小部件，您可以添加文件夹和图像滑块等元素。 如果您的组织有多个 [!UICONTROL Brand Connects]，每个页面都有自己的主页，您可以提供不同的外观。

![您可用的小部件的屏幕截图 [!UICONTROL Brand Connect] homepage](assets/03-brand-connect-home-page-widgets.png)

这些小组件可用：

**A.轮播** — 在图像滑块中显示多个资源。 您可以向每个资源添加描述。 单击添加图标以选择要显示在轮播中的图像。

**B.文件夹** — 显示包含选定资源的文件夹。 单击添加图标以打开 [!UICONTROL Asset Chooser] 以便选择文件夹。 文件夹中的资产对可见 [!UICONTROL Brand Connect] 用户，但只能由具有权限的用户下载。

**C.灯箱** — 显示现有 [!UICONTROL Lightbox]. 中的资产 [!UICONTROL Lightbox] 将对可见 [!UICONTROL Brand Connect] 用户，但只能由具有权限的用户下载。

**D.品牌指南** — 在主页上显示“品牌指南”，而不是/不在顶部导航栏中显示。

**E.说明** — 用于显示短文本。

**F.填写的说明** — 输入要显示在灰色背景上的文本复制块。

**G.HTML** — 使用HTML和CSS创建自定义内容。 例如，您可以嵌入指向视频的链接。 有些是 [HTML要避免的标记](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html).

## 添加搜索栏

如果您为贵组织的 [!UICONTROL Brand Connect]，用户必须单击 [!UICONTROL Assets] 区域以运行搜索。

但系统管理员可以使用HTML小部件和此HTML标记创建搜索栏：

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
