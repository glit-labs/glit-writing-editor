---
description: "Guides pas à pas de Glit, l'app d'écriture pour les auteurs de romans web. Apprenez à écrire en alternant concentration et pause avec le Pomodoro sur mesure."
last_modified: 2026-10-26
layout: single
title: "Guides"
lang: fr
locale: "fr-FR"
toc: false
classes: guide-index
---

Des guides pas à pas pour tirer le meilleur parti de Glit.

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "fr" | sort: "order" %}

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">Guides écrits</h2>
  <p class="guide-band__lead">Des guides écrits à suivre étape par étape.</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">Lire le guide →</span>
    </a>
  {% endfor %}
  </div>
</section>
