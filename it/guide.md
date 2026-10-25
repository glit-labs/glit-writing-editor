---
description: "Guide passo passo di Glit, l'app di scrittura per autori di web novel. Scopri come scrivere alternando concentrazione e pausa con il Pomodoro su misura."
last_modified: 2026-10-26
layout: single
title: "Guide"
lang: it
locale: "it-IT"
toc: false
classes: guide-index
---

Guide passo passo per ottenere di più da Glit.

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "it" | sort: "order" %}

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">Guide scritte</h2>
  <p class="guide-band__lead">Guide scritte da seguire un passo alla volta.</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">Leggi la guida →</span>
    </a>
  {% endfor %}
  </div>
</section>
