---
description: "Glit インサイト：書く技術、作家のための実践的なノウハウ、書き続けるための執筆環境や習慣まで。小説、Web小説、エッセイなどジャンルを問わず、作家と作家を目指すすべての人に向けた記事をお届けします。"
last_modified: 2026-11-05
layout: single
title: "Glit インサイト"
lang: ja
locale: "ja-JP"
toc: false
classes: insight-index
---

書く技術、作家のためのノウハウ、そして書き続けるための環境と習慣。小説、Web小説、エッセイなどジャンルや形式を問わず、書く人と、これから書きたいと願うすべての人に役立つインサイトをお届けします。

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "ja" | sort: "date" | reverse %}

<section class="insight-list" aria-label="インサイト記事一覧">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">続きを読む →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">最初のインサイトを準備中です。もうしばらくお待ちください。</p>
{% endif %}
</section>
