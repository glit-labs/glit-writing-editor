---
description: "Guías paso a paso de Glit, la app de escritura para novelistas web. Aprende a escribir alternando concentración y descanso con el Pomodoro a medida."
last_modified: 2026-10-26
layout: single
title: "Guías"
lang: es
locale: "es-ES"
toc: false
classes: guide-index
---

Guías paso a paso para sacar más partido a Glit.

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "es" | sort: "order" %}

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">Guías escritas</h2>
  <p class="guide-band__lead">Guías escritas que puedes seguir paso a paso.</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">Ver la guía →</span>
    </a>
  {% endfor %}
  </div>
</section>
