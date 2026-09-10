---
layout: archive
title: '<span class="i18n-en">Sitemap</span><span class="i18n-zh">站点地图</span>'
seo_title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

<span class="i18n-en">A list of all the pages found on the site. For you robots out there, there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.</span>
<span class="i18n-zh">本站所有页面的列表。给爬虫准备的还有一份 [XML 版本]({{ base_path }}/sitemap.xml)。</span>

<h2><span class="i18n-en">Pages</span><span class="i18n-zh">页面</span></h2>
{% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %}

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
{% unless collection.output == false or collection.label == "posts" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
  <h2>{{ label }}</h2>
  {% capture written_label %}{{ label }}{% endcapture %}
  {% endif %}
{% endunless %}
{% for post in collection.docs %}
  {% unless collection.output == false or collection.label == "posts" %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
{% endfor %}
