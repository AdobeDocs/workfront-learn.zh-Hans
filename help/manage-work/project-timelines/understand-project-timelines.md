---
title: 浏览Workfront中的项目时间线
description: 了解如何分配任务、使用甘特图和关键路径功能、通过视图监测项目、有效地安排任务以及通过应用限制来实现最佳的项目规划。
activity: use
feature: Work Management
thumbnail: 335213.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: '2024-11-01T00:00:00.000Z'
recommendations: noDisplay,catalog
jira: KT-8953
exl-id: ba993197-9f84-4fc0-86cc-cf849c889f56
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:48:54.364Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 700
ht-degree: 76%

---

# 浏览Workfront中的项目时间线

您将了解的内容：

* 获取使用 Workfront 进行项目规划和管理的概述。 了解父任务如何将多个子任务分组，这些子任务会被分配给相关的工作角色，然后再分配给具有必要技能的用户。 前置任务表示任务之间的顺序关系，没有前置任务的任务可以同时进行。 甘特图提供了清晰可见的时间线，而关键路径功能则突出显示了可能因延误而导致项目延迟的任务。
* Workfront 中的不同视图，例如用于规划的标准视图和用于监测进度的状态视图，其中包括进度、评论、文档、问题、审批、关键路径和里程碑的标志。 可以跟踪最近的活动，以查看更新和注释。
* 可以从开始日期或完成日期进行计划，而 Workfront 则会根据任务持续时间和前置任务计算相应的日期。 该视频建议从开始日期开始安排关键的完成日期，以留出一些余地。 其中还介绍了任务限制，例如“尽快”和“尽可能晚”，说明了它们会如何影响任务计划。 可以通过创建自定义视图来显示任务限制。

>[!VIDEO](https://video.tv.adobe.com/v/3435845/?captions=chi_hans&quality=12&learn=on&enablevpops=1)

>[!IMPORTANT]
>
>有关持续时间类型和任务限制的更完整说明，请参阅[了解和管理持续时间类型以及任务限制。](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md)

## 要点

* **任务管理和分配：**&#x200B;父任务将多个子任务分组，这些子任务将分配给工作角色，以后将分配给具有必要技能的用户。 前置任务&#x200B;指示顺序关系，而无前置任务的任务可以并行完成。  
* **甘特图和关键路径：**&#x200B;甘特图提供了项目的可视时间线，而关键路径功能突出显示了在任务打滑时可能延迟项目的任务。  
* **视图和监测：** Workfront 中的不同视图，例如用于规划的标准视图以及用于监测的状态视图，其中包括进度、评论、文档、问题、审批、关键路径和里程碑的标志。 也可以跟踪最近的活动。  
* **计划选项：**&#x200B;项目可以从开始日期或完成日期开始计划，Workfront会根据任务持续时间和前置任务计算相应的日期。 建议对关键完成日期从开始日期&#x200B;进行计划，以允许一些宽限。  
* **任务限制：**&#x200B;任务限制（如“尽快”和“尽可能迟”）会影响任务计划。 在项目创建后更改计划模式&#x200B;可能会影响任务限制和计划日期。 可创建&#x200B;自定义视图以显示任务限制。  


## 更改或不更改项目时间线上的日期……

| 优点（更改日期） | 缺点（更改日期） | 优点（不改变日期） | 缺点（不改变日期） |
|---------------------------|---------------------------|---------------------------|---------------------------|
| <ul><li>减轻压力/为用户提供最新的期望——”_创作者们不知道什么是真实的_“</li><li>准确分配资源（尤其是在工作负载平衡器中）</li><li>使用日记帐条目报告（或项目持续时间）来调出日期变更</li><li>使用条件显示项目是否超出范围</li><li>可以通过添加自定义表单（或使用问题）来跟踪更改——为什么推送、由谁推送、推送了多长时间</li></ul> | <ul></li><li>报告未反映真实情况，因此数据具有误导性</li><li>对进度的错误认知——错误地认为一切都在按计划进行</li><li>促进一种总是推迟时间线而不是解决根本原因的文化</li><li>利益相关者丧失信心/团队失去按时完成任务的认知 </li></ul> | <ul></li><li>准确呈现项目时间线——数据可用于分析，并清晰地讲述发生的事情</li><li>可选择更改持续时间或为前置任务添加延迟</li><li>轻松识别未来项目规划/风险管理的流程改进</li><li>选择利用基线来捕获原始项目计划并将其用作比较</li><li>如果你没有足够的人手去做这件事，并且无法为所有事情都安排人手，那就不要去做</li></ul> | <ul></li><li>用户感到困惑和/或沮丧——尽管他们刚刚收到通知，但仍有大量“延迟”任务</li><li>资源原本按照原计划进行了有效分配，但现在却因工作延误而超负荷</li><li>项目时间线无法用于向利益相关者清楚地传达更新信息</li></ul> |


## 有关此主题的推荐教程

* [从项目时间线跟踪进度](/help/manage-work/project-timelines/track-work-progress-from-the-project-timeline.md)
* [了解日期类型和进度状态](/help/manage-work/project-timelines/understand-task-dates-and-progress-status.md)
* [了解和管理持续时间类型和任务限制](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md)

