---
description: "Approfondimenti Glit: articoli sul mestiere della scrittura, consigli pratici e abitudini che aiutano a scrivere con costanza, per chi scrive e per chi sogna di farlo."
last_modified: 2026-11-05
layout: single
title: "Approfondimenti Glit"
lang: it
locale: "it-IT"
toc: false
classes: insight-index
---

Articoli sul mestiere della scrittura, consigli pratici per chi scrive, l'ambiente e le abitudini che aiutano a non mollare. Che tu scriva romanzi, storie a puntate online o saggi, sono pensati per tutti gli scrittori e per chi sogna di diventarlo.

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "it" | sort: "date" | reverse %}

<section class="insight-list" aria-label="Articoli">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">Leggi di più →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">Il primo approfondimento è in arrivo. Torna a trovarci presto.</p>
{% endif %}
</section>
