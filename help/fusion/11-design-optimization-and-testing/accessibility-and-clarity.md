---
title: 辅助功能和清晰度
description: 了解一些使情景易于阅读、共享和理解的基本最佳实践。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11037
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 辅助功能和清晰度

在Workfront Fusion培训的早期，您学习了一些使情景易于阅读、共享和理解的基本最佳实践。 这些实践有助于为将来的Workfront Fusion用户或任何疑难解答或支持您的Workfront Fusion实例的人员提供更轻松的工作。 在设计方案时，请按照以下准则提前支付费用。

## 标签和注释

通常，Workfront Fusion的主要目标始终是拥有简单的方案设计。 以下是一些简单易懂的设计制作方法。

* 确保为所有模块命名。 右键单击某个模块并选择“重命名”。 模块标签应该很短，但可以理解该模块执行的操作。 例如，“创建带Ch模板的Mktg Proj”。
   ![处理错误的方案的图像](assets/design-optimization-and-testing-1.png)
* 还为路由路径设置标签。 即使路径没有直接在路由器后使用过滤器，您也可以应用标签而不填写过滤器逻辑。 这样，其他人就可以了解哪些包传递了哪些路径以及原因。 要为没有过滤器的路由器路径创建标签，请右键单击该路径，添加标签并保存。
   ![处理错误的方案的图像](assets/design-optimization-and-testing-2.png)
* 如果模块标签或路由路径标签太短，无法阐明实际发生的情况，请在情景中添加注释（如果适用）。 在整个设计和迭代过程中，您可以根据需要随时添加注释。

但是，在您准备好启动时，如果在方案设计的最后添加注释，则阅读和了解这些注释可能最简单。 从方案设计的末尾（最底部，右角）向后工作。 这样，在打开注释面板时，应用于方案开头的注释就位于列表顶部。

保存或关闭注释面板后，注释将按最近创建的顶部进行排序。 在下图中，创建的第一个注释显示在列表底部。 注释是特意从右下角创建到上面的路径，最后创建到触发器，实质上是数据包在场景中传递的顺序与此相反。 这样，便会按照方案在数据包上实际执行的顺序显示注释。

![处理错误的方案的图像](assets/design-optimization-and-testing-3.png)

## Workfront Fusion模板

简化模块和路由路径标签的一种好方法是使用模板。 最佳实践模板可以加快为常见用例创建情景的速度。

### 模板示例

启动方案时，首先检查是否有可用的模板。 例如，您要创建一个方案，首先从Workfront下载CSV文档，然后对其进行解析。

单击“模板”部分，可查看是否有任何公共模板符合您的需求。

![处理错误的方案的图像](assets/design-optimization-and-testing-4.png)

单击“团队模板”(Team Templates)选项卡，查看团队中是否有人创建了可能有用的模板。

如果找到要使用的模板，请单击名称以将其打开。

![处理错误的方案的图像](assets/design-optimization-and-testing-5.png)

然后转到右上角，单击选项，然后选择创建方案。

![处理错误的方案的图像](assets/design-optimization-and-testing-6.png)

### 创建模板

您可以在“团队模板”(Team Templates)部分中创建模板。 您和您的团队都可以使用您创建的模板，但单击“发布”按钮后，您可以将其与团队外的人员共享。

![处理错误的方案的图像](assets/design-optimization-and-testing-7.png)

在构建模板时，您可以包含一个向导，引导使用该向导来构建方案的人员、根据需要更改连接、映射数据和其他面板字段。

选中“在向导中使用”复选框，可添加当有人使用您的模板构建方案时可用的说明。 此信息将显示在帮助字段中。 要允许用户在使用模板时查看此文本，请启用使用作为默认值。

![处理错误的方案的图像](assets/design-optimization-and-testing-8.png)

## 想了解更多吗？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
