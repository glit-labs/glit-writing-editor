---
description: "Utiliser le Pomodoro sur mesure de Glit : choisir un mode en roman-feuilleton, alterner concentration et pause, régler le signal 1 minute avant et le son de pause."
last_modified: 2026-10-26
layout: single
title: "Guide du Pomodoro sur mesure — alterner concentration et pause"
lang: fr
locale: "fr-FR"
toc: false
guide: true
classes: guide-article
order: 3
summary: "Un minuteur de concentration conçu pour le mode roman-feuilleton. Choisissez un mode, alternez temps de concentration et temps de pause, et sélectionnez un signal 1 minute avant et un son de pause."
---

<header class="guide-hero">
  <p class="guide-back"><a href="/fr/guide.html">← Tous les guides</a></p>
  <span class="guide-hero__eyebrow">Guide écrit</span>
  <h1 class="guide-hero__title">{{ page.title }}</h1>
  <p class="guide-hero__lead">Le <strong>Pomodoro sur mesure</strong> est un minuteur de concentration pensé pour le mode roman-feuilleton. Pendant la concentration, vous ne faites qu'écrire ; pendant la pause, l'éditeur se verrouille pour que vous vous reposiez vraiment. Ce guide présente le choix du mode, les deux façons de démarrer et le réglage du signal et du son de pause.</p>
  <nav class="section-nav" aria-label="Aller à une section">
    <a href="#before-you-start">Avant de commencer</a>
    <a href="#modes">Choisir un mode</a>
    <a href="#custom-mode">Mode personnalisé</a>
    <a href="#top-bar">Option 1. Barre supérieure</a>
    <a href="#focus-writing">Option 2. Écriture concentrée</a>
    <a href="#focus-and-break">Concentration et pause</a>
    <a href="#good-to-know">Bon à savoir</a>
    <a href="#get-glit">Obtenir Glit</a>
  </nav>
</header>

## Avant de commencer {#before-you-start}

Le Pomodoro sur mesure est disponible dans les conditions suivantes.

<div class="info-grid">
  <div class="info-card">
    <h3>Mode roman-feuilleton</h3>
    <p>Il n'apparaît que lorsque le mode roman-feuilleton est activé. Vous pouvez l'activer directement depuis la barre latérale.</p>
  </div>
  <div class="info-card">
    <h3>Un épisode ouvert</h3>
    <p>Ouvrez dans l'éditeur l'épisode que vous comptez écrire aujourd'hui.</p>
  </div>
</div>

Il existe deux façons de démarrer. Choisissez l'**option 1 (barre supérieure)** pour garder la vue habituelle de l'éditeur, ou l'**option 2 (Écriture concentrée)** pour consacrer tout l'écran à votre manuscrit, avec un objectif de caractères et le mode difficile. Les deux options partagent les mêmes réglages.

## Choisir un mode {#modes}

Choisissez un mode dans la liste **Type et objectif** de l'écran de réglages : le temps de concentration, le temps de pause et le nombre de cycles prennent les valeurs de ce mode.

| Type et objectif | Concentration | Pause | Cycles | Durée totale |
| :-- | :-: | :-: | :-: | :-: |
| **Anti-blocage** · Briser le Writer's Block | 15 min | 3 min | 6 | 105 min |
| **Maître du feuilleton quotidien** · La routine quotidienne la plus stable | 25 min | 5 min | 4 | 115 min |
| **Immersion profonde** · Pour les passages longs et denses | 50 min | 10 min | 2 | 110 min |

Première fois ? Commencez par **Anti-blocage** : six tours de 15 minutes de concentration et 3 minutes de pause. Si vous avez d'autres durées en tête, réglez-les vous-même avec le [Mode personnalisé](#custom-mode).

## Régler vos propres durées avec le Mode personnalisé {#custom-mode}

Si aucun des trois modes ne correspond à votre rythme, réglez vous-même la concentration, la pause et les cycles. Le **Mode personnalisé** n'est pas un choix de la liste : ce nom apparaît de lui-même dès que vous modifiez les valeurs.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Dans <strong>Type et objectif</strong>, sur l'écran de réglages, choisissez le mode le plus proche du rythme voulu. <span class="walkthrough__hint">Ce n'est qu'un point de départ : n'importe quel mode convient.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Saisissez les nombres voulus dans les champs <strong>Concentration (min)</strong>, <strong>Pause (min)</strong> et <strong>Cycles</strong>. <span class="walkthrough__hint">Seuls les chiffres sont acceptés. La concentration va de 1 à 120 minutes, la pause de 1 à 60 minutes et les cycles de 1 à 12.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Dès que les trois valeurs ne correspondent plus à aucun mode de la liste, le nom devient <strong>Mode personnalisé</strong> et la durée totale est recalculée avec vos valeurs. <span class="walkthrough__hint">Remettez les trois valeurs d'un mode et son nom revient.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Vérifiez la durée totale et cliquez sur <strong>Commencer</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Par exemple, 40 minutes de concentration, 8 minutes de pause et 3 cycles affichent <strong>Total 136 min (2 h 16 min)</strong>. Il n'y a pas de pause après le dernier cycle, d'où <code>concentration × cycles + pause × (cycles − 1)</code> (40 × 3 + 8 × 2 = 136).</p>

### Règles de saisie

- Un nombre supérieur au maximum est aussitôt ramené au maximum. Par exemple, 150 en concentration devient 120.
- Si vous laissez un champ vide ou saisissez 0, il passe au minimum de 1 quand vous quittez le champ.
- Quand le total est inférieur à 60 minutes, il s'affiche sans les heures, comme « Total 55 min ».
- Vos valeurs sont enregistrées : vous les retrouvez à la prochaine ouverture de l'écran de réglages ou après avoir relancé l'app. La version barre supérieure et la version Écriture concentrée partagent les mêmes valeurs.

## Option 1. Démarrer depuis la barre supérieure de l'éditeur {#top-bar}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Lorsqu'un épisode est ouvert en mode roman-feuilleton, le bouton <strong>Pomodoro sur mesure</strong> apparaît à gauche de la barre supérieure de l'éditeur. Cliquez dessus.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method1-fr.png" alt="Le bouton Pomodoro sur mesure à gauche de la barre supérieure de l'éditeur" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Dans l'écran de réglages, choisissez un <strong>Type et objectif</strong>, puis ajustez si besoin la concentration, la pause et les cycles.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Choisissez le <strong>Signal 1 min avant</strong> (Westminster, Boîte à musique, Carillon ou Désactivé), le <strong>Son de pause</strong> (Désactivé, Eau ou Oiseaux) et le <strong>Volume</strong>. <span class="walkthrough__hint">Les boutons ▶ permettent d'écouter un aperçu. Par défaut, le signal est Westminster et le son de pause est désactivé.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Cliquez sur <strong>Commencer</strong>. La barre latérale se ferme et le bouton affiche la progression, par exemple <strong>Concentration 1/4 · 24:59</strong>.</p>
    </div>
  </li>
</ol>

Cliquez sur l'indicateur de progression pour ouvrir son menu.

- **Réinitialiser** — garde le cycle en cours et ne remet à zéro que le minuteur de la phase actuelle (concentration ou pause).
- **Vue compacte / Vue complète** — la vue compacte n'affiche que le temps restant ; la vue complète ajoute la phase et le cycle, comme « Concentration 1/4 · 2:46 ». Votre choix est mémorisé.
- **Terminer** — arrête le Pomodoro sur mesure.

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Pendant son déroulement, la barre latérale est verrouillée et l'<strong>Écriture concentrée</strong> ne peut pas être lancée. À la fin, la barre latérale retrouve son état d'avant. En plein écran sur Mac, la barre de titre et la barre latérale sont aussi masquées pour ne laisser que votre manuscrit.</p>

## Option 2. L'utiliser avec l'Écriture concentrée {#focus-writing}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Ouvrez <strong>Options de l'éditeur</strong> en bas de l'éditeur, puis cliquez sur <strong>Écriture concentrée</strong>.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method2-fr.png" alt="Options de l'éditeur ouvertes en bas à droite, Écriture concentrée mise en évidence" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Dans l'écran de réglages, cochez <strong>Pomodoro sur mesure</strong>. <span class="walkthrough__hint">La case n'apparaît qu'en mode roman-feuilleton. Une fois cochée, elle déploie les réglages de mode, de durées, de signal et de son de pause, ainsi que les règles de pause.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Définissez aussi, si vous le souhaitez, les <strong>Caractères visés</strong> et le <strong>Mode difficile</strong>, puis cliquez sur <strong>Commencer</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">L'indicateur de progression s'affiche discrètement en bas à droite. Cliquez dessus pour choisir <strong>Réinitialiser</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Avec le <strong>Mode difficile</strong> activé, vous ne pouvez pas quitter l'Écriture concentrée avant d'avoir atteint votre objectif de caractères, même une fois tous les cycles terminés.</p>

## Concentration et pause {#focus-and-break}

Les deux options suivent le même déroulement.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text"><strong>Concentration</strong> — ne pensez qu'à écrire. Quand il reste une minute, les bords de l'écran s'illuminent doucement trois fois de la couleur du thème et le signal retentit une fois. <span class="walkthrough__hint">Vous pouvez continuer à écrire pendant ce temps. Profitez-en pour terminer votre phrase.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">À la fin de la concentration, la fenêtre <strong>« Fin de la concentration »</strong> s'affiche. La pause ne commence qu'après un clic sur <strong>OK</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text"><strong>Pause</strong> — l'éditeur se verrouille et seul le message de pause s'affiche. Les fenêtres d'aperçu ouvertes se ferment et la barre latérale secondaire reste masquée jusqu'à la fin de la pause. Si vous avez choisi un son de pause, il tourne en boucle pendant toute la pause. <span class="walkthrough__hint">Cliquez sur l'icône du haut-parleur à côté de l'indicateur de progression pour changer le son ou le volume pendant la pause.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">À la fin de la pause, la fenêtre <strong>« Fin de la pause »</strong> s'affiche. Cliquez sur <strong>OK</strong> pour lancer la concentration suivante.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Après la concentration du dernier cycle, il n'y a pas de pause : la fenêtre <strong>« Pomodoro sur mesure terminé »</strong> s'affiche. Cliquez sur <strong>OK</strong> pour terminer ; l'écran retrouve son état d'avant le démarrage.</p>

### Bien profiter de ses pauses

L'écran de réglages rappelle aussi ces deux règles.

- Pendant les pauses, évitez ce qui laisse un **résidu d'attention**, comme consulter vos messages ou regarder des vidéos. Cela réduit votre concentration à la séance suivante.
- Pendant les pauses, **fermez les yeux pour vous reposer ou étirez-vous** si possible.

## Bon à savoir {#good-to-know}

<div class="faq">
  <div class="faq__item">
    <p class="faq__q">Mes réglages sont-ils enregistrés ?</p>
    <p class="faq__a">Oui. Les dernières durées de concentration et de pause, le nombre de cycles et les réglages de son sont enregistrés : vous les retrouvez au prochain démarrage ou après avoir relancé l'app. Les deux options partagent les mêmes réglages.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">Si je quitte puis rouvre l'app, le minuteur en cours continue-t-il ?</p>
    <p class="faq__a">Non. Une séance en cours n'est pas restaurée ; lancez-en une nouvelle.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">Je ne vois pas le bouton.</p>
    <p class="faq__a">Vérifiez que le mode roman-feuilleton est activé et qu'un épisode est ouvert. Désactiver le mode roman-feuilleton pendant une séance met aussi fin au Pomodoro sur mesure.</p>
  </div>
</div>

## Obtenir Glit {#get-glit}

Glit est disponible dans les boutiques ci-dessous.

<div class="store-grid">
  <div class="store-card">
    <span class="store-card__badge store-card__badge--included">Pomodoro inclus</span>
    <div class="store-card__icon"><i class="fab fa-app-store" aria-hidden="true"></i></div>
    <h3 class="store-card__name">Mac App Store</h3>
    <p class="store-card__platform">macOS</p>
    <p class="store-card__price">$4.99</p>
    <a class="store-card__btn" href="https://apps.apple.com/us/app/glit-web-novel-writing-editor/id6764386721">Acheter</a>
  </div>

  <div class="store-card">
    <span class="store-card__badge store-card__badge--planned">Pomodoro bientôt</span>
    <div class="store-card__icon"><i class="fab fa-microsoft" aria-hidden="true"></i></div>
    <h3 class="store-card__name">Microsoft Store</h3>
    <p class="store-card__platform">Windows</p>
    <p class="store-card__price">$4.99</p>
    <a class="store-card__btn" href="https://apps.microsoft.com/detail/9n19p02fc7rf">Acheter</a>
  </div>

  <div class="store-card">
    <span class="store-card__badge store-card__badge--planned">Pomodoro bientôt</span>
    <div class="store-card__icon"><i class="fab fa-app-store-ios" aria-hidden="true"></i></div>
    <h3 class="store-card__name">App Store (iOS / iPadOS)</h3>
    <p class="store-card__platform">iPhone · iPad</p>
    <p class="store-card__price">Gratuit <span class="note">· Glit Pro en achat unique</span></p>
    <a class="store-card__btn" href="https://apps.apple.com/app/glit-web-novel-writing/id6783972543">Obtenir</a>
  </div>

  <div class="store-card">
    <span class="store-card__badge store-card__badge--planned">Pomodoro bientôt</span>
    <div class="store-card__icon"><i class="fab fa-google-play" aria-hidden="true"></i></div>
    <h3 class="store-card__name">Play Store (Android)</h3>
    <p class="store-card__platform">Android</p>
    <p class="store-card__price">Gratuit <span class="note">· Glit Pro en achat unique</span></p>
    <a class="store-card__btn" href="https://play.google.com/store/apps/details?id=com.glitlab.gliteditor">Obtenir</a>
  </div>
</div>

D'autres questions ? Parcourez la FAQ de la page [Assistance](/fr/support.html) ou écrivez-nous à tout moment.
