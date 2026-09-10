---
layout: single
permalink: /research/
title: '<span class="i18n-en">Research</span><span class="i18n-zh">研究</span>'
seo_title: "Research"
author_profile: true
---

<div class="i18n-en" markdown="1">

An overview of what I work on. Papers and code will be linked here as they become available.

## Multimodal emotion recognition on SEED-VII — `seedvii-aeon`
*MSc dissertation, University of Southampton, supervised by Prof. Tony Bagnall*

A single benchmark comparing four families of methods on the SEED-VII emotion dataset under four evaluation protocols: classical time-series classifiers from [aeon](https://github.com/aeon-toolkit/aeon) (MultiRocket, Hydra, Arsenal, DrCIF, HIVE-COTE 2), deep-learning baselines (a compact 1-D DECNN, a DE-reshaped EEGNet, InceptionTime), a faithful reproduction of MAET — the dataset paper's own multimodal transformer — and heterogeneous ensembles of EEG and eye-tracking models.

The result the project turns on is a negative one. A 1-nearest-neighbour classifier that sees *nothing but the duration of each video clip* reaches 67.5% under leave-one-subject-out and 64.3% under random splits, against 14.3% chance — well above the 41% my honest ensemble reaches on the same protocols. SEED-VII's fixed 80-video stimulus design leaks the label through clip length whenever stimuli are shared between training and test data, so a strong LOSO number on this dataset is largely an artefact. Genuine above-confound signal only appears under the two cross-video protocols: +14.9 points under leave-one-video-out, +11.6 for the ensemble under subject-dependent evaluation.

Two further commitments shape the work. Ensemble weights are selected on a held-out validation split rather than on test accuracy — an earlier test-selected version scored higher, and reporting the honest number costs about a point. And the MAET reproduction is reported with its gap intact: 62.9% against the 71% published, stable across learning rates, which points at undocumented training details rather than a failure to optimise. Diagnostics along the way quantified what actually carries the pipeline: per-subject z-scoring is worth 15–22 points, more than any architectural choice in the comparison.

## HIVE-COTE on a modular base — contribution to `aeon`
*Merged June 2026*

[Pull request #3386](https://github.com/aeon-toolkit/aeon/pull/3386) to [aeon](https://github.com/aeon-toolkit/aeon), the time-series machine learning toolkit, refactors the HIVE-COTE V1 and V2 ensemble classifiers onto a shared `_BaseHIVECOTE` framework implementing CAWPE probability weighting. Two of the library's flagship classifiers had been carrying substantial duplicated logic; the change removes it while preserving scikit-learn compatibility and the existing public API, with deprecation handling for what had to move. Merged after several rounds of maintainer review with Prof. Tony Bagnall and Dr. Matthew Middlehurst.

## Light-UNETR for 3D medical image segmentation
*Earlier work*

A lightweight UNETR-style architecture for volumetric segmentation, evaluated on left atrium datasets, aimed at keeping transformer-based segmentation accuracy at a much lower computational cost.

</div>

<div class="i18n-zh" markdown="1">

以下是我目前和过去的研究方向，相关论文与代码会陆续在此更新。

## SEED-VII 多模态情感识别 —— `seedvii-aeon`
*硕士毕业设计，南安普顿大学，导师 Prof. Tony Bagnall*

在 SEED-VII 情感数据集上，用四种评估协议横向比较四类方法：来自 [aeon](https://github.com/aeon-toolkit/aeon) 的经典时间序列分类器（MultiRocket、Hydra、Arsenal、DrCIF、HIVE-COTE 2）、深度学习基线（轻量一维 DECNN、按 DE 特征重构的 EEGNet、InceptionTime）、对数据集原论文模型 MAET 的忠实复现，以及 EEG 与眼动模型的异构集成。

整个项目的关键结论是一个否定性结果：一个**只看视频片段时长**的 1-近邻分类器，在跨被试（LOSO）协议下能达到 67.5%、随机划分下 64.3%，而随机猜测只有 14.3%——这远高于我的诚实集成模型在相同协议下的约 41%。SEED-VII 固定的 80 段视频刺激设计，使得只要训练集和测试集共享刺激，标签就会通过片段时长泄漏；因此这个数据集上漂亮的 LOSO 数字很大程度上是伪影。真正高于混淆基线的信号只出现在两种跨视频协议下：LOVO 高出 14.9 个百分点，被试内评估下集成模型高出 11.6 个百分点。

另有两点方法上的坚持。集成权重在留出的验证集上选择，而不是在测试集准确率上挑——早期用测试集选权重的版本数字更好看，换成诚实做法大约损失 1 个百分点。MAET 复现也保留了差距如实报告：62.9%，对比原文的 71%，且在不同学习率下稳定，说明差距来自论文未记录的训练细节，而非我这边没调好。过程中的诊断实验还量化了流程里真正起作用的部分：按被试 z-score 归一化贡献了 15–22 个百分点，比这次比较中任何架构选择的影响都大。

## 把 HIVE-COTE 重构到模块化基类 —— `aeon` 开源贡献
*2026 年 6 月合并*

向时间序列机器学习工具库 [aeon](https://github.com/aeon-toolkit/aeon) 提交的 [Pull Request #3386](https://github.com/aeon-toolkit/aeon/pull/3386)，把 HIVE-COTE V1 与 V2 两个集成分类器重构到共享的 `_BaseHIVECOTE` 框架上，并在其中实现 CAWPE 概率加权。这两个旗舰分类器此前携带大量重复逻辑，重构在消除重复的同时保持了 scikit-learn 兼容性与既有公开 API，对必须迁移的部分做了弃用处理。经 Prof. Tony Bagnall 与 Dr. Matthew Middlehurst 多轮维护者评审后合并。

## Light-UNETR 三维医学图像分割
*早期工作*

一种轻量化的 UNETR 架构，在左心房数据集上做体数据分割，目标是以远低于原模型的计算开销保持基于 Transformer 的分割精度。

</div>
