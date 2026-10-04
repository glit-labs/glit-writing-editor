---
description: "영상과 글로 보는 Glit 가이드 모음입니다. 1분 데모, 모바일에서 만든 작품을 Dropbox로 데스크톱에서 이어 쓰는 방법, 샘플 웹소설 열기를 안내합니다."
last_modified: 2026-10-04
layout: single
title: "가이드"
lang: ko
locale: "ko-KR"
toc: false
classes: guide-index
---

Glit을 더 잘 활용하는 방법을 영상과 글로 안내합니다. 처음이라면 1분 데모부터 보세요.

{% assign guides = site.pages | where_exp: "p", "p.guide == true" | where: "lang", "ko" | sort: "order" %}
<nav class="guide-toc" aria-label="가이드 목록">
  <div class="guide-toc__group">
    <a class="guide-toc__head" href="#video-guides">영상 가이드 <span class="guide-toc__count">3</span></a>
    <ul class="guide-toc__list">
      <li><a href="#video-demo"><i class="fab fa-youtube" aria-hidden="true"></i><span class="guide-toc__label">1분 데모 · 글릿 에디터 사용 데모</span><span class="guide-toc__meta">1:05</span></a></li>
      <li><a href="#video-dropbox-mobile"><i class="fab fa-youtube" aria-hidden="true"></i><span class="guide-toc__label">01 · 모바일에서 작품 만들고 Dropbox에 올리기</span><span class="guide-toc__meta">2:32</span></a></li>
      <li><a href="#video-dropbox-desktop"><i class="fab fa-youtube" aria-hidden="true"></i><span class="guide-toc__label">02 · 데스크톱에서 내려받아 이어 쓰고 다시 올리기</span><span class="guide-toc__meta">2:09</span></a></li>
    </ul>
  </div>
  <div class="guide-toc__group">
    <a class="guide-toc__head" href="#text-guides">글 가이드 <span class="guide-toc__count">{{ guides.size }}</span></a>
    <ul class="guide-toc__list">
    {% for g in guides %}
      <li><a href="#text-guide-{{ forloop.index }}"><i class="fas fa-file-alt" aria-hidden="true"></i><span class="guide-toc__label">{{ g.title }}</span></a></li>
    {% endfor %}
    </ul>
  </div>
</nav>

## 영상 가이드 {#video-guides}

<div id="video-demo" class="video-row video-row--feature">
  <div class="video-row__text">
    <span class="video-row__eyebrow">1분 데모</span>
    <h3 class="video-row__title">글릿 에디터 사용 데모</h3>
    <p class="video-row__desc">웹소설 집필 앱 Glit의 화면 구성과 주요 기능을 1분 안에 살펴봅니다.</p>
    <a class="video-card__yt" href="https://www.youtube.com/watch?v=-9S1nZp2vyY" target="_blank" rel="noopener"><i class="fab fa-youtube" aria-hidden="true"></i>YouTube에서 보기 <span aria-hidden="true">↗</span></a>
  </div>
  <div class="video-row__media">
    {% include video-embed.html id="-9S1nZp2vyY" title="글릿 에디터(Glit Editor) 사용 데모" poster="/assets/images/guide/video-demo.jpg" duration="1:05" eager=true %}
  </div>
</div>

<h3 class="video-group__title">Dropbox로 모바일과 데스크톱에서 이어 쓰기</h3>
<p class="video-group__lead">두 영상은 같은 작품으로 이어집니다. 모바일에서 작품을 만들어 Dropbox에 올린 뒤, 데스크톱에서 내려받아 이어 쓰고 다시 올려 동기화합니다.</p>

<div class="video-steps">
  <div id="video-dropbox-mobile" class="video-row">
    <div class="video-row__text">
      <span class="video-row__step">01</span>
      <span class="video-row__eyebrow">모바일 · 숏츠</span>
      <h4 class="video-row__title">모바일에서 작품 만들고 Dropbox에 올리기</h4>
      <p class="video-row__desc">모바일 Glit에서 작품을 만들고, Dropbox를 연결해 업로드합니다.</p>
      <a class="video-card__yt" href="https://www.youtube.com/shorts/QYQ3OCz2n68" target="_blank" rel="noopener"><i class="fab fa-youtube" aria-hidden="true"></i>YouTube에서 보기 <span aria-hidden="true">↗</span></a>
    </div>
    <div class="video-row__media">
      {% include video-embed.html id="QYQ3OCz2n68" title="글릿 에디터 모바일에서 쓴 원고, Dropbox로 동기화하는 법" poster="/assets/images/guide/video-dropbox-mobile.jpg" duration="2:32" vertical=true %}
    </div>
  </div>
  <div id="video-dropbox-desktop" class="video-row">
    <div class="video-row__text">
      <span class="video-row__step">02</span>
      <span class="video-row__eyebrow">데스크톱</span>
      <h4 class="video-row__title">데스크톱에서 내려받아 이어 쓰고 다시 올리기</h4>
      <p class="video-row__desc">01에서 올린 작품을 데스크톱 Glit에서 내려받아 이어서 쓰고, 다시 업로드해 동기화합니다.</p>
      <a class="video-card__yt" href="https://www.youtube.com/watch?v=kj6NePyNbAs" target="_blank" rel="noopener"><i class="fab fa-youtube" aria-hidden="true"></i>YouTube에서 보기 <span aria-hidden="true">↗</span></a>
    </div>
    <div class="video-row__media">
      {% include video-embed.html id="kj6NePyNbAs" title="글릿 에디터 데스크톱에서 원고 내려받고 이어 쓰기 | Dropbox 동기화" poster="/assets/images/guide/video-dropbox-desktop.jpg" duration="2:09" %}
    </div>
  </div>
</div>

<p class="video-note">재생 버튼을 누르면 YouTube 플레이어를 불러옵니다. 그 전에는 YouTube로 어떤 정보도 전송되지 않습니다.</p>

<section class="guide-band" aria-labelledby="text-guides">
  <h2 class="guide-band__title" id="text-guides">글 가이드</h2>
  <p class="guide-band__lead">화면을 보며 한 단계씩 따라 할 수 있는 글 가이드입니다.</p>
  <div class="guide-list">
  {% for g in guides %}
    <a class="guide-card" id="text-guide-{{ forloop.index }}" href="{{ g.url | relative_url }}">
      <h3 class="guide-card__title">{{ g.title }}</h3>
      {% if g.summary %}<p class="guide-card__desc">{{ g.summary }}</p>{% endif %}
      <span class="guide-card__more">가이드 보기 →</span>
    </a>
  {% endfor %}
  </div>
</section>

<script>
  // Swap a poster for the YouTube player on click (see _includes/video-embed.html).
  // The player itself is left exactly as YouTube draws it: its title, channel
  // and branding overlays cannot be switched off by any embed parameter, and
  // the YouTube API Services Developer Policies forbid covering or blocking them.
  // The "전체 화면" pill shows only where element fullscreen works (not iPhone).
  if (document.fullscreenEnabled || document.webkitFullscreenEnabled) {
    document.documentElement.classList.add("has-fullscreen");
  }
  document.addEventListener("click", function (e) {
    var link = e.target.closest ? e.target.closest("a.video-embed[data-video-id]") : null;
    if (!link || e.button !== 0 || e.metaKey || e.ctrlKey || e.shiftKey || e.altKey) return;
    e.preventDefault();
    var wantsFullscreen = !!e.target.closest(".video-embed__fs");
    var frame = document.createElement("iframe");
    frame.src = "https://www.youtube-nocookie.com/embed/" + encodeURIComponent(link.getAttribute("data-video-id")) +
      "?autoplay=1&controls=0&rel=0&playsinline=1&iv_load_policy=3";
    frame.title = link.getAttribute("data-video-title");
    frame.allow = "accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share";
    frame.allowFullscreen = true;
    frame.referrerPolicy = "strict-origin-when-cross-origin";
    var box = document.createElement("div");
    box.className = link.className + " is-playing";
    box.appendChild(frame);
    link.replaceWith(box);
    frame.focus();
    // Still inside the click, so the browser accepts the fullscreen request.
    if (wantsFullscreen) {
      var request = frame.requestFullscreen || frame.webkitRequestFullscreen;
      if (request) {
        var result = request.call(frame);
        if (result && result.catch) result.catch(function () {});
      }
    }
  });
</script>
