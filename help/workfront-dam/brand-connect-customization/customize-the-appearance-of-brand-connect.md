---
title: 自定义外观 [!UICONTROL Brand Connect]
description: 了解如何自定义导航栏和页脚，以及如何在中自定义主页和登录页面 [!UICONTROL Brand Connect] 表示 [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 自定义的外观 [!UICONTROL Brand Connect]

在此视频中，您将学习如何：

* 自定义导航栏和页脚
* 自定义主页和登录页面

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12)

## 其他 [!UICONTROL Appearance] 设置

的 [!UICONTROL Font] 选项 [!UICONTROL Appearance] 菜单样式 [!UICONTROL Brand Portal] 中。 支持800多种Google字体。

![的 [!UICONTROL Font] 选项 [!UICONTROL Appearance] 菜单样式 [!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## 主页小组件

自定义 [!UICONTROL Brand Connect] 主页以匹配您的组织。 使用小组件，您可以添加文件夹和图像滑块等元素。 如果贵组织具有多个 [!UICONTROL Brand Connects]，则每个页面都有其自己的主页，您可以为其提供不同的外观。

![可用小组件的屏幕截图 [!UICONTROL Brand Connect] homepage](assets/03-brand-connect-home-page-widgets.png)

以下小组件可用：

**A.轮播** — 在图像滑块中显示多个资产。 您可以向每个资产添加描述。 单击“添加”图标以选择要在轮播中显示的图像。

**B.文件夹** — 显示包含选定资产的文件夹。 单击添加图标以打开 [!UICONTROL Asset Chooser] 以便您选择文件夹。 文件夹中的资产对 [!UICONTROL Brand Connect] 用户，但只能由具有权限的用户下载。

**C.灯箱** — 显示现有 [!UICONTROL Lightbox]. 中的资产 [!UICONTROL Lightbox] 将显示为 [!UICONTROL Brand Connect] 用户，但只能由具有权限的用户下载。

**D.品牌准则** — 在主页上显示品牌准则，而不是在顶部导航栏中显示/添加。

**E.说明** — 用于显示短文本段。

**F.填写的说明** — 输入要在灰色背景中显示的文本复制块。

**G.HTML** — 使用HTML和CSS创建自定义内容。 例如，您可以嵌入指向视频的链接。 有些 [HTML标记以避免](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html).

## 添加搜索栏

如果您为组织的 [!UICONTROL Brand Connect]，用户必须单击 [!UICONTROL Assets] 区域来执行搜索。

但是，系统管理员可以使用HTML小组件和此HTML标记创建搜索栏：

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
