---
description: "Perspectivas de Glit: artículos sobre el oficio de escribir, consejos prácticos y hábitos que te ayudan a seguir escribiendo, para escritores y futuros escritores."
last_modified: 2026-11-05
layout: single
title: "Perspectivas de Glit"
lang: es
locale: "es-ES"
toc: false
classes: insight-index
---

Artículos sobre el oficio de escribir, consejos prácticos para escritores y el entorno y los hábitos que te ayudan a no dejarlo. Escribas novelas, historias por capítulos en internet o ensayos, están pensados para todos los escritores y para quienes sueñan con serlo.

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "es" | sort: "date" | reverse %}

<section class="insight-list" aria-label="Artículos">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">Leer más →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">La primera entrada está en camino. Vuelve pronto.</p>
{% endif %}
</section>
