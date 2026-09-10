---
permalink: /
title: '<span class="i18n-en">About Me</span><span class="i18n-zh">关于我</span>'
seo_title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="i18n-en" markdown="1">

I am an incoming PhD student at the University of Warwick, starting in October 2026, and I am completing an MSc in Artificial Intelligence at the University of Southampton, due to finish in December 2026.

My work sits between machine learning theory and the engineering that makes it usable. The question I keep returning to is *why* a model fits the way it does — which part of it carries the signal, and what is really being measured when a number goes up.

My MSc dissertation, [`seedvii-aeon`](/research/), is that question in concrete form. Benchmarking classical time-series classifiers, deep baselines and multimodal ensembles on the SEED-VII emotion dataset, I found that a classifier seeing nothing but the *duration* of each video clip scores 67.5% under leave-one-subject-out — far above what the actual EEG and eye-tracking models achieve. Much of the reported performance on that dataset is a stimulus-design artefact rather than emotion recognition, and only cross-video protocols survive the check. Before that I worked on lightweight transformer segmentation with Light-UNETR on left atrium volumes.

EEG is where I am focused now, and it sharpens the same question. Neural recordings are small, noisy, and expensive to collect, so full fine-tuning of a large model is the wrong tool. I work on parameter-efficient tuning — LoRA-One and related low-rank methods — both to make these models practical and because the adapters that result are themselves evidence about where the signal lives. Alongside this I study semantic and emotion decoding from brain signals, in the direction opened up by frameworks such as DeWave, including how the decoded representations can be visualised in a way that is genuinely interpretable rather than merely decorative.

I am currently preparing for my doctoral research. Papers, code, and notes will appear here as the work develops.

### Get in touch

Email is the fastest way to reach me — [Fuwen.Li@warwick.ac.uk](mailto:Fuwen.Li@warwick.ac.uk). Code lives on [GitHub](https://github.com/li-f8).

</div>

<div class="i18n-zh" markdown="1">

我将于 2026 年 10 月入学华威大学（University of Warwick）攻读博士学位，目前在南安普顿大学（University of Southampton）攻读人工智能硕士，2026 年 12 月毕业。

我的工作处在机器学习理论与工程实现之间。我反复回到的问题是：模型*为什么*会这样拟合——它的哪一部分真正承载了信号，以及当一个数字变好时，我们究竟测到了什么。

我的硕士毕业设计 [`seedvii-aeon`](/research/) 就是这个问题的具体形态。在 SEED-VII 情感数据集上比较经典时间序列分类器、深度学习基线与多模态集成时，我发现一个**只看视频片段时长**的分类器在跨被试协议下能拿到 67.5%，远高于真正的 EEG 与眼动模型。也就是说，该数据集上很多已报告的性能来自刺激设计带来的伪影，而非情感识别本身，只有跨视频协议下的结论经得起检验。在此之前，我用 Light-UNETR 在左心房数据上做过轻量化的 Transformer 分割。

EEG 是我目前的重心，它把同一个问题问得更尖锐。神经信号数据量小、噪声大、采集成本高，全量微调大模型并不是合适的工具。我关注参数高效微调——LoRA-One 及相关低秩方法——一方面让这类模型真正可用，另一方面，训练出的适配器本身就是关于「信号藏在哪里」的证据。与此同时，我研究脑信号的语义与情感解码，沿着 DeWave 一类框架打开的方向，也包括如何把解码得到的表征做成真正可解释、而非仅仅好看的可视化。

我正在为博士阶段的研究做准备，后续会在这里持续更新论文、代码与研究笔记。

### 联系我

邮件是最快的方式：[Fuwen.Li@warwick.ac.uk](mailto:Fuwen.Li@warwick.ac.uk)。代码在 [GitHub](https://github.com/li-f8)。

</div>
