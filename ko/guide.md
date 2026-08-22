---
description: "Glit을 더 잘 활용하는 방법을 담은 한국어 가이드 모음입니다. 샘플 웹소설 열기부터 차근차근 따라 할 수 있는 안내를 제공합니다."
last_modified: 2026-08-23
layout: single
title: "가이드"
lang: ko
locale: "ko-KR"
toc: false
---

Glit을 더 잘 활용하는 방법을 안내하는 가이드 모음입니다. 원하는 가이드를 선택해 시작하세요.

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "ko" | sort: "order" %}
<div class="guide-list">
{% for g in guides %}
  <a class="guide-card" href="{{ g.url | relative_url }}">
    <h3 class="guide-card__title">{{ g.title }}</h3>
    {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
    <span class="guide-card__more">가이드 보기 →</span>
  </a>
{% endfor %}
</div>
