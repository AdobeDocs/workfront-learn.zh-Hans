---
title: 易访问性和清晰度
description: 学习使场景易于阅读、共享和理解的一些基本最佳实践。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11037
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '706'
ht-degree: 100%

---

# 易访问性和清晰度

在之前的 Workfront Fusion 培训中，您学习了使场景易于阅读、共享和理解的一些基本最佳实践。这些实践有助于让未来的 Workfront Fusion 用户或任何对您的 Workfront Fusion 实例进行故障排除或支持的人员更容易操作。在设计场景时，请遵循以下指导原则

## 标签和注释

一般来说，Workfront Fusion 的主要目标始终是实现简单的场景设计。以下是一些简单易懂的设计方法。

* 确保您为所有模块命名。右键单击模块并选择“重命名”。模块标签应该保持简短，但又能够让人理解该模块正在执行的操作。例如，“创建 Mktg Proj w/ Ch 模板”。
  ![错误处理场景的图像](assets/design-optimization-and-testing-1.png)
* 还要标记路由路径。即使某个路径没有直接在路由器之后使用过滤器，也可以在不填写过滤器逻辑的情况下应用标签。这样做可以让其他人了解哪些捆绑包通过了哪些路径及其原因。要为不带过滤器的路由器路径创建标签，请右键单击该路径，添加标签并保存。
  ![错误处理场景的图像](assets/design-optimization-and-testing-2.png)
* 如果模块标签或路由路径标签太短，无法说明实际发生的情况，请在适用的情况下在场景中添加注释。在整个设计和迭代过程中，您可以随时添加注释。

但是，如果在场景设计的最后，准备启动时添加注释，则可能最容易阅读和理解。从场景设计的最后（最底部，右角）反向添加注释。这样，当打开注释面板时，应用于场景开头的注释将会位于列表的顶部。

保存或关闭注释面板后，系统会对注释进行排序，其中最近创建的注释会列在最上方。在下图中，所创建的第一个注释会显示在列表底部。这里是有意将注释按照从右下角到上面的路径，最后到触发器的顺序创建的，这本质上与数据捆绑包会在场景中传递的顺序相反。这使得注释能够按照场景在数据捆绑包上实际执行的顺序显示。

![错误处理场景的图像](assets/design-optimization-and-testing-3.png)

## Workfront Fusion 模板

简化对模块和路由路径进行标记的一个好方法是使用模板。最佳实践模板可以加快为常见用例创建场景的速度。

### 模板示例

开始创建场景时，首先检查是否有可用的模板会有所帮助。例如，您希望创建一个场景，其首先会从 Workfront 中下载 CSV 文档，然后会对其进行解析。

单击“模板”部分查看是否有能够满足您的需求的公共模板。

![错误处理场景的图像](assets/design-optimization-and-testing-4.png)

单击“团队模板”选项卡可以查看团队中是否有人创建了可能会有所帮助的模板。

如果找到了自己想要使用的模板，请单击名称将其打开。

![错误处理场景的图像](assets/design-optimization-and-testing-5.png)

然后转到右上角，单击“选项”，然后选择“创建场景”。

![错误处理场景的图像](assets/design-optimization-and-testing-6.png)

### 创建模板

您可以在“团队模板”部分创建一个模板。您创建的模板可供您和您的团队使用，但是如果您单击“发布”按钮，您可以与团队外部的人员共享。

![错误处理场景的图像](assets/design-optimization-and-testing-7.png)

构建模板时，您可以包含一个向导来指导使用它的人员构建场景，并根据需要更改连接、映射数据和其他面板字段。

选中“在向导中使用”复选框，添加当有人使用您的模板构建场景时可以提供的说明。该信息将会出现在“帮助”字段中。若要允许用户在使用模板时看到此文本，请启用“用作默认值”。

![错误处理场景的图像](assets/design-optimization-and-testing-8.png)

## 想要了解详情？我们建议查看以下内容：

[Workfront Fusion 文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=zh-Hans)
