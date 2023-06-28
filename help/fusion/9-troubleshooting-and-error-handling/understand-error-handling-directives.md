---
title: 了解错误处理指令
description: 了解允许继续执行的错误处理程序指令和停止执行的错误处理程序指令，请参见 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# 了解错误处理指令

在本视频中，您将了解：

* 允许继续执行的三个错误处理程序指令
* 停止执行的两个错误处理程序指令

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## 指令 — 场景继续

### 恢复

* 指定替代输出并将其提供给遇到错误的模块。
* 后续模块被处理。
* 场景执行状态被标记为“成功”。

![恢复指令的图像](assets/troubleshooting-and-error-handling-2.png)

### 中断

* 场景执行的状态存储在未完成执行的队列中，其中的错误可以手动解决。 但是，这里也提到一些例外情况。
* 不处理后续模块。
* 如果存在未处理的包，则场景执行会正常继续。
* 场景执行状态被标记为“警告”。

![Break指令的图像](assets/troubleshooting-and-error-handling-3.png)

### 忽略

* 将忽略该错误，并且不处理后续模块。
* 如果存在未处理的包，则场景执行会正常继续。
* 场景执行状态被标记为“成功”。

![Ignore指令图像](assets/troubleshooting-and-error-handling-4.png)

## 指令 — 方案停止

### 回滚

* 将立即停止场景执行，并对所有模块启动回滚阶段，以尝试将所有模块恢复到其初始状态。
* 不处理后续模块。
* 除非出现少数几种错误类型，否则在“场景”设置下指定的“连续错误数”之后，将停用场景。
* 场景执行状态被标记为“错误”。

>[!NOTE]
>
>如果没有将错误处理程序路由附加到模块，并且未选中场景设置下的“允许存储不完整的执行”设置，则这是默认行为。

![回退指令的图像](assets/troubleshooting-and-error-handling-5.png)

### 提交

* 将忽略该错误，并且不处理后续模块。
* 如果存在未处理的包，则场景执行会正常继续。
* 场景执行状态被标记为“成功”。

![Commit指令图像](assets/troubleshooting-and-error-handling-6.png)
