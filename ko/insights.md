---
description: "글릿 인사이트: 글쓰기의 기술, 작가를 위한 노하우, 집필 환경과 습관까지. 작가와 작가를 꿈꾸는 모든 사람을 위한 글을 전합니다."
last_modified: 2026-11-05
layout: single
title: "글릿 인사이트"
lang: ko
locale: "ko-KR"
toc: false
classes: insight-index
---

글쓰기의 기술, 작가를 위한 노하우, 그리고 꾸준히 쓰게 해 주는 환경과 습관까지. 소설, 웹소설, 에세이 등 장르와 형식에 상관없이 작가와 작가를 꿈꾸는 모든 분께 도움이 될 인사이트를 전합니다.

{% comment %}
  Insight articles are pages with `insight: true` and this page's `lang`,
  newest first by `date`. Put them at /insights/<slug>.md (English) or
  /<lang>/insights/<slug>.md with a `summary` for the card.
{% endcomment %}
{% assign insights = site.pages | where_exp: "p", "p.insight == true" | where: "lang", "ko" | sort: "date" | reverse %}

<section class="insight-list" aria-label="인사이트 글 목록">
{% if insights.size > 0 %}
  <div class="guide-list">
  {% for p in insights %}
    <a class="guide-card" href="{{ p.url | relative_url }}">
      {% if p.date %}<time class="insight-card__date" datetime="{{ p.date | date: '%Y-%m-%d' }}">{{ p.date | date: '%Y-%m-%d' }}</time>{% endif %}
      <h3 class="guide-card__title">{{ p.title }}</h3>
      {% if p.summary %}<p class="guide-card__desc">{{ p.summary }}</p>{% endif %}
      <span class="guide-card__more">자세히 보기 →</span>
    </a>
  {% endfor %}
  </div>
{% else %}
  <p class="insight-empty">첫 인사이트를 준비하고 있습니다. 곧 찾아올게요.</p>
{% endif %}
</section>
