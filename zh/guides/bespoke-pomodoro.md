---
description: "介绍 Glit 定制番茄钟的用法：在网络小说创作模式中选择模式，交替进行专注与休息，并设置剩余1分钟提示音和休息声音。"
last_modified: 2026-10-26
layout: single
title: "定制番茄钟指南：专注与休息交替写作"
lang: zh
locale: "zh-CN"
toc: false
guide: true
classes: guide-article
order: 3
summary: "专为网络小说创作模式打造的专注计时器。选择模式，交替进行专注时间和休息时间，并选择剩余1分钟提示音与休息声音。"
---

<header class="guide-hero">
  <p class="guide-back"><a href="/zh/guide.html">← 全部指南</a></p>
  <span class="guide-hero__eyebrow">图文指南</span>
  <h1 class="guide-hero__title">{{ page.title }}</h1>
  <p class="guide-hero__lead"><strong>定制番茄钟</strong>是专为网络小说创作模式打造的专注计时器。专注时间只管写作；休息时间会锁定编辑器，让你真正休息。本指南将介绍如何选择模式、两种开始方式，以及如何设置提示音和休息声音。</p>
  <nav class="section-nav" aria-label="跳转到章节">
    <a href="#before-you-start">开始之前</a>
    <a href="#modes">选择模式</a>
    <a href="#custom-mode">自定义模式</a>
    <a href="#top-bar">方法 1. 顶部栏</a>
    <a href="#focus-writing">方法 2. 专注写作</a>
    <a href="#focus-and-break">专注与休息</a>
    <a href="#good-to-know">小贴士</a>
  </nav>
</header>

## 开始之前 {#before-you-start}

满足以下条件即可使用定制番茄钟。

<div class="info-grid">
  <div class="info-card">
    <h3>Mac 版 Glit 1.5.0 或更高版本</h3>
    <p>请在 Mac App Store 中将 Glit 更新到最新版本。</p>
  </div>
  <div class="info-card">
    <h3>网络小说创作模式</h3>
    <p>仅在开启网络小说创作模式时显示。可直接在侧边栏中开启该模式。</p>
  </div>
  <div class="info-card">
    <h3>打开章节文件</h3>
    <p>请先在编辑器中打开今天要写的章节。</p>
  </div>
</div>

开始方式有两种。想保留平常的编辑器界面，请选择**方法 1（顶部栏）**；想让整个屏幕只留给稿件，并配合目标字数和硬核模式使用，请选择**方法 2（专注写作）**。两种方法共用同一套设置。

## 选择模式 {#modes}

在设置界面的**类型与目的**列表中选择一个模式，专注时间、休息时间和循环次数就会切换为该模式的数值。

| 类型与目的 | 专注时间 | 休息时间 | 循环 | 总时长 |
| :-- | :-: | :-: | :-: | :-: |
| **打破写作瓶颈模式** · 突破 Writer's Block | 15 分钟 | 3 分钟 | 6 次 | 105 分钟 |
| **每日连载大师模式** · 最稳定的日常节奏 | 25 分钟 | 5 分钟 | 4 次 | 115 分钟 |
| **深度写作沉浸模式** · 适合长篇高密度叙述 | 50 分钟 | 10 分钟 | 2 次 | 110 分钟 |

第一次使用？建议从**每日连载大师模式**开始：专注 25 分钟、休息 5 分钟，重复四次，正适合写完一章。如果心里有自己的时间安排，可以用下方的[自定义模式](#custom-mode)自行设定。

## 用自定义模式自行设定 {#custom-mode}

如果列表中的三个模式都不适合你的节奏，可以自行设定专注时间、休息时间和循环次数。**自定义模式**不是在列表中选择的项目，而是修改数值后自动显示的名称。

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">在设置界面的<strong>类型与目的</strong>中，选择与理想节奏最接近的模式。<span class="walkthrough__hint">这只是起点，选哪个模式都可以。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">在<strong>专注时间（分钟）</strong>、<strong>休息时间（分钟）</strong>和<strong>循环（次）</strong>栏中输入想要的数字。<span class="walkthrough__hint">只能输入数字。专注时间可设为 1–120 分钟，休息时间 1–60 分钟，循环 1–12 次。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">三个数值与列表中任何模式都不一致时，模式名称会变为<strong>自定义模式</strong>，总时长也会按新数值重新计算。<span class="walkthrough__hint">把三个数值改回与某个模式完全相同，就会恢复该模式的名称。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">确认总时长后，点击<strong>「开始」</strong>。</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>例如设为专注 40 分钟、休息 8 分钟、循环 3 次，会显示<strong>总时长 136 分钟（2 小时 16 分钟）</strong>。最后一个循环之后没有休息，因此按 <code>专注时间 × 循环 + 休息时间 × (循环 − 1)</code> 计算（40 × 3 + 8 × 2 = 136）。</p>

### 输入规则

- 输入超过上限的数字时，会立即变为上限值。例如专注时间输入 150，会变为 120。
- 栏位留空或输入 0 时，离开该栏位后会变为下限值 1。
- 总时长不足 60 分钟时，会像“总时长 55 分钟”这样不带括号显示。
- 设定的数值会被保存，下次打开设置界面或重新启动应用后依然保留。顶部栏版本和专注写作版本共用同一套数值。

## 方法 1. 从编辑器顶部栏开始 {#top-bar}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">在网络小说创作模式中打开章节后，编辑器顶部栏左侧会出现<strong>「定制番茄钟」</strong>按钮。点击该按钮。</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method1-zh.png" alt="编辑器顶部栏左侧的「定制番茄钟」按钮" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">在设置界面中选择<strong>类型与目的</strong>，需要时再调整专注时间、休息时间和循环次数。</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">选择<strong>剩余1分钟提示音</strong>（威斯敏斯特、八音盒、铃声或关闭）、<strong>休息声音</strong>（关闭、流水声或鸟鸣）以及<strong>音量</strong>。<span class="walkthrough__hint">可通过 ▶ 按钮试听。提示音默认为威斯敏斯特，休息声音默认为关闭。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">点击<strong>「开始」</strong>。侧边栏会关闭，按钮变为<strong>专注 1/4 · 24:59</strong>这样的进度显示。</p>
    </div>
  </li>
</ol>

点击进度显示会打开菜单。

- **重置** — 保持当前循环不变，只将当前阶段（专注或休息）的计时器恢复到开头。
- **简洁显示 / 完整显示** — 简洁显示只显示剩余时间；完整显示还会显示阶段和循环，例如“专注 1/4 · 2:46”。所选方式下次仍会保留。
- **结束** — 结束定制番茄钟。

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>进行期间侧边栏会被锁定，也无法开始<strong>专注写作</strong>。定制番茄钟结束后，侧边栏会恢复到开始前的状态。在 Mac 全屏模式下，标题栏和侧边栏也会隐藏，只留下稿件。</p>

## 方法 2. 与专注写作一起使用 {#focus-writing}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">打开编辑器下方的<strong>「编辑器选项」</strong>，点击<strong>「专注写作」</strong>。</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method2-zh.png" alt="打开右下角的「编辑器选项」并选择「专注写作」的界面" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">在设置界面中勾选<strong>「定制番茄钟」</strong>。<span class="walkthrough__hint">该选项仅在网络小说创作模式下显示。勾选后会展开模式、时间、提示音和休息声音的设置，以及休息规则说明。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">需要时同时设置<strong>目标字数</strong>和<strong>硬核模式</strong>，然后点击<strong>「开始」</strong>。</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">进度显示会安静地出现在屏幕右下角。点击进度显示即可选择<strong>「重置」</strong>。</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>如果同时开启了<strong>硬核模式</strong>，即使完成了所有循环，在达到目标字数之前也无法结束专注写作。</p>

## 专注时间与休息时间 {#focus-and-break}

两种方法的流程相同。

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text"><strong>专注时间</strong> — 此刻只想着写作。剩余 1 分钟时，屏幕边缘会以主题色柔和地闪亮三次，并响起一次提示音。<span class="walkthrough__hint">闪亮期间仍可继续写作。把它当作收尾的信号吧。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">专注时间结束后会弹出<strong>“专注时间结束”</strong>提示框。点击<strong>「确定」</strong>后才会开始休息。</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text"><strong>休息时间</strong> — 编辑器会锁定输入，只显示休息提示。已打开的预览窗口会关闭，辅助侧边栏在休息结束前会隐藏。如果选择了休息声音，休息期间会循环播放。<span class="walkthrough__hint">点击进度显示旁的扬声器图标，休息期间也能更改声音和音量。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">休息结束后会弹出<strong>“休息结束”</strong>提示框。点击<strong>「确定」</strong>即可开始下一段专注时间。</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>最后一个循环的专注时间结束后不再休息，而是弹出<strong>“定制番茄钟已完成”</strong>提示框。点击<strong>「确定」</strong>即可结束，屏幕会恢复到开始前的状态。</p>

### 如何好好休息

设置界面中也会显示以下两条规则。

- 休息时请避免查看消息、观看视频等会留下**注意力残留**的行为，否则会降低下一段专注时间的专注力。
- 休息时尽量**闭眼休息或做伸展运动**。

## 小贴士 {#good-to-know}

<div class="faq">
  <div class="faq__item">
    <p class="faq__q">设置会被保存吗？</p>
    <p class="faq__a">会。最后使用的专注时间、休息时间、循环次数和声音设置都会保存，下次开始或重新启动应用后依然保留。两种方法共用同一套设置。</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">退出并重新打开应用后，进行中的计时会继续吗？</p>
    <p class="faq__a">不会。进行中的会话不会恢复，请重新开始。</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">看不到按钮怎么办？</p>
    <p class="faq__a">请确认已开启网络小说创作模式并打开了章节文件。进行中关闭网络小说创作模式，定制番茄钟也会随之结束。</p>
  </div>
</div>

本次更新的其他变更请参阅 [macOS v1.5.0 发布说明](/releases/mac/v1.5.0/zh.html)。还有其他问题？欢迎查看[支持](/zh/support.html)页面的常见问题，或随时发送邮件联系我们。
