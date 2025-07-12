---
date: 2024-01-19
categories:
  - lernos
  - produktionskette
  - github
  - 37c3
---

# Lightning Talk zur lernOS Produktionskette auf dem 37C3

Beim [37. Chaos Communication Congress](https://events.ccc.de/category/37c3/) ([#37C3](https://chaos.social/tags/37c3)) hat [Simon](https://www.linkedin.com/in/simondueckert/) einen Lightning Talk mit dem Titel **"Single Source Publishing mit Markdown, Github, Mkdocs, Material und Pandoc"** gehalten ([Folien](https://cloud.dueckert.eu/s/YW2Sw98nDPrWGqT)). Aus der Kurzbeschreibung:

> Das Open Source Projekt lernOS (lernos.org) verwendet für die Publikation von Lern-Leitfäden Markdown-Quellen, die über eine Produktionskette mit pandoc in eine Webseite sowie PDF- und E-Book-Versionen konvertiert wird. Der Lightning Talk stellt den Ansatz vor und zeigt einige Problemfelder.

<!-- more -->

Die Lightning Talks des 37C3 sind zusätzlich zu [den Vortragsaufzeichnungen](https://media.ccc.de/c/37c3) (auch als [Playlist auf YouTube](https://www.youtube.com/watch?v=se0jni9bPBQ&list=PL_IxoDz1Nq2ZaHqsvqyBCrm8EdCTvkIxr)) auf media.ccc.de [in einem eigenen Kanal](https://media.ccc.de/c/37c3-meta) veröffentlicht.

<iframe width="1024" height="576" src="https://media.ccc.de/v/37c3-lightningtalks-58012-single-source-publishing-mit-markdown-github-mkdocs-material-und-pandoc/oembed" frameborder="0" allowfullscreen></iframe>

Anmerkung Simon: im Nachgang des Lightning Talks kam Maximilian in die Sendegate Assembly und hat Unterstützung bei der Umsetzung der Produktionskette auf Github angeboten. Insbesondere hat er darauf hingewiesen, dass es kein sauberer Stil ist, die Binärdateien (PDF, Word etc.) im Repository abzulegen. Grund: jede Version wird dort gespeichert und das macht das Repository auf Dauer sehr groß und unhandlich ("skaliert nicht"). Besser wäre, die Binärdateien immer beim jeweiligen Release abzulegen, so [wie das der Leitfaden Prozessmodellierung gemacht hat](https://github.com/cogneon/lernos-prozessmodellierung/releases) (die "Assets"). Das greifen wir im Kernteam auf und besprechen, ob das mit unser Produktionskette v2 auch geht.