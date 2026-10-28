---
name: app-content
description: Use for any content work in this app - researching, writing, extending, correcting or reviewing its competencies, chapters, pages, rounds, questions, exercises, figures, terms or sources. This app's own content decisions; they take precedence over the generic lernapps content skills. Load it before you change any content.
---

# Content guide of this app

## Curriculum

Kein Lehrplan. Die App stimmt auf einen naturwissenschaftlichen Schülerwettbewerb für die Klassen 5 und 6 ein
(Mensch und Natur, Aufgaben mit drei Antworten, eine richtig, 45 Fragen in 45 Minuten, Punkte +3, −1, 0 bei 45 Punkten
Start). Umfang sind die Themenbereiche und der Fragestil des Materials des Creators (Hefte früherer Jahre). Das Material
bleibt lokal, nie in der App; alle Fragen sind neu geschrieben.

## Competencies

- Start: Ich kann die Punkte eines Wettbewerbsbogens berechnen (`start/so-geht-heureka`, `start-punkte-berechnen`).
  Ich kann beurteilen, wann sich Raten lohnt (`start-raten-wahr-falsch`, `start-ausschliessen`).
  Ich kann meinen Stand je Bereich einschätzen (`start/selbsteinschaetzung`, Ids `se-…`).
- Denken: Ich kann in „Welche Aussage ist falsch?“ jede Aussage einzeln prüfen (`denken/falsche-aussage`).
  Ich kann Antworten durch Schätzen und Ausschließen eingrenzen (`denken/schaetzen-ausschliessen`).
- Mensch und Tier: Ich kann Tiergruppen und Jungtiere zuordnen und Besonderheiten unterscheiden
  (`tiere-und-ihre-jungen`). Ich kann Bestandteile und Aufgaben von Blut, Immunsystem, Nährstoffen und Hormonen nennen
  (`koerper-und-blut`). Ich kann den Weg der Luft, die Aufgaben von Haut und Niere und die Reizleitung erklären
  (`atmen-haut-sinne`).
- Natur und Umwelt: `sonne-erde-mond`, `planeten-weltall`, `wasser-wetter`, `natur-schuetzen`, je mit Aufgaben `<seite>-…`.
- Technik und Fortschritt: `internet-computer`, `energie-strom`, `stoffe-messgeraete`, Aufgaben `internet-…`, `energie-…`,
  `stoffe-…`.

## Content structure

Jede Themenseite hat die Abschnitte `ueberblick`, `wissen` (Definitionen, Tabellen, ein `example` mit dem Denkweg) und
`uebung` mit rund sechs Aufgaben, darunter immer eine Frage „Welche Aussage ist falsch?“ mit einfacher Verneinung. Die
Seiten der Kapitel „Start“ und „Denken“ haben dieselben Abschnitte, `selbsteinschaetzung` hat `uebung` vor `auswertung`.

## Terminology

Anrede „du“, kurze Sätze, Klasse 5 und 6. Begriffe stehen als `definition`. Punkte immer „+3“, „−1“, „0“.
Das Startkapital heißt „Startkapital“.

## Exercise patterns

- Wettbewerbsfrage: `single-choice`, genau drei Optionen, jede Option mit `info`; Beispiel `falsch-spinnen`
  in `src/denken/falsche-aussage.yaml`.
- Aussage prüfen: `true-false` mit Grund (`falsch-signalwort`).
- Zuordnen: `matching` mit `distractors`; an Abbildungen mit `pairsFrom: material`.
- Reihenfolge: `ordering` nur bei fester Folge (Planeten, Weg der Luft, Weg des Windstroms).
- Schätzen: `number` mit `tolerance` und `mistakes` (`schaetzen-everest`).
- Punkte rechnen: `generated` mit `mistakes` (`start-punkte-berechnen`).
- Die Selbsteinschätzung übernimmt zwölf Fragen der Themenseiten mit neuer Id `se-<id>` (Skript nicht Teil der App);
  ändert sich eine Frage, wird die Kopie mit geändert.

## Figures

Eigene SVG-Zeichnungen ohne Schrift in `src/images/` (`mt-atemwege.svg`, `nu-sonne-mond-erde.svg`, `te-windrad.svg`),
`source: eigene Zeichnung`, `licence: CC-BY-4.0`. In Übungen als `labelled-figure` mit Buchstaben und `legend: false`,
dazu ein `matching` mit `pairsFrom: material`. Die Zeichnung zeigt nie die Zuordnung.

## Sources

`sources` in `src/app.yaml` listet alle verlinkten Seiten (überwiegend deutsche Wikipedia, einzelne Klexikon und
Medienseiten). Jede Seite wurde beim Schreiben geöffnet und die Fakten daran geprüft; was keine Quelle belegt, steht
nicht in der App. Das Punktesystem (+3, −1, 0, Startkapital 45) stammt aus den Heften früherer Jahre und steht im Text
als „in den Heften der letzten Jahre“; die Rate-Rechnung ist eine eigene Rechnung. Das Material des Creators bleibt lokal.

## Adding a chapter or round

1. Ordner `src/<kapitel>/` mit `chapter.yaml`, Kapitel in `chapters` von `src/app.yaml` eintragen.
2. Seiten mit den Abschnitten `ueberblick`, `wissen`, `uebung`, in `pages` der `chapter.yaml` listen.
3. Fakten an geöffneten Quellen prüfen, Quellen in `sources` ergänzen.
4. `npm run build`, `npx lernapps check`, committen.

## Rules learned from mistakes

- Diese App wird über lernapps/practice eingereicht: eine Änderung ist ein neues ZIP im Issue; kein Push, kein Listing.
- Ein Doppelpunkt in einem unquotierten YAML-Wert bricht das Parsen: Titel mit Doppelpunkt in Anführungszeichen setzen.
- `sources` in `src/app.yaml` darf nicht leer sein.
