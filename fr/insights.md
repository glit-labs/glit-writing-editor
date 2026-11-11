---
description: "Perspectives Glit : l'art d'écrire, des conseils pratiques et les habitudes pour écrire régulièrement, pour les auteurs de webnovels et de romans en ligne."
last_modified: 2026-11-05
layout: single
title: "Perspectives Glit"
lang: fr
locale: "fr-FR"
toc: false
classes: insight-index
---

Des articles sur l'art d'écrire, des conseils pratiques pour les auteurs, l'environnement et les habitudes qui permettent d'écrire avec régularité. Que vous écriviez des romans, des fictions publiées en ligne chapitre par chapitre ou des essais, ils s'adressent à tous les auteurs et à celles et ceux qui rêvent de le devenir.

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "fr" | sort: "date" | reverse %}

<section class="insight-list" aria-label="Articles">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">Lire la suite →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">Le premier article arrive bientôt. Revenez nous voir.</p>
{% endif %}
</section>
