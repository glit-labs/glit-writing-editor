---
description: "Glit 洞察：关于写作技巧、写作方法，以及帮助你坚持写作的环境与习惯的文章，献给每一位作者和想成为作者的人。"
last_modified: 2026-11-05
layout: single
title: "Glit 洞察"
lang: zh
locale: "zh-CN"
toc: false
classes: insight-index
---

关于写作技巧、写作方法，以及让你坚持写下去的环境与习惯的文章。无论你写的是小说、网络小说还是随笔，这些内容都献给每一位写作者，以及每一个想成为作者的人。

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "zh" | sort: "date" | reverse %}

<section class="insight-list" aria-label="文章列表">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">阅读全文 →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">第一篇洞察正在准备中，敬请期待。</p>
{% endif %}
</section>
