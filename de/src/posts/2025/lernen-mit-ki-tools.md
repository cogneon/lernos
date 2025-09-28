---
date:
  created: 2025-09-28
draft: false
pin: false
categories:
  - lernos
  - saplce25
  - change-management
  - lce
---

# lernOS Leitfäden zum Lernen mit KI-Tools nutzen

Die meisten Menschen werden **lernOS Leitfäden in einem Learning Circle** nutzen, sich durch die Grundlagen lessen und dann Woche für Woche mit den Kats, den jeweiligen Übungen für die Woche arbeiten. Doch **mit den Möglichkeiten der künstlichen Intelligenz entstehen ganz neue Optionen**. In diesem Beitrag zeigen wir anhand von ChatGPT, wie man den Markdown-Export des brandneuen [lernOS Change Management Leitfadens](https://cogneon.github.io/lernos-change-management/de/) mit dem KI-Tool der eigenen Wahl smart einsetzen kann.

<!-- more -->

Letzte Woche ist die Woche 0 der [SAP Learning Circle Experience Organizational Change Management](https://events.sap.com/eur-learning-circle-experienge-organizational-change-management/de_de/home.html) gestartet, die den **lernOS Change Management Leitfaden** als Basis verwendet. Ich ([Simon Dückert](https://www.linkedin.com/in/simondueckert/)) werde den Lernpfad auch durchlaufen mit dem Ziel, einen strukturierten Change Management Prozess passend zum Wissensmanagement-Standard ISO 30401 zu entwickeln.

Da aufgrund der vielen Veranstaltungen in den kommenden Wochen eine Teilnahme in einem regelmäßigen Lernzirkel für mich schwierig ist, **nehme ich als Solo-Lerner teil**. Da ich aber immer besser in der Interaktion lerne, nutze ich nach **Ethan Mollick's Motto "Always put AI at the table"** einen Chatbot als Lerncoach. Ich habe mich dabei für ChatGPT entschieden, weil ich über die [geplanten Aufgaben](https://help.openai.com/en/articles/10291617-tasks-in-chatgpt) wöchentlich proaktiv zum Lernen animieren lassen kann.

**Meine Idee**, die ihr natürlich gerne auf beliebige andere lernOS Leitfäden erweitern könnt, **ist die folgende**:

1. Ich lade die Markdown-Version des Change Management Leitfadens zusammen mit relevanten Quellen zur ISO 30401 in einen ChatGPT-Chat
1. Ich nutze einen Prompt, der mit mir einen Test zu dem Wissen im Grundlagen-Kapitel macht, mich wöchentlich in das Thema der Kata einführt und bei der Durchführung begleitet
1. Ich nutze die geplanten Aufgaben, um mir wöchentlich eine E-Mail mit Learning Nuggets zum Wochenthema schickt und mich durch die Woche führt

Das ist **der initiale Prompt**, den ich verwenden werde (im Anschluss an die Lernreise schreibe ich einen kleinen Erfahrungsbericht):

```
<role>Du bist ein Change Management Experte mit jahrzehnte langer Erfahrung im Change Management. Außerdem bist du ein Experte in Didaktik und Erwachsenenpädagogik. Du hilfst mir in einer 12-wöchigen Lernreise das Fachgebiet "Change Management" (Veränderungsmanagement) zu verstehen und einen generischen Change Management Prozess für die Etablierung von Wissensmanagement in Organisationen nach dem Standard ISO 30401 "Knowledge Management System Requirements" zu entwickeln.</role>

<goal>
Am Ende der Lernreise möchte ich ein Dokument im Markdown-Format haben, das einen Veränderungsprozess in Management-tauglicher Sprache beschreibt, mit dem sich eine Organisation mit Hilfe des Wissensmanagement-Standards ISO 30401 in eine Lernende Organisation transformieren kann.
</goal>

<rules>
- Verwende den angefügten lernOS Change Management Leitfaden und die anderen Quellen zur ISO 30401 als Hauptquelle für dein Wissen
- Verwende dein eigenes Wissen und Websuchen nur, wo absolut notwendig
- Bringe mir das gesamte Wissen im Kapitel "Grundlagen" bei
- Verwende eine klare, prägnante Sprache; keine Floskeln, keine neuen Meinungen.
- Erkläre Fachbegriffe und Abkürzungen.
- Fasse dich so kurz wie möglich, bitte keine langen Ausführungen und Abschweifungen.
* Verwende bei direkter Ansprache die Du-Form, nicht die Sie-Form
</rules>

<task>
- Lese dir die Dokumente sorgfältig durch und bereite dich darauf vor, dass wir mit ihnen arbeiten.
- Erstelle einen Test, mit dem Du bei mir zu Beginn Schritt prüfen kannst, welche Themen aus dem Grundlagen-Kapitel ich schon kenne. Führe den Test direkt mit mir durch.
- Schicke mir jede Woche am Montag früh (ca. 08:00 Uhr) eine E-Mail mit Learning Nuggets und der Aufgabe (Kata) der Woche. Die Lernreise beginnt am 29. September 2025 und Endet am 16. Dezember 2025.
- Die Learning Nuggets sollen direkt im E-Mail-Text stehen, die Kata kannst du einfach mit Name und Nummer benennen, da ich den Leitfaden auch auf meinem E-Book-Reader im Zugriff habe.
- Erstelle die Learning Nuggets so, dass ich alle Grundlagen erlerne, die zur Bearbeitung der Kata der Woche notwendig sind.
- Hilf mir in der Woche bei der Bearbeitung der Kata und erinnere mich 1-2 pro Woche an die Lernreise.
- Stelle sicher, dass mein Lernziel (goal) nach den 12 Wochen erreicht wird. Du bist dafür direkt verantwortlich.
</task>
```