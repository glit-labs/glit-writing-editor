---
description: "Step-by-step guides for Glit, the writing app for web novelists. Learn how to write in focus and break sessions with Bespoke Pomodoro."
last_modified: 2026-10-25
layout: single
title: "Guides"
lang: en
toc: false
classes: guide-index
---

Step-by-step guides to help you get more out of Glit.

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "en" | sort: "order" %}

Video guides are currently available in Korean only. You can watch them on the [Korean guide page](/ko/guide.html).

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">Text guides</h2>
  <p class="guide-band__lead">Written guides you can follow one step at a time.</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">Read the guide →</span>
    </a>
  {% endfor %}
  </div>
</section>
