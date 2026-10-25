---
description: "Glit のビスポーク・ポモドーロの使い方を案内します。Web小説執筆モードでモードを選び、集中時間と休憩時間を交互に繰り返して書く方法と、通知音・休憩サウンドの設定をまとめました。"
last_modified: 2026-10-26
layout: single
title: "ビスポーク・ポモドーロ ガイド — 集中と休憩を交互に書く"
lang: ja
locale: "ja-JP"
toc: false
guide: true
classes: guide-article
order: 3
summary: "Web小説執筆モード専用の集中タイマーです。モードを選んで集中時間と休憩時間を交互に繰り返し、残り1分の通知音と休憩サウンドを選ぶ方法を案内します。"
---

<header class="guide-hero">
  <p class="guide-back"><a href="/ja/guide.html">← ガイド一覧</a></p>
  <span class="guide-hero__eyebrow">テキストガイド</span>
  <h1 class="guide-hero__title">{{ page.title }}</h1>
  <p class="guide-hero__lead"><strong>ビスポーク・ポモドーロ</strong>は、Web小説執筆モード専用の集中タイマーです。集中時間は書くことだけに向き合い、休憩時間はエディタをロックしてしっかり休ませます。このガイドでは、モードの選び方から 2 つの開始方法、通知音と休憩サウンドの設定までを案内します。</p>
  <nav class="section-nav" aria-label="ガイド内リンク">
    <a href="#before-you-start">始める前に</a>
    <a href="#modes">モードを選ぶ</a>
    <a href="#custom-mode">自由設定</a>
    <a href="#top-bar">方法 1. 上部バー</a>
    <a href="#focus-writing">方法 2. 集中執筆</a>
    <a href="#focus-and-break">集中と休憩</a>
    <a href="#good-to-know">知っておくと便利</a>
  </nav>
</header>

## 始める前に {#before-you-start}

ビスポーク・ポモドーロは、次の条件で使えます。

<div class="info-grid">
  <div class="info-card">
    <h3>Mac 版 Glit 1.5.0 以降</h3>
    <p>Mac App Store で Glit を最新バージョンにアップデートしてください。</p>
  </div>
  <div class="info-card">
    <h3>Web小説執筆モード</h3>
    <p>Web小説執筆モードがオンのときだけ表示されます。サイドバーからすぐにオンにできます。</p>
  </div>
  <div class="info-card">
    <h3>エピソードファイルを開く</h3>
    <p>今日書くエピソードをエディタで開いておきましょう。</p>
  </div>
</div>

開始方法は 2 つあります。いつものエディタ画面のまま使うなら **方法 1（上部バー）**、目標文字数やハードモードと合わせて画面全体を原稿に集中させたいなら **方法 2（集中執筆）** を選んでください。2 つの方法は同じ設定値を共有します。

## モードを選ぶ {#modes}

設定画面の **［タイプと目的］** リストからモードを選ぶと、集中時間・休憩時間・サイクルがそのモードの値に切り替わります。

| タイプと目的 | 集中時間 | 休憩時間 | サイクル | 合計時間 |
| :-- | :-: | :-: | :-: | :-: |
| **スランプ突破モード** · Writer's Block を打ち破る | 15 分 | 3 分 | 6 回 | 105 分 |
| **デイリー連載マスターモード** · 最も安定した毎日のルーティン | 25 分 | 5 分 | 4 回 | 115 分 |
| **深層執筆没入モード** · 長く密度の高い叙述向け | 50 分 | 10 分 | 2 回 | 110 分 |

初めてなら **デイリー連載マスターモード** から始めてみてください。集中 25 分・休憩 5 分を 4 回繰り返す流れは、1 エピソードを書くのにちょうどよい長さです。好みの時間があるなら、下の[自由設定モード](#custom-mode)で自分で決められます。

## 自由設定モードで自分で決める {#custom-mode}

リストの 3 つのモードが自分のリズムに合わないときは、集中時間・休憩時間・サイクルを自分で決めましょう。**自由設定モード** はリストから選ぶ項目ではなく、値を変えると自動的に切り替わる名前です。

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">設定画面の <strong>［タイプと目的］</strong> で、希望のリズムにいちばん近いモードを選びます。<span class="walkthrough__hint">出発点にすぎないので、どのモードでもかまいません。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text"><strong>集中時間（分）</strong>・<strong>休憩時間（分）</strong>・<strong>サイクル（回）</strong> の欄に希望の数字を入力します。<span class="walkthrough__hint">入力できるのは数字だけです。集中時間は 1〜120 分、休憩時間は 1〜60 分、サイクルは 1〜12 回まで設定できます。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">3 つの値がリストのどのモードとも一致しなくなると、モード名の欄が <strong>自由設定モード</strong> に変わり、合計時間が新しい値で再計算されます。<span class="walkthrough__hint">3 つの値をいずれかのモードとまったく同じに戻すと、そのモード名に戻ります。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">合計時間を確認して <strong>［開始］</strong> をクリックします。</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>たとえば集中 40 分・休憩 8 分・サイクル 3 回にすると、<strong>合計 136分（2時間16分）</strong> と表示されます。最後のサイクルの後には休憩がないため、<code>集中時間 × サイクル + 休憩時間 × (サイクル − 1)</code> で計算します（40 × 3 + 8 × 2 = 136）。</p>

### 入力のルール

- 最大値より大きい数字を入れると、すぐに最大値に変わります。たとえば集中時間に 150 と入れると 120 になります。
- 欄を空にするか 0 を入れると、その欄から離れたときに最小値の 1 に変わります。
- 合計時間が 60 分未満のときは、「合計 55分」のように括弧なしで表示されます。
- 決めた値は保存され、次に設定画面を開いたときやアプリを再起動したときもそのまま残ります。上部バー版と集中執筆版は同じ値を共有します。

## 方法 1. エディタ上部バーから始める {#top-bar}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Web小説執筆モードでエピソードを開くと、エディタ上部バーの左側に <strong>［ビスポーク・ポモドーロ］</strong> ボタンが表示されます。ボタンをクリックします。</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method1-ja.png" alt="エディタ上部バー左側の［ビスポーク・ポモドーロ］ボタン" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">設定画面で <strong>［タイプと目的］</strong> を選び、必要に応じて集中時間・休憩時間・サイクルを変更します。</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text"><strong>残り1分の通知音</strong>（ウェストミンスター・オルゴール・チャイム・オフ）、<strong>休憩サウンド</strong>（オフ・水の音・鳥のさえずり）、<strong>音量</strong>を選びます。<span class="walkthrough__hint">▶ ボタンで試聴できます。通知音の初期値はウェストミンスター、休憩サウンドの初期値はオフです。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text"><strong>［開始］</strong> をクリックします。サイドバーが閉じ、ボタンが <strong>集中 1/4 · 24:59</strong> のような進行表示に変わります。</p>
    </div>
  </li>
</ol>

進行表示をクリックするとメニューが開きます。

- **リセット** — サイクルはそのままで、現在の段階（集中または休憩）のタイマーだけを最初に戻します。
- **簡易表示 / 全体表示** — 簡易表示は残り時間だけ、全体表示は「集中 1/4 · 2:46」のように段階とサイクルまで表示します。選んだ表示は次回も保持されます。
- **終了** — ビスポーク・ポモドーロを終了します。

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>実行中はサイドバーがロックされ、<strong>集中執筆</strong>は開始できません。ビスポーク・ポモドーロが終わると、サイドバーは開始前の状態に戻ります。Mac のフルスクリーンでは、タイトルバーとサイドバーも隠れて原稿だけが残ります。</p>

## 方法 2. 集中執筆と一緒に使う {#focus-writing}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">エディタ下部の <strong>［編集オプション］</strong> を開き、<strong>［集中執筆］</strong> をクリックします。</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method2-ja.png" alt="右下の［編集オプション］を開き［集中執筆］を選ぶ画面" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">設定画面で <strong>［ビスポーク・ポモドーロ］</strong> にチェックを入れます。<span class="walkthrough__hint">チェック項目は Web小説執筆モードのときだけ表示されます。チェックすると、モード・時間・通知音・休憩サウンドの設定と休憩のルールが展開されます。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">必要なら <strong>目標文字数</strong> と <strong>ハードモード</strong> も設定し、<strong>［開始］</strong> をクリックします。</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">進行表示は画面の右下に控えめに表示されます。進行表示をクリックすると <strong>［リセット］</strong> を選べます。</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i><strong>ハードモード</strong>もオンにしている場合、すべてのサイクルを終えても、目標文字数に達するまでは集中執筆を終了できません。</p>

## 集中時間と休憩時間 {#focus-and-break}

どちらの方法でも、同じ流れで進みます。

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text"><strong>集中時間</strong> — 今は書くことだけを考えましょう。残り時間が 1 分になると、画面の縁がテーマカラーでやわらかく 3 回光り、通知音が 1 回鳴ります。<span class="walkthrough__hint">光っている間も書き続けられます。文章をまとめる合図にしてください。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">集中時間が終わると <strong>「集中時間終了」</strong> のダイアログが表示されます。<strong>［確認］</strong> をクリックすると休憩が始まります。</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text"><strong>休憩時間</strong> — エディタの入力がロックされ、休憩の案内だけが表示されます。開いていたプレビューウィンドウは閉じ、補助サイドバーは休憩が終わるまで隠れます。休憩サウンドを選んでいれば、休憩中は繰り返し再生されます。<span class="walkthrough__hint">進行表示の横にあるスピーカーアイコンをクリックすると、休憩中でもサウンドの種類と音量を変えられます。</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">休憩が終わると <strong>「休憩終了」</strong> のダイアログが表示されます。<strong>［確認］</strong> をクリックすると次の集中時間が始まります。</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>最後のサイクルの集中時間が終わると、休憩なしで <strong>「ビスポーク・ポモドーロ完了」</strong> のダイアログが表示されます。<strong>［確認］</strong> をクリックすると終了し、画面は開始前の状態に戻ります。</p>

### 休憩を上手に過ごすには

設定画面にも表示される 2 つのルールです。

- 休憩中は、メッセージの確認や動画視聴など **注意残余** を残す行動を避けてください。次の集中時間の集中力が落ちます。
- 休憩中は、できれば **目を閉じて休むかストレッチ** をしてください。

## 知っておくと便利 {#good-to-know}

<div class="faq">
  <div class="faq__item">
    <p class="faq__q">設定値は保存されますか？</p>
    <p class="faq__a">はい。最後に使った集中時間・休憩時間・サイクルとサウンドの設定が保存され、次に開始するときやアプリを再起動したときもそのまま残ります。2 つの方法は同じ設定値を共有します。</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">アプリを終了して開き直すと、実行中のタイマーは続きますか？</p>
    <p class="faq__a">いいえ。実行中のセッションは復元されないため、もう一度開始してください。</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">ボタンが表示されません。</p>
    <p class="faq__a">Web小説執筆モードがオンになっていて、エピソードファイルが開いているか確認してください。実行中に Web小説執筆モードをオフにすると、ビスポーク・ポモドーロも一緒に終了します。</p>
  </div>
</div>

今回のアップデートのその他の変更点は [macOS v1.5.0 リリースノート](/releases/mac/v1.5.0/ja.html)でご覧いただけます。ほかにご不明な点はありますか？ [サポート](/ja/support.html)ページのよくある質問をご覧いただくか、いつでもメールでお問い合わせください。
