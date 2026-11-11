---
description: "网络小说写作应用 Glit 的使用指南合集。按步骤介绍定制番茄钟等功能的用法，教你如何交替安排专注时间与休息时间来写作，更顺手地用 Glit 写完每一章。"
last_modified: 2026-10-26
layout: single
title: "指南"
lang: zh
locale: "zh-CN"
toc: false
classes: guide-index
---

按步骤介绍如何更好地使用 Glit。

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "zh" | sort: "order" %}

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">图文指南</h2>
  <p class="guide-band__lead">可以一步一步跟着操作的图文指南。</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">查看指南 →</span>
    </a>
  {% endfor %}
  </div>
</section>
