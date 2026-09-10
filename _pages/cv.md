---
layout: archive
permalink: /cv/
title: '<span class="i18n-en">CV</span><span class="i18n-zh">简历</span>'
seo_title: "CV"
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div class="i18n-en" markdown="1">

<!-- Once you have a PDF version, drop it in files/ and uncomment the line below:
[Download PDF]({{ base_path }}/files/cv.pdf){: .btn}
-->

Education
======
* Ph.D. in Computer Science, University of Warwick, 2026– (incoming, starting October 2026)
* M.Sc. in Artificial Intelligence, University of Southampton, expected December 2026

Research experience
======
* **MSc dissertation — multimodal emotion recognition on SEED-VII (`seedvii-aeon`)**
  * University of Southampton, supervised by Prof. Tony Bagnall
  * Benchmarked classical time-series classifiers from aeon (MultiRocket, Hydra, Arsenal, DrCIF, HIVE-COTE 2), deep-learning baselines (DECNN, EEGNet, InceptionTime), a reproduction of the dataset paper's MAET transformer, and heterogeneous EEG + eye-tracking ensembles across four evaluation protocols
  * Identified a stimulus-duration confound: clip length alone classifies at 67.5% under LOSO against 14.3% chance, so cross-video protocols are required for any honest claim on this dataset
  * Reported validation-selected ensemble weights and a documented 8-point gap in the MAET reproduction rather than test-tuned figures
* EEG algorithm optimisation — parameter-efficient tuning (LoRA-One and related methods) for neural signal models
* Semantic and emotion decoding from EEG, including visualisation of the decoded representations
* 3D medical image segmentation — Light-UNETR architectures on left atrium datasets

Skills
======
* Deep learning: PyTorch, transformer architectures, parameter-efficient fine-tuning (LoRA)
* Domains: EEG / neural signal processing, medical image segmentation, time-series classification
* Engineering: Python, experiment tracking and reproducible training pipelines

{% if site.publications.size > 0 %}
Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% endif %}

Contact
======
* Email: [Fuwen.Li@warwick.ac.uk](mailto:Fuwen.Li@warwick.ac.uk)
* GitHub: [li-f8](https://github.com/li-f8)

</div>

<div class="i18n-zh" markdown="1">

<!-- 有 PDF 版简历后，放到 files/ 目录并取消下面这行的注释：
[下载 PDF]({{ base_path }}/files/cv.pdf){: .btn}
-->

教育经历
======
* 计算机科学 博士，华威大学（University of Warwick），2026 年 10 月入学
* 人工智能 硕士，南安普顿大学（University of Southampton），2026 年 12 月毕业

研究经历
======
* **硕士毕业设计——SEED-VII 多模态情感识别（`seedvii-aeon`）**
  * 南安普顿大学，导师 Prof. Tony Bagnall
  * 在四种评估协议下横向比较 aeon 的经典时间序列分类器（MultiRocket、Hydra、Arsenal、DrCIF、HIVE-COTE 2）、深度学习基线（DECNN、EEGNet、InceptionTime）、对数据集原论文 MAET 模型的复现，以及 EEG 与眼动的异构集成
  * 发现刺激时长混淆：仅凭片段时长在 LOSO 下即可达到 67.5% 准确率（随机为 14.3%），因此该数据集上任何可信结论都必须建立在跨视频协议之上
  * 集成权重在验证集上选择而非测试集调优，MAET 复现与原文 8 个百分点的差距如实报告
* EEG 算法优化——面向神经信号模型的参数高效微调（LoRA-One 及相关方法）
* 脑电语义与情感解码，以及解码表征的可视化
* 三维医学图像分割——左心房数据集上的 Light-UNETR 架构

技能
======
* 深度学习：PyTorch、Transformer 架构、参数高效微调（LoRA）
* 研究领域：EEG／神经信号处理、医学图像分割、时间序列分类
* 工程能力：Python、实验管理与可复现训练流程

{% if site.publications.size > 0 %}
论文
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% endif %}

联系方式
======
* 邮箱：[Fuwen.Li@warwick.ac.uk](mailto:Fuwen.Li@warwick.ac.uk)
* GitHub：[li-f8](https://github.com/li-f8)

</div>
