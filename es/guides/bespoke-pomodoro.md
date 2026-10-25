---
description: "Cómo usar el Pomodoro a medida de Glit: elige un modo en el modo novela por entregas, alterna concentración y descanso y ajusta el aviso y el sonido de descanso."
last_modified: 2026-10-26
layout: single
title: "Guía del Pomodoro a medida — alterna concentración y descanso"
lang: es
locale: "es-ES"
toc: false
guide: true
classes: guide-article
order: 3
summary: "Un temporizador de concentración pensado para el modo novela por entregas. Elige un modo, alterna tiempos de concentración y de descanso, y escoge un aviso 1 minuto antes y un sonido de descanso."
---

<header class="guide-hero">
  <p class="guide-back"><a href="/es/guide.html">← Todas las guías</a></p>
  <span class="guide-hero__eyebrow">Guía escrita</span>
  <h1 class="guide-hero__title">{{ page.title }}</h1>
  <p class="guide-hero__lead">El <strong>Pomodoro a medida</strong> es un temporizador de concentración hecho para el modo novela por entregas. Durante la concentración solo escribes; durante el descanso el editor se bloquea para que descanses de verdad. Esta guía explica cómo elegir un modo, las dos formas de empezar y cómo ajustar el aviso y el sonido de descanso.</p>
  <nav class="section-nav" aria-label="Ir a una sección">
    <a href="#before-you-start">Antes de empezar</a>
    <a href="#modes">Elegir un modo</a>
    <a href="#custom-mode">Modo personalizado</a>
    <a href="#top-bar">Opción 1. Barra superior</a>
    <a href="#focus-writing">Opción 2. Escritura concentrada</a>
    <a href="#focus-and-break">Concentración y descanso</a>
    <a href="#good-to-know">Conviene saber</a>
  </nav>
</header>

## Antes de empezar {#before-you-start}

El Pomodoro a medida está disponible cuando se cumplen estas condiciones.

<div class="info-grid">
  <div class="info-card">
    <h3>Glit para Mac 1.5.0 o posterior</h3>
    <p>Actualiza Glit a la última versión desde la Mac App Store.</p>
  </div>
  <div class="info-card">
    <h3>Modo novela por entregas</h3>
    <p>Solo aparece con el modo novela por entregas activado. Puedes activarlo directamente desde la barra lateral.</p>
  </div>
  <div class="info-card">
    <h3>Un episodio abierto</h3>
    <p>Abre en el editor el episodio que vas a escribir hoy.</p>
  </div>
</div>

Hay dos formas de empezar. Elige la **opción 1 (barra superior)** para seguir con la vista normal del editor, o la **opción 2 (Escritura concentrada)** para dedicar toda la pantalla al manuscrito, junto con un objetivo de caracteres y el modo difícil. Las dos opciones comparten los mismos ajustes.

## Elegir un modo {#modes}

Elige un modo en la lista **Tipo y propósito** de la pantalla de ajustes, y el tiempo de concentración, el de descanso y los ciclos pasan a los valores de ese modo.

| Tipo y propósito | Concentración | Descanso | Ciclos | Tiempo total |
| :-- | :-: | :-: | :-: | :-: |
| **Modo rompebloqueos** · Romper el Writer's Block | 15 min | 3 min | 6 | 105 min |
| **Modo maestro de serial diario** · La rutina diaria más estable | 25 min | 5 min | 4 | 115 min |
| **Modo inmersión profunda** · Para pasajes largos y densos | 50 min | 10 min | 2 | 110 min |

¿Es tu primera vez? Empieza con el **Modo maestro de serial diario**: cuatro rondas de 25 minutos de concentración y 5 de descanso son la medida justa para un episodio. Si tienes otros tiempos en mente, fíjalos tú con el [Modo personalizado](#custom-mode).

## Fija tus propios tiempos con el Modo personalizado {#custom-mode}

Si ninguno de los tres modos encaja con tu ritmo, fija tú la concentración, el descanso y los ciclos. El **Modo personalizado** no es una opción que se elija en la lista: el nombre aparece solo cuando cambias los valores.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">En <strong>Tipo y propósito</strong>, en la pantalla de ajustes, elige el modo más parecido al ritmo que quieres. <span class="walkthrough__hint">Es solo un punto de partida, así que cualquiera sirve.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Escribe los números que quieras en los campos <strong>Concentración (min)</strong>, <strong>Descanso (min)</strong> y <strong>Ciclos</strong>. <span class="walkthrough__hint">Solo se aceptan cifras. La concentración puede ir de 1 a 120 minutos, el descanso de 1 a 60 minutos y los ciclos de 1 a 12.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Cuando los tres valores ya no coinciden con ningún modo de la lista, el nombre pasa a <strong>Modo personalizado</strong> y el tiempo total se recalcula con tus valores. <span class="walkthrough__hint">Si vuelves a dejar los tres valores iguales a los de un modo, recupera su nombre.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Revisa el tiempo total y haz clic en <strong>Empezar</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Por ejemplo, con 40 minutos de concentración, 8 de descanso y 3 ciclos se muestra <strong>Total 136 min (2 h 16 min)</strong>. Después del último ciclo no hay descanso, así que el total es <code>concentración × ciclos + descanso × (ciclos − 1)</code> (40 × 3 + 8 × 2 = 136).</p>

### Reglas de entrada

- Un número mayor que el máximo pasa al máximo al instante. Por ejemplo, si escribes 150 en concentración, queda en 120.
- Si dejas un campo vacío o escribes 0, pasa al mínimo de 1 al salir del campo.
- Cuando el total es inferior a 60 minutos, se muestra sin horas, como «Total 55 min».
- Tus valores se guardan, así que siguen ahí la próxima vez que abras la pantalla de ajustes o la app. La versión de la barra superior y la de Escritura concentrada comparten los mismos valores.

## Opción 1. Empezar desde la barra superior del editor {#top-bar}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Con un episodio abierto en el modo novela por entregas, el botón <strong>Pomodoro a medida</strong> aparece a la izquierda de la barra superior del editor. Haz clic en él.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method1-es.png" alt="El botón Pomodoro a medida a la izquierda de la barra superior del editor" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">En la pantalla de ajustes, elige un <strong>Tipo y propósito</strong> y, si quieres, ajusta la concentración, el descanso y los ciclos.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Elige el <strong>Aviso 1 min antes</strong> (Westminster, Caja de música, Campanilla o Desactivado), el <strong>Sonido de descanso</strong> (Desactivado, Agua o Pájaros) y el <strong>Volumen</strong>. <span class="walkthrough__hint">Usa los botones ▶ para escucharlos. El aviso es Westminster por defecto y el sonido de descanso está desactivado.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Haz clic en <strong>Empezar</strong>. La barra lateral se cierra y el botón muestra el progreso, por ejemplo <strong>Concentración 1/4 · 24:59</strong>.</p>
    </div>
  </li>
</ol>

Haz clic en el indicador de progreso para abrir su menú.

- **Reiniciar** — mantiene el ciclo actual y solo devuelve al inicio el temporizador de la fase en curso (concentración o descanso).
- **Vista compacta / Vista completa** — la vista compacta muestra solo el tiempo restante; la completa añade la fase y el ciclo, como en «Concentración 1/4 · 2:46». Tu elección se recuerda.
- **Terminar** — finaliza el Pomodoro a medida.

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Mientras está en marcha, la barra lateral queda bloqueada y no se puede iniciar la <strong>Escritura concentrada</strong>. Al terminar, la barra lateral vuelve a como estaba. En pantalla completa en Mac, también se ocultan la barra de título y la barra lateral, y solo queda tu manuscrito.</p>

## Opción 2. Usarlo con la Escritura concentrada {#focus-writing}

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text">Abre <strong>Opciones del editor</strong> en la parte inferior del editor y haz clic en <strong>Escritura concentrada</strong>.</p>
    </div>
    <img class="walkthrough__img walkthrough__img--window" src="/assets/images/guide/bespoke-pomodoro-method2-es.png" alt="Opciones del editor abiertas abajo a la derecha, con Escritura concentrada resaltada" />
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">En la pantalla de ajustes, marca <strong>Pomodoro a medida</strong>. <span class="walkthrough__hint">La casilla solo aparece en el modo novela por entregas. Al marcarla se despliegan los ajustes de modo, tiempos, aviso y sonido de descanso, junto con las reglas del descanso.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text">Si quieres, fija también los <strong>Caracteres objetivo</strong> y el <strong>Modo difícil</strong>, y haz clic en <strong>Empezar</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">El indicador de progreso aparece discretamente en la esquina inferior derecha. Haz clic en él para elegir <strong>Reiniciar</strong>.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Con el <strong>Modo difícil</strong> activado, no puedes salir de la Escritura concentrada hasta alcanzar tu objetivo de caracteres, aunque hayas terminado todos los ciclos.</p>

## Concentración y descanso {#focus-and-break}

Las dos opciones siguen el mismo recorrido.

<ol class="walkthrough">
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">1</span>
      <p class="walkthrough__text"><strong>Concentración</strong> — piensa solo en escribir. Cuando queda un minuto, los bordes de la pantalla brillan suavemente tres veces con el color del tema y el aviso suena una vez. <span class="walkthrough__hint">Puedes seguir escribiendo mientras brilla. Aprovéchalo para cerrar la frase.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">2</span>
      <p class="walkthrough__text">Al terminar la concentración aparece el aviso <strong>«Fin de la concentración»</strong>. El descanso empieza solo cuando haces clic en <strong>Aceptar</strong>.</p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">3</span>
      <p class="walkthrough__text"><strong>Descanso</strong> — el editor se bloquea y solo se muestra el aviso de descanso. Las ventanas de vista previa abiertas se cierran y la barra lateral secundaria se oculta hasta que acaba el descanso. Si elegiste un sonido de descanso, se repite durante todo el descanso. <span class="walkthrough__hint">Haz clic en el icono del altavoz junto al indicador de progreso para cambiar el sonido o el volumen durante el descanso.</span></p>
    </div>
  </li>
  <li>
    <div class="walkthrough__head">
      <span class="walkthrough__num">4</span>
      <p class="walkthrough__text">Al terminar el descanso aparece el aviso <strong>«Fin del descanso»</strong>. Haz clic en <strong>Aceptar</strong> para empezar la siguiente concentración.</p>
    </div>
  </li>
</ol>

<p class="walkthrough__done"><i class="fas fa-check" aria-hidden="true"></i>Tras la concentración del último ciclo no hay descanso: aparece el aviso <strong>«Pomodoro a medida completado»</strong>. Haz clic en <strong>Aceptar</strong> para terminar, y la pantalla vuelve a como estaba antes de empezar.</p>

### Cómo aprovechar los descansos

La pantalla de ajustes también muestra estas dos reglas.

- En los descansos, evita lo que deja **residuo de atención**, como revisar mensajes o ver vídeos. Reduce tu concentración en la siguiente sesión.
- En los descansos, si puedes, **cierra los ojos para descansar o estírate**.

## Conviene saber {#good-to-know}

<div class="faq">
  <div class="faq__item">
    <p class="faq__q">¿Se guardan los ajustes?</p>
    <p class="faq__a">Sí. Se guardan la última concentración, descanso, ciclos y ajustes de sonido que usaste, así que siguen ahí la próxima vez que empieces o abras la app. Las dos opciones comparten los mismos ajustes.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">Si cierro y vuelvo a abrir la app, ¿continúa el temporizador?</p>
    <p class="faq__a">No. Una sesión en curso no se restaura, así que empieza una nueva.</p>
  </div>
  <div class="faq__item">
    <p class="faq__q">No veo el botón.</p>
    <p class="faq__a">Comprueba que el modo novela por entregas está activado y que hay un episodio abierto. Si desactivas el modo novela por entregas durante una sesión, el Pomodoro a medida también termina.</p>
  </div>
</div>

Consulta las [notas de la versión macOS v1.5.0](/releases/mac/v1.5.0/es.html) para ver el resto de cambios de esta actualización. ¿Tienes más preguntas? Revisa las preguntas frecuentes en la página de [Soporte](/es/support.html) o escríbenos cuando quieras.
