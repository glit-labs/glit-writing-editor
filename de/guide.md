---
description: "Schritt-für-Schritt-Anleitungen für Glit, die Schreib-App für Webroman-Autoren. So schreibst du mit dem Bespoke-Pomodoro im Wechsel aus Fokus und Pause."
last_modified: 2026-10-26
layout: single
title: "Anleitungen"
lang: de
locale: "de-DE"
toc: false
classes: guide-index
---

Schritt-für-Schritt-Anleitungen, mit denen du mehr aus Glit herausholst.

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "de" | sort: "order" %}

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">Text-Anleitungen</h2>
  <p class="guide-band__lead">Schriftliche Anleitungen, denen du Schritt für Schritt folgen kannst.</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">Anleitung lesen →</span>
    </a>
  {% endfor %}
  </div>
</section>
