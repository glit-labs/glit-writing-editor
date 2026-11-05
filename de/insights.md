---
description: "Glit Einblicke: Beiträge über das Handwerk des Schreibens, Praxiswissen für Autorinnen und Autoren sowie Umgebung und Gewohnheiten, die beim Dranbleiben helfen – für alle, die schreiben oder schreiben möchten."
last_modified: 2026-11-05
layout: single
title: "Glit Einblicke"
lang: de
locale: "de-DE"
toc: false
classes: insight-index
---

Beiträge über das Handwerk des Schreibens, Praxiswissen für Autorinnen und Autoren und die Umgebung und Gewohnheiten, mit denen du dranbleibst. Ob Roman, Fortsetzungsgeschichte im Netz oder Essay: Sie richten sich an alle, die schreiben – und an alle, die Autorin oder Autor werden möchten.

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "de" | sort: "date" | reverse %}

<section class="insight-list" aria-label="Beiträge">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">Weiterlesen →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">Der erste Beitrag ist in Arbeit. Schau bald wieder vorbei.</p>
{% endif %}
</section>
