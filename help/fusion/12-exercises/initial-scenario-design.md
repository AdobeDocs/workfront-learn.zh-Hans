---
title: 初始方案设计
description: 了解首次登录Workfront Fusion以及构建第一个场景时的一些基本导航提示。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: e639d3391ea6a8b46592dd18cf57b9eed50fbf8c
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 0%

---

# 初始方案设计

了解首次登录Workfront Fusion以及构建第一个场景时的一些基本导航提示。

## 先决条件

1. 本练习需要使用Workfront试用版。 您可以通过填写来请求一个 [此表单](https://forms.office.com/r/f1J8HRGrNY). 如果您无法访问表单，请将您的姓名、电子邮件地址和公司名称发送到wfttstdr@adobe.com。
1. Fusion练习假定您已观看了与练习对应的演练视频。 在这个案例中 [初始方案设计演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/understand-the-basics/initial-scenario-design-walkthrough.html?lang=en).


## 练习概述

在Workfront中为项目列表CSV文件中的每一行创建一个新项目。

![初始方案设计图像1](../12-exercises/assets/initial-scenario-design-1.png)

## 要遵循的步骤

1. 在场景部分创建一个名为“Fusion启用练习”的文件夹。
1. 单击进入文件夹，然后单击“创建新方案”。

   ![初始方案设计图像2](../12-exercises/assets/initial-scenario-design-2.png)

1. 在下一页，搜索Workfront并选择该应用程序。 然后单击“Continue（继续）”。
1. 在场景设计器屏幕的左上角，将场景重命名为“初始场景设计”
1. 单击屏幕中心的空触发器模块，选择Workfront应用程序，然后选择“下载文档”模块。

   **验证模块与您的Workfront帐户的连接。**

1. 要首次创建连接，请单击添加按钮。

   ![初始方案设计图像3](../12-exercises/assets/initial-scenario-design-3.png)

1. 为连接命名，如“我的Workfront 2020”

   ![初始方案设计图像4](../12-exercises/assets/initial-scenario-design-4.png)

1. 输入的URL **您的Workfront实例**，然后单击下一步。

   ![初始方案设计图像5](../12-exercises/assets/initial-scenario-design-5.png)

1. 输入密码，然后单击“登录”。

   **已建立连接。 现在，输入要从Workfront下载的文档的文档ID。**

   ![初始方案设计图像7](../12-exercises/assets/initial-scenario-design-7.png)

1. 返回Workfront。 在“Fusion练习文件”文件夹中，选择“_Fusion2020_Project List.csv”，然后单击左侧面板中的“文档详细信息”。 从URL地址复制文档ID号（这是URL中的第一个长数字）。

   ![初始方案设计图像8](../12-exercises/assets/initial-scenario-design-8.png)

1. 返回到Fusion并在“文档ID”字段中粘贴该编号，然后单击“确定”。
1. 最佳做法是在创建模块时重命名模块。 右键单击Workfront模块，然后选择“重命名”。 将模块命名为“获取项目列表”。

   **接下来，您将分析刚刚下载的CSV文件，以便访问文件中的每一行。 每行创建项目时，您都将使用此信息。**

1. 单击Workfront模块的右侧以添加另一个模块。 搜索CSV应用程序并选择解析CSV模块。
1. 为6列（CSV包含标头、逗号分隔符类型）设置“解析CSV” ，并将“数据”放置到CSV字段中。 然后单击“确定”。

   ![初始方案设计图像9](../12-exercises/assets/initial-scenario-design-9.png)

1. 将此模块重命名为“解析项目列表”。
1. 在方案设计器的底部，单击保存以保存方案。
1. 单击运行一次以查看输出。

   >[!NOTE]
   >
   >忽略警告，即转换器不应是最后一个模块（这为true，但与此测试无关）。 单击“Run Anyway（仍要运行）”。

   ![初始方案设计图像10](../12-exercises/assets/initial-scenario-design-10.png)

1. 打开解析CSV模块上的执行检查器，查看模块的输入和输出。 有一个捆绑（一个CSV文件）作为输入，多个捆绑作为输出（CSV文件中的每行一个捆绑）。 它应该类似于下面的样子：

   ![初始方案设计图像11](../12-exercises/assets/initial-scenario-design-11.png)

   **添加模块以为CSV文件中的每一行创建一个项目。**

1. 添加另一个模块。 选择Workfront应用程序，然后选择创建记录模块。
1. 将记录类型设置为项目。

   >[!TIP]
   >
   >通过开始键入几个字母来搜索它，例如 *项目*，以直接使用它。

1. 然后使用Cmd/Ctrl+G查找名称（项目名称）。 选中“名称”旁边的框；该字段显示在下方。
1. 现在，选中“Planned Start Date”（计划开始日期）和“Priority”（优先级）旁边的框。
1. 单击“名称”字段，以便显示映射面板。 单击“解析CSV”模块中的“列1”字段，以将其添加到“名称”字段。 这是CSV文件中的项目名称。
1. 对于计划的开始日期，单击解析CSV模块中的列5 。
1. 对于“优先级”，从下拉菜单中选择“正常”。

   **您的映射面板应如下所示：**

   ![初始方案设计图像12](../12-exercises/assets/initial-scenario-design-12.png)

1. 单击“确定”。

   >[!NOTE]
   >
   >如果不单击“确定”并意外地再次单击回设计器，您的工作将不会保存，您将必须再次映射。

1. 右键单击Workfront模块，并将其重命名为“创建Workfront项目”。
1. 保存方案，然后单击运行一次按钮。
1. 单击最后一个模块右上角的执行检查器。

   + 您将看到已执行20个操作。 每个操作都从CSV文件中获取一个捆绑（即一行）作为输入和输出一个捆绑，该捆绑是在Workfront中创建的一个项目。 创建的项目的项目ID随输出捆绑一起显示。

   ![初始方案设计图像13](../12-exercises/assets/initial-scenario-design-13.png)

   **使用注释**

1. 注释有助于创建场景设计的可见性。 要在创建Workfront项目模块中添加注释，请右键单击并选择添加注释。 设计器窗口右侧会弹出一个面板，以便您向模块中添加注释。 键入“创建项目，该项目具有从CSV文件映射的名称、计划开始日期和优先级。”
1. 添加另一条注释以描述触发器模块(第一个Workfront模块)正在执行的操作。
1. 单击右上角的X关闭注释面板。

   + 通过单击底部工具栏中的“注释”按钮或者右键单击任何模块并添加新注释，可再次访问注释。
   + 注释按逆时间顺序排序。
   + 添加注释后，“注释”按钮上会显示一个橙色圆点。

   ![初始方案设计图像14](../12-exercises/assets/initial-scenario-design-14.png)

1. 单击控件工具栏中的保存按钮以保存方案。
1. 您可以查看在Workfront实例中创建的项目。
