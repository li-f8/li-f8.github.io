---
layout: single
permalink: /research/
title: '<span class="i18n-en">Research</span><span class="i18n-zh">研究</span>'
seo_title: "Research"
author_profile: true
---

<div class="i18n-en" markdown="1">

An overview of what I work on. Papers and code will be linked here as they become available.

## EEG with parameter-efficient tuning
*Ongoing*

EEG datasets are small, noisy, and expensive to collect, which makes full fine-tuning of large models a poor fit. I work on low-rank adaptation methods — LoRA-One and its variants — to see how far the efficiency/accuracy trade-off can be pushed on neural recordings, and what the resulting adapters reveal about which parts of a model actually carry the signal.

## Semantic and emotion decoding from brain signals
*Ongoing*

Following the direction opened up by frameworks such as DeWave, I study how semantic and affective content can be decoded from EEG, and how those decoded representations can be visualised in a way that is interpretable rather than merely decorative.

## Fitting mechanisms of time-series classifiers
*Earlier work*

I analysed how HIVE-COTE ensembles fit time-series data — where their accuracy actually comes from across the constituent transforms, and what that implies for choosing or simplifying such ensembles.

## Light-UNETR for 3D medical image segmentation
*Earlier work*

A lightweight UNETR-style architecture for volumetric segmentation, evaluated on left atrium datasets, aimed at keeping transformer-based segmentation accuracy at a much lower computational cost.

</div>

<div class="i18n-zh" markdown="1">

以下是我目前和过去的研究方向，相关论文与代码会陆续在此更新。

## 面向 EEG 的参数高效微调
*进行中*

脑电数据规模小、噪声大、采集成本高，直接全量微调大模型并不合适。我关注低秩适配方法（LoRA-One 及其变体）在神经信号上的表现：效率与精度的权衡能推到什么程度，以及训练出的适配器能否反过来揭示模型中真正承载信号的部分。

## 脑信号的语义与情感解码
*进行中*

沿着 DeWave 等框架打开的方向，研究如何从 EEG 中解码语义与情感内容，以及如何把解码得到的表征做成真正可解释、而非仅仅好看的可视化。

## 时间序列分类器的拟合机制
*早期工作*

分析 HIVE-COTE 集成模型在时间序列上的拟合机制：精度究竟来自哪些组成变换，以及这对如何选择、简化这类集成模型意味着什么。

## Light-UNETR 三维医学图像分割
*早期工作*

一种轻量化的 UNETR 架构，在左心房数据集上做体数据分割，目标是以远低于原模型的计算开销保持基于 Transformer 的分割精度。

</div>
