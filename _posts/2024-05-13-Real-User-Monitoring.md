---
layout:     post
title:      真实用户监控
subtitle:   监控
date:       2024-05-13
author:     大风哥
header-img: img/thinking.png
catalog: true
tags:
    - 思维
    - 监控
    - Distributed tracing
    - 系统系能
---
企业软件发展的困境
引入方法，来决定何时应该介入来优化性能
介绍tracing，RUM，以及SLO
但是RUM+SLO不是银弹，还存在问题，以及如何解决问题
展望未来

* [为什么RUM](#为什么RUM)
* [解决什么问题](#解决什么问题)
* [技术细节概略](#技术细节概率)
* [如何解决](#如何解决)
    * [找到性能瓶颈](#找到性能瓶颈)
    * [分析性能瓶颈](#分析性能瓶颈)
    * [数据驱动决策](#数据驱动决策)
        * [Google-SRE](#Google-SRE)
        * [SLO/SLI](#SLO/SLI)
        * [Error-Bugget](#Error-Bugget)
* [落地工具框架参考](#落地工具框架参考)
    * [Sumologic](#Sumologic)


如何全周期的衡量产品质量的状态，是有很多办法的。比如
1. Lagging indicator. 通过用户反馈，问卷调查，CSAT等
2. Leading indicator. 比如监控系统，Logs，RUM，SRE，SLI/SLO，Error Budget等

每一种评估都是基于

这里想要介绍的通过RUM，SRE，

作为技术人员，产出技术方案是日常交付中，咨询中必不可少的一项重要工作。那么，如何才能输出高质量的解决方案设计呢？以下我给出了一些总结与反思。



