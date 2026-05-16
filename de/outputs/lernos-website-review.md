# Review der lernOS Website (https://lernos.org/de/)

*Externes Feedback aus der Perspektive der drei Zielgruppen. Grundlage: Markdown-Quellen im Verzeichnis, keine Änderungen vorgenommen.*

---

## Erster Eindruck (vor Bearbeitung der Leitfragen)

Die Startseite kommuniziert in den ersten zehn Sekunden, **was lernOS ist** ("offenes System für selbstgesteuertes Lernen und Peer Learning") und **für wen** ("Ich will lernen / Ich will an Leitfäden mitarbeiten / Ich will lernOS in meiner Organisation"). Das Drei-Karten-Layout ist die stärkste gestalterische Entscheidung der Seite, weil es den Nutzer in der ersten Interaktion zur richtigen Pfadwahl zwingt, anstatt ihn lesen zu lassen.

Die Schwächen werden ebenfalls schnell sichtbar: Es gibt **viele Kanäle** (Discord, CONNECT, Mastodon, LinkedIn, Newsletter, Podcast, RSS, Meetup), aber kein klares Bild, welcher Kanal welche Funktion hat. Begriffe wie **Kata, Sprint, Circle, Weekly, Boxenstopp** tauchen verstreut auf, ohne dass es eine zentrale Stelle gibt, an der sie definiert sind. Die Beziehung zwischen **lernOS und Cogneon** wird auf der Website weder erklärt noch sauber getrennt - sie erscheint nur als Sponsor-Hinweis im Footer.

Aufgeräumt, freundlich, technisch solide. Aber an mehreren Stellen redundant und an wenigen Stellen schlampig.

---

## Zielgruppe 1: Lernende (Newbies)

| Leitfrage | Befund |
|---|---|
| Verstehst du sofort, was lernOS ist und was es dir bringt? | **Ja.** Der Einstiegsabsatz auf `index.md` ist präzise. Das "lernOS in a Nutshell"-Bild und der 5-Minuten-Lightning-Talk sind starke Anker. |
| Findest du schnell einen passenden Einstieg? | **Bedingt.** Die Karte "Ich will lernen" leitet zu `guides.md` - dort findet man aber eine lange Liste, ohne klare Empfehlung für den ersten Schritt. Erst im Fließtext wird "lernOS für Dich" als Einstieg empfohlen. |
| Ist klar, wie du einen Learning Circle startest? | **Ja, sehr gut.** `learning-circles.md` enthält eine konkrete Checkliste für Woche 0 und alle Folgewochen. Das ist eine der stärksten Seiten der ganzen Website. |
| Weißt du, wo du Fragen stellen und Mitlerner finden kannst? | **Teilweise.** CONNECT, Discord, LinkedIn und Peerfinder werden alle erwähnt, aber die Funktionsteilung (CONNECT = Lernende, Discord = Maintainer) wird erst auf `contribute.md` klar ausgesprochen. Auf den Lernenden-relevanten Seiten fehlt dieser Hinweis. |
| Begriffe oder Konzepte unklar? | **Ja.** *Kata* wird auf der Startseite und in `guides.md` benutzt, aber erst in `learning-circles.md` über einen Wikipedia-Link erklärt. *Weekly*, *Boxenstopp*, *Sprint*, *Lernpfad* haben keine zentrale Definition. Ein kurzes **Glossar** würde sehr helfen. |

**Konkrete Reibungspunkte:**

- `guides.md` enthält den Link `[lernOS Leitfäden](1-guides.md)` und `learning-circles.md` enthält `/de/1-guides/` - beides läuft vermutlich ins Leere und wirkt wie ein Rest einer alten Verzeichnisstruktur.
- "lernOS für Teams (noch nicht verfügbar)" steht prominent in der Core-Liste, ohne Zeithorizont. Das wirkt wie ein offenes Versprechen.
- Auf `learning-circles.md` werden zwei verschiedene Sprint-Grafiken eingebunden (eine extern von GitHub, eine lokal als SVG). Optisch unruhig.

---

## Zielgruppe 2: Leitfaden-Teams

| Leitfrage | Befund |
|---|---|
| Findest du schnell heraus, wie du mitmachen kannst? | **Ja.** `contribute.md` trennt sauber zwischen Lernenden, Maintainern und Redakteuren. Die Aufforderung "Melde dich im Discord" ist eindeutig. |
| Ist die Produktionskette (Markdown, GitHub, Pandoc, mkdocs) verständlich erklärt? | **Im Überblick ja, im Detail nein.** `create-guide.md` listet die Tools auf und verweist auf das Template-Repository. Eine technische Schritt-für-Schritt-Anleitung auf der Website selbst gibt es nicht - sie wird vollständig nach GitHub ausgelagert. Für nicht-technische Maintainer ist das eine harte Kante. |
| Weißt du, wo du dich mit anderen Leitfaden-Teams koordinierst? | **Ja, Discord.** Wird mehrfach klar genannt. |
| Sind die Anforderungen an einen lernOS Leitfaden klar (Struktur, Lizenz, Qualität)? | **Struktur und Lizenz: ja** (Grundlagen + Lernpfad mit 11 Katas + Anhang, CC BY 4.0, 13 Wochen, max. 2h/Woche). **Qualität: nein** - es gibt keinen sichtbaren Review- oder Freigabeprozess, keine Definition, was 0.x von 1.0 unterscheidet außer "Praxistest". |

**Konkrete Reibungspunkte:**

- `create-guide.md` endet abrupt mit einem einzelnen Aufzählungspunkt unter "Fragen und Unterstützung" - dort fehlen offenbar weitere Anlaufstellen (CONNECT? Simon direkt? Issue-Tracker?). Die Seite wirkt unfertig.
- In `guides/zettelkasten.md` und `guides/sketchnoting.md` wird unter "Links" jeweils die "Webversion lernOS KI Leitfaden" verlinkt - das ist ein Copy-Paste-Fehler aus der KI-Leitfaden-Vorlage. Dasselbe Muster bei `guides/problem-solving.md` ("Der lernOS KI Leitfadens richtet sich an Personen..." im Zielgruppen-Abschnitt).
- Die Liste der Leitfäden-Teams (z.B. KI-Leitfaden) wirkt vertrauensbildend, aber nur ein Bruchteil der Leitfäden hat überhaupt eine eigene Übersichtsseite unter `/guides/`. Die Mehrheit ist nur als Linkliste in `guides.md` aufgeführt.

---

## Zielgruppe 3: Organisationen

| Leitfrage | Befund |
|---|---|
| Verstehst du, welchen Mehrwert lernOS für deine Organisation hat? | **Ja.** Der Einstieg über das 70-20-10-Modell auf `for-organizations.md` ist überzeugend: "Die meisten Organisationen investieren in 10%, lernOS adressiert die 90%." Das ist eine klare, in zwei Sätzen kommunizierbare Wertversprechung. |
| Sind konkrete Einstiegsszenarien für Organisationen beschrieben? | **Ja, drei Szenarien:** Pilotgruppe, Intranet-Integration, Koalition des Lernens. Sehr nützlich. |
| Ist klar, wie lernOS in bestehende Lerninfrastruktur (LMS, Intranet) integriert werden kann? | **Nur ansatzweise.** Ein Satz: "Leitfäden können als PDF oder Webversion direkt ins Intranet oder LMS eingebunden werden, die CC-BY-Lizenz erlaubt das." Für L&D- oder IT-Verantwortliche ist das zu dünn. Es fehlen: Beispiele, technische Optionen (SCORM? xAPI?), Single-Sign-On-Aspekte, Reporting. |
| Findest du Informationen zu professioneller Begleitung bei der Einführung? | **Nein, nicht auf der lernOS-Website.** Es gibt einen Link zu `cogneon.de/lernos` (Supporter-Modell), aber keine eigene Seite "Begleitung & Beratung". Wer Hilfe sucht, muss raten. |
| Ist die Trennung zwischen kostenlosem Open-Source-Projekt (lernOS) und kommerziellem Dienstleister (Cogneon) verständlich? | **Nein.** Cogneon taucht nur im Footer-Copyright und im Supporter-Hinweis auf. Es wird nirgends auf der Website ausgesprochen, dass lernOS das Open-Source-Projekt ist und Cogneon der Initiator/Sponsor/Dienstleister. Für eine seriöse organisationale Bewertung ist das ein zentrales Vertrauensthema - und genau dort eine Leerstelle. |

---

## Allgemeine Fragen

### Drei Dinge, die positiv überrascht haben

1. **Die Drei-Karten-Architektur der Startseite.** Drei klar getrennte Personas, drei klar getrennte Einstiege. Das ist eine reife Designentscheidung.
2. **Die Operationalisierung der Learning Circles.** Die Wochen-Checklisten in `learning-circles.md` sind handwerklich exzellent: Timeboxen in Minuten, Check-in/Check-out-Struktur, Boxenstopps. Ein Team könnte morgen damit starten.
3. **Die konsequente CC-BY-Lizenzierung.** Auf jeder relevanten Seite wiederholt, mit Lizenz-Logo verlinkt, kommerziell nutzbar. Das senkt die Eintrittshürde für Organisationen massiv und ist ein echtes Differenzierungsmerkmal gegenüber proprietären L&D-Programmen.

### Drei Dinge, die irritiert haben

1. **Begriffliche Unbestimmtheit.** *Kata, Sprint, Circle, Weekly, Boxenstopp, Lernpfad* werden über fünf Seiten verteilt eingeführt, oft nur im Kontext. Ein einseitiges Glossar fehlt. Für jemanden, der das Vokabular zum ersten Mal liest, ist das eine Kohärenzlücke.
2. **Kanalvielfalt ohne klare Funktionstrennung.** Discord, CONNECT, Mastodon, LinkedIn, Newsletter, Podcast, RSS, Meetup, Spotify. Die Trennung "Discord = Maintainer / CONNECT = Lernende" wird nur an einer Stelle ausgesprochen. Auf der Startseite stehen alle Kanäle gleichberechtigt - das ist eine Entscheidung, die Nutzer trifft, nicht die Website.
3. **Handwerkliche Schluffigkeiten.** Copy-Paste-Fehler in Zettelkasten- und Sketchnoting-Leitfaden ("lernOS KI Leitfaden" statt des jeweiligen Themas), Tippfehler "Working Out Looud" im FAQ und "39C§" im Blog-Titel, vermutlich tote interne Links (`1-guides.md`), abrupt endende `create-guide.md`. Einzeln Kleinigkeiten, in Summe ein professioneller Eindruck mit Rauschen.

### Was fehlt, das man erwartet hätte

1. **Ein Glossar zentraler Begriffe.**
2. **Eine "lernOS in der Praxis"-Seite mit Fallstudien.** Es werden Logos großer Organisationen (SAP, DATEV, Telekom, Siemens Healthineers, Bayernwerk, LV1871 etc.) im Verzeichnis bereitgehalten, aber auf keiner Seite gezeigt. Das ist verschenktes Vertrauenskapital.
3. **Eine klare "lernOS vs. Cogneon"-Erklärseite.** Wer betreibt das Projekt, wer finanziert es, wo hört Open Source auf, wo fängt kommerzielle Begleitung an. Zwei Absätze würden reichen.
4. **Eine "Erste 15 Minuten"-Spur für Newbies**, die jemanden ohne Vorwissen aktiv durch *Was → Warum → Wie starten* führt.
5. **Sichtbarer Reifegrad / Wirkungsbelege:** Anzahl Circles, Anzahl Lernender, Reichweite. Eine kleine Kennzahlenleiste auf der Startseite.

### Wie vertrauenswürdig und professionell wirkt die Seite?

Vertrauensaufbauend wirken: die offene Lizenz, die namentliche Nennung realer Leitfaden-Teams mit LinkedIn-Profilen, die transparente Verlinkung des GitHub-Repositories, die Open-Source-Produktionskette, die mehrjährige Publikationsliste mit konkreten Vorträgen und Podcasts.

Vertrauensmindernd wirken: die ungeklärte Beziehung zu Cogneon, die Copy-Paste-Fehler in den Leitfaden-Übersichten, das Fehlen jeder Wirkungsmessung oder Kundenreferenz auf den Seiten selbst.

Gesamteindruck: **professionell und glaubwürdig, aber unter eigenem Niveau geliefert.** Die Substanz - die Methodik, die Leitfäden, die Community-Struktur - ist offensichtlich gewachsen und tragfähig. Die Website schöpft das nicht aus.

---

## Empfehlungen (priorisiert)

1. **Glossar anlegen** (`glossary.md` in der Navigation) - eine Seite, zehn Begriffe, je drei Zeilen.
2. **`create-guide.md` zu Ende schreiben** und Copy-Paste-Fehler in den Leitfaden-Seiten (`guides/*.md`) korrigieren.
3. **"lernOS und Cogneon"-Erklärbox** auf `for-organizations.md` und in den Footer - zwei Absätze reichen.
4. **Tote interne Links prüfen** (`1-guides.md` etc.) und konsolidieren.
5. **Fallstudien-Seite** mit den bereits vorhandenen Logos und kurzen Erfolgsgeschichten.
6. **Kanal-Funktionstrennung** prominent auf der Startseite, nicht versteckt auf `contribute.md`.

---

*Review erstellt aus den Markdown-Quellen, ohne Änderungen am Verzeichnis. Bewusst aus der Perspektive eines Erstbesuchers verfasst, der die Website ohne Vorwissen liest.*
