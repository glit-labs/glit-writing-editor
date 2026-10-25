---
description: "Come usare il Pomodoro su misura di Glit: scegli una modalità nel romanzo a puntate, alterna concentrazione e pausa e imposta l'avviso e il suono di pausa."
last_modified: 2026-10-26
layout: single
title: "Guida al Pomodoro su misura — alterna concentrazione e pausa"
lang: it
locale: "it-IT"
toc: false
guide: true
classes: guide-article
order: 3
summary: "Un timer di concentrazione pensato per la modalità romanzo a puntate. Scegli una modalità, alterna tempi di concentrazione e di pausa, e seleziona un avviso 1 minuto prima e un suono di pausa."
---

<header class="guide-hero">
  <p class="guide-back"><a href="/it/guide.html">← Tutte le guide</a></p>
  <span class="guide-hero__eyebrow">Guida scritta</span>
  <h1 class="guide-hero__title">{{ page.title }}</h1>
  <p class="guide-hero__lead">Il <strong>Pomodoro su misura</strong> è un timer di concentrazione creato per la modalità romanzo a puntate. Durante la concentrazione scrivi e basta; durante la pausa l'editor si blocca perché tu possa riposare davvero. Questa guida spiega come scegliere una modalità, i due modi per iniziare e come impostare l'avviso e il suono di pausa.</p>
  <nav class="section-nav" aria-label="Vai a una sezione">
    <a href="#before-you-start">Prima di iniziare</a>
    <a href="#modes">Scegliere una modalità</a>
    <a href="#custom-mode">Modalità personalizzata</a>
    <a href="#top-bar">Opzione 1. Barra superiore</a>
    <a href="#focus-writing">Opzione 2. Scrittura focalizzata</a>
    <a href="#focus-and-break">Concentrazione e pausa</a>
    <a href="#good-to-know">Buono a sapersi</a>
    <a href="#get-glit">Scarica Glit</a>
  </nav>
</header>

## Prima di iniziare {#before-you-start}

Il Pomodoro su misura è disponibile alle condizioni seguenti.

<div class="info-grid">
  <div class="info-card">
    <h3>Modalità romanzo a puntate</h3>
    <p>Compare solo quando la modalità romanzo a puntate è attiva. Puoi attivarla direttamente dalla barra laterale.</p>
  </div>
  <div class="info-card">
    <h3>Un episodio aperto</h3>
    <p>Apri nell'editor l'episodio che vuoi scrivere oggi.</p>
  </div>
</div>

Ci sono due modi per iniziare. Scegli l'**opzione 1 (barra superiore)** per restare nella normale vista dell'editor, oppure l'**opzione 2 (Scrittura focalizzata)** per dedicare l'intero schermo al manoscritto, insieme a un obiettivo di caratteri e alla modalità difficile. Le due opzioni condividono le stesse impostazioni.

## Scegliere una modalità {#modes}

Scegli una modalità dall'elenco **Tipo e scopo** nella schermata delle impostazioni: concentrazione, pausa e cicli assumono i valori di quella modalità.

| Tipo e scopo | Concentrazione | Pausa | Cicli | Durata totale |
| :-- | :-: | :-: | :-: | :-: |
| **Sblocca-scrittura** · Superare il Writer's Block | 15 min | 3 min | 6 | 105 min |
| **Maestro del seriale quotidiano** · La routine quotidiana più stabile | 25 min | 5 min | 4 | 115 min |
| **Immersione profonda** · Per passaggi lunghi e densi | 50 min | 10 min | 2 | 110 min |

È la prima volta? Inizia con **Sblocca-scrittura**: sei giri da 15 minuti di concentrazione e 3 di pausa. Se hai in mente altri tempi, impostali tu con la [Modalità personalizzata](#custom-mode).

## Imposta i tuoi tempi con la Modalità personalizzata {#custom-mode}

Se nessuna delle tre modalità si adatta al tuo ritmo, imposta tu concentrazione, pausa e cicli. La **Modalità personalizzata** non è una voce da scegliere nell'elenco: il nome compare da solo quando modifichi i valori.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">In <strong>Tipo e scopo</strong>, nella schermata delle impostazioni, scegli la modalità più vicina al ritmo che vuoi. <span class="walkthrough__hint">È solo un punto di partenza, va bene qualsiasi modalità.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Inserisci i numeri che vuoi nei campi <strong>Concentrazione (min)</strong>, <strong>Pausa (min)</strong> e <strong>Cicli</strong>. <span class="walkthrough__hint">Sono accettate solo cifre. La concentrazione va da 1 a 120 minuti, la pausa da 1 a 60 minuti e i cicli da 1 a 12.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Quando i tre valori non corrispondono più a nessuna modalità dell'elenco, il nome diventa <strong>Modalità personalizzata</strong> e la durata totale viene ricalcolata con i tuoi valori. <span class="walkthrough__hint">Riporta i tre valori a quelli di una modalità e ne ricompare il nome.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Controlla la durata totale e fai clic su <strong>Inizia</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Per esempio, con 40 minuti di concentrazione, 8 di pausa e 3 cicli compare <strong>Totale 136 min (2 h 16 min)</strong>. Dopo l'ultimo ciclo non c'è pausa, quindi il totale è <code>concentrazione × cicli + pausa × (cicli − 1)</code> (40 × 3 + 8 × 2 = 136).</p>

### Regole di inserimento

- Un numero superiore al massimo diventa subito il massimo. Per esempio, 150 in concentrazione diventa 120.
- Se lasci un campo vuoto o inserisci 0, diventa il minimo di 1 quando esci dal campo.
- Quando il totale è inferiore a 60 minuti, compare senza le ore, come «Totale 55 min».
- I valori vengono salvati, quindi li ritrovi alla prossima apertura della schermata delle impostazioni o dopo aver riaperto l'app. La versione della barra superiore e quella di Scrittura focalizzata condividono gli stessi valori.

## Opzione 1. Iniziare dalla barra superiore dell'editor {#top-bar}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Con un episodio aperto nella modalità romanzo a puntate, il pulsante <strong>Pomodoro su misura</strong> compare a sinistra nella barra superiore dell'editor. Fai clic su di esso.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method1-it.png" alt="Il pulsante Pomodoro su misura a sinistra nella barra superiore dell'editor" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Nella schermata delle impostazioni scegli un <strong>Tipo e scopo</strong> e, se vuoi, modifica concentrazione, pausa e cicli.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Scegli l'<strong>Avviso 1 min prima</strong> (Westminster, Carillon, Campanello o Disattivato), il <strong>Suono di pausa</strong> (Disattivato, Acqua o Uccelli) e il <strong>Volume</strong>. <span class="walkthrough__hint">Con i pulsanti ▶ puoi ascoltarli in anteprima. Per impostazione predefinita l'avviso è Westminster e il suono di pausa è disattivato.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Fai clic su <strong>Inizia</strong>. La barra laterale si chiude e il pulsante mostra l'avanzamento, ad esempio <strong>Concentrazione 1/4 · 24:59</strong>.</p>
    </div>
  </li>
</ol>

Fai clic sull'indicatore di avanzamento per aprirne il menu.

- **Reimposta** — mantiene il ciclo attuale e riporta all'inizio solo il timer della fase in corso (concentrazione o pausa).
- **Vista compatta / Vista completa** — la vista compatta mostra solo il tempo rimasto; quella completa aggiunge fase e ciclo, come «Concentrazione 1/4 · 2:46». La scelta viene ricordata.
- **Termina** — conclude il Pomodoro su misura.

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Mentre è in corso, la barra laterale è bloccata e la <strong>Scrittura focalizzata</strong> non si può avviare. Al termine, la barra laterale torna com'era. A schermo intero su Mac vengono nascoste anche la barra del titolo e la barra laterale, lasciando solo il manoscritto.</p>

## Opzione 2. Usarlo con la Scrittura focalizzata {#focus-writing}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Apri <strong>Opzioni editor</strong> in fondo all'editor e fai clic su <strong>Scrittura focalizzata</strong>.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method2-it.png" alt="Opzioni editor aperte in basso a destra, con Scrittura focalizzata evidenziata" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Nella schermata delle impostazioni seleziona <strong>Pomodoro su misura</strong>. <span class="walkthrough__hint">La casella compare solo nella modalità romanzo a puntate. Selezionandola si aprono le impostazioni di modalità, tempi, avviso e suono di pausa, insieme alle regole per le pause.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Se vuoi, imposta anche i <strong>Caratteri obiettivo</strong> e la <strong>Modalità difficile</strong>, poi fai clic su <strong>Inizia</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">L'indicatore di avanzamento compare discretamente in basso a destra. Fai clic su di esso per scegliere <strong>Reimposta</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Con la <strong>Modalità difficile</strong> attiva, non puoi uscire dalla Scrittura focalizzata finché non raggiungi l'obiettivo di caratteri, anche dopo aver completato tutti i cicli.</p>

## Concentrazione e pausa {#focus-and-break}

Le due opzioni seguono lo stesso percorso.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text"><strong>Concentrazione</strong> — pensa solo a scrivere. Quando manca un minuto, i bordi dello schermo si illuminano dolcemente tre volte con il colore del tema e l'avviso suona una volta. <span class="walkthrough__hint">Puoi continuare a scrivere mentre si illuminano. Approfittane per chiudere la frase.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Al termine della concentrazione compare la finestra <strong>«Fine della concentrazione»</strong>. La pausa inizia solo dopo aver fatto clic su <strong>OK</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text"><strong>Pausa</strong> — l'editor si blocca e compare solo l'avviso di pausa. Le finestre di anteprima aperte si chiudono e la barra laterale secondaria resta nascosta fino alla fine della pausa. Se hai scelto un suono di pausa, viene ripetuto per tutta la pausa. <span class="walkthrough__hint">Fai clic sull'icona dell'altoparlante accanto all'indicatore di avanzamento per cambiare suono o volume durante la pausa.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Al termine della pausa compare la finestra <strong>«Fine della pausa»</strong>. Fai clic su <strong>OK</strong> per iniziare la concentrazione successiva.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Dopo la concentrazione dell'ultimo ciclo non c'è pausa: compare invece la finestra <strong>«Pomodoro su misura completato»</strong>. Fai clic su <strong>OK</strong> per terminare e lo schermo torna com'era prima di iniziare.</p>

### Sfruttare al meglio le pause

Anche la schermata delle impostazioni ricorda queste due regole.

- Durante le pause evita ciò che lascia **residui di attenzione**, come controllare i messaggi o guardare video. Riduce la concentrazione nella sessione successiva.
- Durante le pause, se puoi, **chiudi gli occhi per riposare o fai stretching**.

## Buono a sapersi {#good-to-know}

<div class="faq">
  <div class="faq__item">
    <p class="faq__q">Le impostazioni vengono salvate?</p>
    <p class="faq__a">Sì. Gli ultimi tempi di concentrazione e pausa, i cicli e le impostazioni audio vengono salvati, quindi li ritrovi al prossimo avvio o dopo aver riaperto l'app. Le due opzioni condividono le stesse impostazioni.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">Se chiudo e riapro l'app, il timer in corso continua?</p>
    <p class="faq__a">No. Una sessione in corso non viene ripristinata: avviane una nuova.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">Non vedo il pulsante.</p>
    <p class="faq__a">Controlla che la modalità romanzo a puntate sia attiva e che sia aperto un episodio. Disattivando la modalità romanzo a puntate durante una sessione, termina anche il Pomodoro su misura.</p>
  </div>
</div>

## Scarica Glit {#get-glit}

Glit è disponibile negli store qui sotto.

<div class="store-grid">
  <div class="store-card">
    <span class="store-card__badge store-card__badge--included">Pomodoro incluso</span>
    <div class="store-card__icon"><i class="fab fa-app-store" aria-hidden="true"></i></div>
    <h3 class="store-card__name">Mac App Store</h3>
    <p class="store-card__platform">macOS</p>
    <p class="store-card__price">$4.99</p>
    <a class="store-card__btn" href="https://apps.apple.com/us/app/glit-web-novel-writing-editor/id6764386721">Acquista ora</a>
  </div>

  <div class="store-card">
    <span class="store-card__badge store-card__badge--planned">Pomodoro in arrivo</span>
    <div class="store-card__icon"><i class="fab fa-microsoft" aria-hidden="true"></i></div>
    <h3 class="store-card__name">Microsoft Store</h3>
    <p class="store-card__platform">Windows</p>
    <p class="store-card__price">$4.99</p>
    <a class="store-card__btn" href="https://apps.microsoft.com/detail/9n19p02fc7rf">Acquista ora</a>
  </div>

  <div class="store-card">
    <span class="store-card__badge store-card__badge--planned">Pomodoro in arrivo</span>
    <div class="store-card__icon"><i class="fab fa-app-store-ios" aria-hidden="true"></i></div>
    <h3 class="store-card__name">App Store (iOS / iPadOS)</h3>
    <p class="store-card__platform">iPhone · iPad</p>
    <p class="store-card__price">Gratis <span class="note">· Glit Pro con acquisto unico</span></p>
    <a class="store-card__btn" href="https://apps.apple.com/app/glit-web-novel-writing/id6783972543">Ottieni</a>
  </div>

  <div class="store-card">
    <span class="store-card__badge store-card__badge--planned">Pomodoro in arrivo</span>
    <div class="store-card__icon"><i class="fab fa-google-play" aria-hidden="true"></i></div>
    <h3 class="store-card__name">Play Store (Android)</h3>
    <p class="store-card__platform">Android</p>
    <p class="store-card__price">Gratis <span class="note">· Glit Pro con acquisto unico</span></p>
    <a class="store-card__btn" href="https://play.google.com/store/apps/details?id=com.glitlab.gliteditor">Ottieni</a>
  </div>
</div>

Hai altre domande? Sfoglia le FAQ nella pagina [Supporto](/it/support.html) o scrivici quando vuoi.
