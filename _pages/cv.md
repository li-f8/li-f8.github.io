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
* Ph.D., University of Warwick, 2026– (incoming, starting October 2026)
<!-- Add the programme/department and supervisor here once you want them shown -->
* M.Sc. in Artificial Intelligence, University of Southampton, Oct 2025 – Dec 2026
  * Expected classification: Distinction

Research experience
======
* **MSc dissertation — multimodal emotion recognition on SEED-VII (`seedvii-aeon`)**, Sept 2025 – present
  * University of Southampton, supervised by Prof. Tony Bagnall
  * Benchmarked classical time-series classifiers from aeon (MultiRocket, Hydra, Arsenal, DrCIF, HIVE-COTE 2), deep-learning baselines (DECNN, EEGNet, InceptionTime), a reproduction of the dataset paper's MAET transformer, and heterogeneous EEG + eye-tracking ensembles across four evaluation protocols
  * Identified a stimulus-duration confound: clip length alone classifies at 67.5% under LOSO against 14.3% chance, so cross-video protocols are required for any honest claim on this dataset
  * Reported validation-selected ensemble weights and a documented 8-point gap in the MAET reproduction rather than test-tuned figures
* **Brain Science and Neurotechnology Internship**, Aug 2026
  * Institute of Science and Technology for Brain-Inspired Intelligence (ISTBI), Fudan University
  * On-site, supervised by Prof. Shouyan Wang; performance rated Excellent
* 3D medical image segmentation — Light-UNETR architectures on left atrium datasets

Open-source contribution
======
* **[aeon](https://github.com/aeon-toolkit/aeon) — time-series machine learning toolkit**, [PR #3386](https://github.com/aeon-toolkit/aeon/pull/3386) merged June 2026
  * Refactored the HIVE-COTE V1 and V2 ensemble classifiers onto a shared `_BaseHIVECOTE` framework implementing CAWPE probability weighting, removing substantial duplication between two of the library's flagship classifiers
  * Kept scikit-learn compatibility by storing fitted components in `self._estimators`, added deprecation handling for `save_component_probas`, and guarded weight properties
  * Merged after several rounds of maintainer review with Prof. Tony Bagnall and Dr. Matthew Middlehurst

Awards
======
* Best Life Integration Award, Future Home Health Innovation Challenge Finals, Fudan University, Aug 2026

Skills
======
* Deep learning: PyTorch, scikit-learn, aeon, TensorFlow/Keras; CNN, transformer and GNN architectures, multimodal fusion, parameter-efficient fine-tuning (LoRA)
* Signal and data: EEG signal processing, time-series classification, feature engineering, exploratory data analysis
* Programming and systems: Python, Java, JavaScript, Linux, Git; MySQL, MongoDB
* Languages: Mandarin Chinese (native), English (fluent, IELTS 6.5)

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
* 博士，华威大学（University of Warwick），2026 年 10 月入学
<!-- 想显示具体专业/学院与导师的话，在这行补上 -->
* 人工智能 硕士，南安普顿大学（University of Southampton），2025 年 10 月 – 2026 年 12 月
  * 预计等级：Distinction

研究经历
======
* **硕士毕业设计——SEED-VII 多模态情感识别（`seedvii-aeon`）**，2025 年 9 月至今
  * 南安普顿大学，导师 Prof. Tony Bagnall
  * 在四种评估协议下横向比较 aeon 的经典时间序列分类器（MultiRocket、Hydra、Arsenal、DrCIF、HIVE-COTE 2）、深度学习基线（DECNN、EEGNet、InceptionTime）、对数据集原论文 MAET 模型的复现，以及 EEG 与眼动的异构集成
  * 发现刺激时长混淆：仅凭片段时长在 LOSO 下即可达到 67.5% 准确率（随机为 14.3%），因此该数据集上任何可信结论都必须建立在跨视频协议之上
  * 集成权重在验证集上选择而非测试集调优，MAET 复现与原文 8 个百分点的差距如实报告
* **脑科学与神经技术实习**，2026 年 8 月
  * 复旦大学类脑智能科学与技术研究院（ISTBI）
  * 线下实习，指导教师 王守岩 教授；考核评价 Excellent
* 三维医学图像分割——左心房数据集上的 Light-UNETR 架构

开源贡献
======
* **[aeon](https://github.com/aeon-toolkit/aeon) —— 时间序列机器学习工具库**，[PR #3386](https://github.com/aeon-toolkit/aeon/pull/3386)，2026 年 6 月合并
  * 将 HIVE-COTE V1 与 V2 集成分类器重构到共享的 `_BaseHIVECOTE` 框架上，实现 CAWPE 概率加权，消除了该库两个旗舰分类器之间的大量重复代码
  * 通过将拟合后的组件存入 `self._estimators` 保持 scikit-learn 兼容性，为 `save_component_probas` 添加弃用处理，并对权重属性做了保护
  * 经与 Prof. Tony Bagnall、Dr. Matthew Middlehurst 多轮维护者评审后合并

获奖
======
* Best Life Integration Award，未来家庭健康创新挑战赛决赛，复旦大学，2026 年 8 月

技能
======
* 深度学习：PyTorch、scikit-learn、aeon、TensorFlow/Keras；CNN、Transformer、GNN 架构，多模态融合，参数高效微调（LoRA）
* 信号与数据：EEG 信号处理、时间序列分类、特征工程、探索性数据分析
* 编程与系统：Python、Java、JavaScript、Linux、Git；MySQL、MongoDB
* 语言：中文（母语）、英语（流利，雅思 6.5）

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
