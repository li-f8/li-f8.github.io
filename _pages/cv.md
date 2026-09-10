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
* EEG algorithm optimisation — parameter-efficient tuning (LoRA-One and related methods) for neural signal models
* Semantic and emotion decoding from EEG, including visualisation of the decoded representations
* Time-series classification — analysis of the fitting mechanisms of HIVE-COTE ensembles
* 3D medical image segmentation — Light-UNETR architectures on left atrium datasets
<!-- Add dates, institutions and supervisors as they apply, e.g.:
* 2024–2025: Research Assistant, <Lab>, <University>. Supervisor: <Name>
-->

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
* EEG 算法优化——面向神经信号模型的参数高效微调（LoRA-One 及相关方法）
* 脑电语义与情感解码，以及解码表征的可视化
* 时间序列分类——HIVE-COTE 集成模型拟合机制分析
* 三维医学图像分割——左心房数据集上的 Light-UNETR 架构

<!-- 可按需补充时间、单位与导师，例如：
* 2024–2025：研究助理，<实验室>，<学校>。导师：<姓名>
-->

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
