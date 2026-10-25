---
description: "Web小説執筆アプリ Glit のガイド集です。ビスポーク・ポモドーロで集中時間と休憩時間を交互に繰り返して書く方法を、手順を追って案内します。"
last_modified: 2026-10-26
layout: single
title: "ガイド"
lang: ja
locale: "ja-JP"
toc: false
classes: guide-index
---

Glit をもっと活用するためのガイドを、手順を追って案内します。

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "ja" | sort: "order" %}

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">テキストガイド</h2>
  <p class="guide-band__lead">画面を見ながら一歩ずつ進められるテキストガイドです。</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">ガイドを見る →</span>
    </a>
  {% endfor %}
  </div>
</section>
