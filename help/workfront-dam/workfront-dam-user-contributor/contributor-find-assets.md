---
title: 在中查找和组织资产 [!UICONTROL Workfront DAM]
description: 了解如何搜索资产、在文件夹中搜索、简化搜索结果、将元数据和关键字用作搜索过滤器，以及 [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 参与者：查找资产

在此视频中，您将学习如何：

* 搜索资产
* 在文件夹中搜索
* 简化搜索结果
* 将元数据和关键字用作搜索过滤器
* 查看文件夹详细信息
* 查看和更新资产元数据和关键词

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## 基本搜索标准

基本搜索会检查文件名、元数据字段、关键字和资产内容（具体取决于资产类型）。 它不包括文件夹名称。

大多数搜索结果完全匹配。 此“完全匹配”规则的例外是： [!UICONTROL Workfront DAM] 搜索文件名字段。 [!UICONTROL Workfront DAM] 返回部分文件名匹配，而不是仅返回精确的文件名匹配。

## 搜索时的用户运算符

尽管基本搜索功能通常会找到您需要的资产，但您可能需要不时使用其他搜索参数。

### 部分匹配

要查找部分匹配项，请在搜索词中添加一个星号。 星号只能在单词的结尾使用。

### AND运算符

要查找包含多个搜索词的结果，请在词之间输入AND。 这些字可以按任意顺序找到。 在所有字段中搜索时，这两个字词可能不存在于同一字段中。 例如， Paris AND Tower将在任何字段中查找同时具有这两个词语的资产。

### OR运算符

使用OR运算符查找包含任何搜索词的资产。 例如，Paris OR Arc将查找包含其中任一词语的资产，但不一定同时包含这两个词。

### 短语

要查找确切的短语，请在单词周围使用双引号。 所有的词都会按顺序找到。 例如，“埃菲尔铁塔”将按该确切顺序找到这些词。

### 负运算符

如果要从搜索结果中排除某个词，请在该词前面加一个减号(-)。 确保减号和单词之间没有空格。 例如，要排除元数据中包含“tower”字样的资产，您的搜索可以设置为“Paris-tower”。

### 空字段运算符

要查找特定元数据字段中没有任何信息的资产，请输入要以此格式搜索的字段：?[xxxxx]. 例如，如果要查找未分配关键词的资产，请输入？[关键词] 中。
