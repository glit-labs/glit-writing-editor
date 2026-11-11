---
description: "Glit Insights: articles on the craft of writing, practical know-how for writers, and the habits that help you keep writing — for writers and anyone who wants to be one."
last_modified: 2026-11-05
layout: single
title: "Glit Insights"
lang: en
toc: false
classes: insight-index
---

Articles on the craft of writing, practical know-how for writers, and the environment and habits that keep you writing. Whether you write novels, web serials or essays, they are written for every writer — and for everyone who hopes to become one.

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "en" | sort: "date" | reverse %}

<section class="insight-list" aria-label="Insight articles">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">Read more →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">The first insight is on its way. Check back soon.</p>
{% endif %}
</section>
