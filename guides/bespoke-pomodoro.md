---
description: "How to use Bespoke Pomodoro in Glit: pick a mode in Web Novel Mode, alternate focus and break sessions, and set the 1-minute warning and break sound."
last_modified: 2026-10-26
layout: single
title: "Bespoke Pomodoro Guide — Alternate Focus and Breaks"
lang: en
toc: false
guide: true
classes: guide-article
order: 3
summary: "A focus timer built for Web Novel Mode. Pick a mode, write in alternating focus and break sessions, and choose a 1-minute warning and a break sound."
---

<header class="guide-hero">
  <p class="guide-back"><a href="/guide.html">← All guides</a></p>
  <span class="guide-hero__eyebrow">Text guide</span>
  <h1 class="guide-hero__title">{{ page.title }}</h1>
  <p class="guide-hero__lead"><strong>Bespoke Pomodoro</strong> is a focus timer made for Web Novel Mode. During focus time you only write; during breaks the editor locks so you actually rest. This guide walks through choosing a mode, the two ways to start, and setting the warning chime and break sound.</p>
  <nav class="section-nav" aria-label="Jump to a section">
    <a href="#before-you-start">Before you start</a>
    <a href="#modes">Choose a mode</a>
    <a href="#custom-mode">Custom mode</a>
    <a href="#top-bar">Option 1. Top bar</a>
    <a href="#focus-writing">Option 2. Focus Writing</a>
    <a href="#focus-and-break">Focus and breaks</a>
    <a href="#good-to-know">Good to know</a>
  </nav>
</header>

## Before you start {#before-you-start}

Bespoke Pomodoro is available when all of the following are true.

<div class="info-grid">
  <div class="info-card">
    <h3>Glit for Mac 1.5.0 or later</h3>
    <p>Update Glit to the latest version from the Mac App Store.</p>
  </div>
  <div class="info-card">
    <h3>Web Novel Mode</h3>
    <p>It appears only while Web Novel Mode is on. You can turn the mode on right from the sidebar.</p>
  </div>
  <div class="info-card">
    <h3>An episode file is open</h3>
    <p>Open the episode you plan to write today in the editor.</p>
  </div>
</div>

There are two ways to start. Choose **Option 1 (top bar)** to keep the regular editor view, or **Option 2 (Focus Writing)** to give the whole screen to your manuscript, together with a character target and Hard mode. Both options share the same settings.

## Choose a mode {#modes}

Pick a mode from the **Type & purpose** list on the settings screen, and the focus time, break time, and number of cycles change to that mode's values.

| Type & purpose | Focus | Break | Cycles | Total time |
| :-- | :-: | :-: | :-: | :-: |
| **Writer's Block Breaker** · Break through writer's block | 15 min | 3 min | 6 | 105 min |
| **Daily Serial Master** · The most stable daily routine | 25 min | 5 min | 4 | 115 min |
| **Deep Writing Immersion** · For long, dense passages | 50 min | 10 min | 2 | 110 min |

New to it? Start with **Daily Serial Master**: four rounds of 25 minutes of focus and 5 minutes of rest are about right for one episode. If you have your own timing in mind, set it yourself with [Custom mode](#custom-mode) below.

## Set your own timing with Custom mode {#custom-mode}

If none of the three modes fits your rhythm, set the focus time, break time, and cycles yourself. **Custom mode** is not an item you pick from the list; the name appears on its own once you change the values.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Under <strong>Type &amp; purpose</strong> on the settings screen, pick the mode closest to the rhythm you want. <span class="walkthrough__hint">It is only a starting point, so any mode will do.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Type the numbers you want into the <strong>Focus (min)</strong>, <strong>Break (min)</strong>, and <strong>Cycles</strong> fields. <span class="walkthrough__hint">Only digits are accepted. Focus can be 1–120 minutes, break 1–60 minutes, and cycles 1–12.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Once the three values no longer match any mode in the list, the mode name changes to <strong>Custom mode</strong> and the total time is recalculated for your values. <span class="walkthrough__hint">Set all three back to a mode's values and that mode's name returns.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Check the total time and click <strong>Start</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>For example, 40 minutes of focus, 8 minutes of break, and 3 cycles shows <strong>Total 136 min (2 h 16 min)</strong>. There is no break after the last cycle, so the total is <code>focus × cycles + break × (cycles − 1)</code> (40 × 3 + 8 × 2 = 136).</p>

### Input rules

- A number above the maximum changes to the maximum right away. For example, typing 150 for focus gives 120.
- If you leave a field empty or type 0, it changes to the minimum of 1 when you leave the field.
- When the total is under 60 minutes, it is shown without the hours, as in "Total 55 min".
- Your values are saved, so they are still there the next time you open the settings screen or relaunch the app. The top bar and Focus Writing versions share the same values.

## Option 1. Start from the editor's top bar {#top-bar}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">With an episode open in Web Novel Mode, the <strong>Bespoke Pomodoro</strong> button appears on the left of the editor's top bar. Click it.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method1-en.png" alt="The Bespoke Pomodoro button on the left of the editor's top bar" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">On the settings screen, choose a <strong>Type &amp; purpose</strong>, and adjust the focus time, break time, and cycles if you like.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Choose a <strong>1-minute warning</strong> (Westminster, Music box, Chime, or Off), a <strong>Break sound</strong> (Off, Water, or Birds), and the <strong>Volume</strong>. <span class="walkthrough__hint">Use the ▶ buttons to preview. The warning defaults to Westminster and the break sound to Off.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Click <strong>Start</strong>. The sidebar closes and the button turns into a progress display such as <strong>Focus 1/4 · 24:59</strong>.</p>
    </div>
  </li>
</ol>

Click the progress display to open its menu.

- **Reset** — keeps the current cycle and restarts only the timer of the current phase (focus or break).
- **Compact view / Full view** — Compact view shows only the time left; Full view also shows the phase and cycle, as in "Focus 1/4 · 2:46". Your choice is remembered.
- **Stop** — ends Bespoke Pomodoro.

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>While it runs, the sidebar is locked and <strong>Focus Writing</strong> cannot be started. When Bespoke Pomodoro ends, the sidebar returns to how it was before. In Mac full screen, the title bar and sidebar are hidden too, leaving only your manuscript.</p>

## Option 2. Use it with Focus Writing {#focus-writing}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Open <strong>Editor Options</strong> at the bottom of the editor and click <strong>Focus Writing</strong>.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method2-en.png" alt="Editor Options opened at the bottom right, with Focus Writing highlighted" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">On the settings screen, tick <strong>Bespoke Pomodoro</strong>. <span class="walkthrough__hint">The checkbox appears only in Web Novel Mode. Ticking it expands the mode, time, warning, and break sound settings, along with the break rules.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Set a <strong>Target characters</strong> count and <strong>Hard mode</strong> as well if you want, then click <strong>Start</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">The progress display sits quietly in the bottom-right corner. Click it to choose <strong>Reset</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>With <strong>Hard mode</strong> on, you cannot exit Focus Writing until you reach your character target, even after every cycle is finished.</p>

## Focus time and breaks {#focus-and-break}

Both options follow the same flow.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text"><strong>Focus time</strong> — think only about writing. When one minute is left, the edges of the screen glow softly in your theme color three times and the warning chime plays once. <span class="walkthrough__hint">You can keep writing while it glows. Use it to wrap up your sentence.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">When focus time ends, a <strong>"Focus time is over"</strong> dialog appears. The break starts only after you click <strong>OK</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text"><strong>Break time</strong> — the editor locks and only the break notice is shown. Any open preview windows close, and the secondary sidebar stays hidden until the break ends. If you chose a break sound, it loops for the length of the break. <span class="walkthrough__hint">Click the speaker icon next to the progress display to change the sound or volume during a break.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">When the break ends, a <strong>"Break is over"</strong> dialog appears. Click <strong>OK</strong> to start the next focus session.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>After the focus time of the last cycle, there is no break: a <strong>"Bespoke Pomodoro complete"</strong> dialog appears instead. Click <strong>OK</strong> to finish, and the screen returns to how it was before you started.</p>

### Making the most of your breaks

The settings screen shows these two rules as well.

- During breaks, avoid things that leave **attention residue**, like checking messages or watching videos. They weaken your focus in the next session.
- During breaks, **close your eyes and rest, or stretch**, if you can.

## Good to know {#good-to-know}

<div class="faq">
  <div class="faq__item">
    <p class="faq__q">Are my settings saved?</p>
    <p class="faq__a">Yes. Your last focus time, break time, cycles, and sound settings are saved, so they are still there the next time you start or relaunch the app. Both options share the same settings.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">If I quit and reopen the app, does a running timer carry on?</p>
    <p class="faq__a">No. A session in progress is not restored, so start a new one.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">I can't see the button.</p>
    <p class="faq__a">Check that Web Novel Mode is on and that an episode file is open. Turning Web Novel Mode off while a session is running also ends Bespoke Pomodoro.</p>
  </div>
</div>

See the [macOS v1.5.0 release notes](/releases/mac/v1.5.0/en.html) for everything else in this update. Have more questions? Browse the FAQ on the [Support](/support.html) page or email us any time.
