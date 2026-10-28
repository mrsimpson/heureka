---
# Read by the hooks, the review, the evals. Schema: @lernapps/tooling/guidance/plan-front-matter.v1.schema.json
# Keep all four keys.
# Archetype, null until Explore ends; then explainer, the only archetype of lernapps practice. Never another value.
archetype: explainer
# Current phase. Allowed values: explore, plan, code, commit. Change the value line below, never this comment.
phase: code
# prePushFailures: written by the pre-push hook. Never change it.
prePushFailures: 0
# failedChecks: failed rules and runs, written by lernapps check and the hooks. Never change it.
failedChecks: {}
---

# Plan: <occasion>, a learning app through lernapps practice

<!--
For you, the assistant. lernapps practice: the creator has an occasion (a class test, a cover lesson, …) and no app
of the catalog fits. You make a small explainer for it on this computer; the creator submits its src/ as a ZIP file
in an issue of lernapps/practice, and GitHub serves it for two weeks at https://lernapps.net/practice/i/<number>/.
1. Path: `.vibe/plans/01-<occasion>.md`, in a new, empty folder. A correction after the submission is no new plan:
   it is a task of Commit.
2. Read this plan before each step. One phase at a time, tasks in order.
3. Task done → tick `[x]` at once and move it to "Completed" of its phase. An unticked box counts as not done.
4. New task found → add it.
5. Each phase installs and names its skills. Install them when the phase begins, load a skill when its task comes, not
   before. Read it in full, from its file. Install no other skill: this app is not published through GitHub and not
   listed.
6. Checkpoint: stop, ask, wait for the creator's answer. A message sent before the question is no yes.
   Only a checkpoint waits. A phase's last box → set the next phase and go on in the same message.
7. At most 2 questions per message, one topic each. No questions inside drafts or lists.
8. Work locally, in this folder. Push nothing, create no repository, list nothing: the submission is the ZIP file.
9. Plan in the creator's language. Keep headings and front matter keys. Delete a comment once its part is filled.
10. Begin each reply to the creator with the phase in `phase:`, and at a checkpoint the word checkpoint:
    "**Plan · Checkpoint**", "**Code**". The creator always knows where you are.
11. You need a shell with Node 22.18 or newer, git and the network (github.com, raw.githubusercontent.com,
    codeload.github.com, registry.npmjs.org). Blocked → ask the creator to allow it, then run again.
-->

*Explore, Plan, Code, Commit.*

## Goal

Der Sohn (Klasse 5/6) stimmt sich auf den naturwissenschaftlichen Schülerwettbewerb „Heureka! Mensch und Natur“ ein. Danach kann er Aufgaben im Stil des Wettbewerbs in 45 Minuten angehen: Aussagen prüfen, falsche Antworten ausschließen, sinnvoll raten und Wissen aus Mensch und Tier, Natur und Umwelt sowie Technik und Fortschritt anwenden.

## Key decisions

- Archetyp explainer: die einzige Form von lernapps practice. Kein Timer und kein Spiel möglich; die Zeit übt der Sohn mit der Uhr auf dem Tisch (Vorschlag).
- Kein Lehrplan, sondern Wettbewerbsstil: Aufgaben mit drei Antworten, eine richtig, oft „Welche Aussage ist falsch?“ (Antwort des Creators).
- Alle Aufgaben sind neu geschrieben, im Stil und zu den Themen der Vorjahreshefte; keine Frage aus den Heften wird übernommen.
- Erst Denkwerkzeuge, dann Themen: eine Seite „So geht Heureka“ mit Wertung und Rate-Strategie, eine Seite „Falsche Aussage finden“ und eine „Schätzen und Ausschließen“, damit der Sohn die Technik des Wettbewerbs übt, nicht nur Wissen (Vorschlag).
- Rate-Rechnung als Übung: +3, −1, 0 bei drei Antworten heißt, Raten lohnt sich im Mittel (Erwartungswert +1/3 Punkt je Frage); bei zwei übrigen Antworten +1 (eigene Rechnung, aus den Regeln der Hefte).
- Selbsteinschätzung zuerst (12 Fragen quer durch alle drei Bereiche) mit Auswertung, die zu den Themenseiten verlinkt.
- Drei Themenkapitel wie im Heft; je 2 bis 3 Seiten, nur Themen, die in beiden Vorjahresheften vorkommen oder gut dazu passen (Vorschlag).
- Klassenstufe: Aufgaben für 5 und 6 gemischt (Vorschlag).
- Sprache: nur Deutsch (Vorschlag).

## Notes

- Anlass: Schülerwettbewerb „Heureka! Mensch und Natur“, Berlin, Klassenstufen 5 und 6, Herbst. Fach Naturwissenschaften, Berlin.
- Format des Wettbewerbs (Ausschreibung): 45 Fragen, je eine richtige von drei Antworten, 45 Minuten, Startkapital 45 Punkte, richtig +3, falsch −1, offen 0. Einzelarbeit ohne Hilfen. (Vorschlag: das Punktesystem als Übungsmodus abbilden.)
- Themen aus dem Material, 3 Bereiche zu je 15 Fragen:
  - Mensch und Tier: Tierfamilien und Jungtiernamen, Fortpflanzung und Besonderheiten von Wirbeltieren, Insekten und Verwandlung, Pinguine, Eisbären und Flamingos, Quallen; Blut, Immunsystem und Impfung, Nährstoffe und Vitamine, Mineralstoffe und Hormone, Niere, Haut, Lunge und Atmung, Knochen, Sinne und Nerven, Krankheitserreger (Viren, Bakterien).
  - Natur und Umwelt: Sonne, Erde, Mond, Sonnenfinsternis, Planeten und Reihenfolge, Komet, Meteoroiden, Galaxie, Weltraum; Wasser (Meerwasser, Löslichkeit, Eisberge); Wetter und Klimazonen, Wolken, Regenbogen, Wind; Ökosystem, Nachhaltigkeit, Treibhauseffekt, Müll und Abbauzeiten, Bäume und Pilze, Pflanzenfamilien.
  - Technik und Fortschritt: Internet, WLAN, IP-Adresse, QR-Code, Dateiformate, Spam, Künstliche Intelligenz, Hashtag, Software-Updates; Recycling, Metalle, Gentechnik und Klonen, Magnetismus, Windkraft, Elektromobilität, fossile Brennstoffe, Messgeräte (Barometer, Hygrometer), Drohnen.
- Abbildungen: nur das Logo der Hefte, ohne Bedeutung für den Stoff. Keine Figuren zum Nachbauen.
- Kein Lehrplan: Umfang sind die Themen und der Aufgabenstil der Hefte, nicht ein Schuljahr. Das Ziel ist Einstimmung auf den Wettbewerb durch ähnliche Knobelaufgaben (Wissen, Schlussfolgern, Ausschließen falscher Antworten).
- Quellen für Fakten: nicht geprüft. Jede Sachaussage wird in Plan an einer geöffneten Quelle geprüft; was keine Quelle klärt, geht an den Creator.
- Offen: Klassenstufe des Sohnes (Vorschlag: Aufgaben für 5 und 6).
- Das Material (PDF) bleibt lokal und kommt nicht in die App.

## Explore

<!--
- Find out the occasion, whether an app exists and what the material holds: that is the scope. Ask only what only the
  creator knows, in one message; decide the rest yourself and propose it in Plan.
- Stick to the scope: research only to explain the material and to check facts, never to find more to ask.
- Write no code, run no `create`.
- An answer counts only in the creator's words under "Answers". What you decided is a proposal, marked "(Vorschlag)".
- Skills: `lernapps-practice-explore`, `lernapps-practice-photos`, `lernapps-content-research`.
-->

### Tasks

_Alle Aufgaben von Explore sind erledigt, siehe „Completed“._

### Answers

<!-- The creator's answers, in their words. Keep the topics. -->

- Occasion: Vorbereitung auf den Schülerwettbewerb „Heureka! Mensch und Natur“ (Berlin, Oktober/November, Klassenstufen 5 und 6, 45 Minuten, 45 Fragen mit je drei Antworten, Einzelwettbewerb), für den Sohn des Creators.
- Learners: Naturwissenschaften (Mensch und Tier, Natur und Umwelt, Technik und Fortschritt); Klassenstufe 5 oder 6 (Vorschlag: Aufgaben für beide, wie die Ausschreibung).
- Material: Aufgabenhefte der Vorjahre 2024 und 2025 (PDF), alle drei Themenbereiche zählen.
- Changes: Kein Lehrplanbezug: Heureka ist ein naturwissenschaftlicher Wettbewerb, kein Schulstoff. Der Sohn soll auf den Wettbewerb eingestimmt werden und dafür ähnliche Knobelaufgaben bekommen.
  Vorschlag bestätigt („Passt“). Die Zeit ist nicht wichtig; es geht um die Inhalte und die Art, wie die Fragen gestellt sind.

### Completed

- [x] Install the skills of Explore in this folder:
      `npx --yes skills add lernapps/practice -y -s lernapps-practice-explore -s lernapps-practice-photos` and
      `npx --yes skills add lernapps/tooling -y -s lernapps-content-research`.
- [x] Load skill `lernapps-practice-explore`. In one message, as it says: ask the occasion, subject, school year,
      Land and the material; say what the creator must know before. Wait for the answer.
- [x] Search the catalog as the skill says. An app fits → give the creator its link and ask whether it is enough;
      yes → the plan ends here.
- [x] Load skill `lernapps-practice-photos`. Read the material as it says. Under "Notes": the topics, page by page;
      each figure of the material and how you redraw it.
- [x] Load skill `lernapps-content-research`. Every fact you are not sure of (numbers, dates, names, ways of
      counting): a source you opened, under "Notes". Open it now, not later. Only what no source you opened settles
      goes to the creator to check. Research only what explains the material; nothing beyond it.
- [x] Write the answers under "Answers" and the scope under "Notes": the topics of the material, nothing else.
- [x] Set `archetype: explainer` and `phase: plan`: change the value lines (`grep -E '^(archetype|phase):'` prints
      `archetype: explainer` and `phase: plan`). Tell the creator in one sentence that you now prepare the proposal;
      do not ask. Go on in the same message.

## Plan

<!--
- Decide the app and map it onto the explainer: chapters, pages, blocks, exercises, figures, components.
- No new questions. A gap → decide and mark it "(Vorschlag)". Stay within the scope of Explore.
- One proposal, confirmable in one read; the only checkpoint before the app is built. After the yes, work on your
  own until Commit.
- Skills: `lernapps-practice-plan`, `lernapps-exercise-patterns`, `lernapps-explainer-design`; and
  `lernapps-content-research`, loaded in Explore; reread it if it is no longer in view.
-->

### Tasks

- [x] **Checkpoint:** proposal. Brief and structured, as skill `lernapps-practice-plan` says: only what is special
      or conceptual, not page by page; your guesses ("(Vorschlag)") highlighted; the facts the creator should check.
      Ask for one yes or for changes. Stop and wait. Changes → change, write them under "Answers", show
      only what changed. No `create` before the yes.
- [x] Set `phase: code`: change the value line (`grep '^phase:'` prints `phase: code`).

### Content method

- **Seitenaufbau (alle Themenseiten):** Überblick, Wissen oder Denkweg (`definition`, `example`, ggf. `table`), Übung. Gleiche Abschnitte, feste ids.
- **Wettbewerbsfrage:** `single-choice`, drei Optionen, genau eine richtig; jede falsche Option mit Begründung im Feedback. „Welche Aussage ist falsch?“ ist eine Variante desselben Typs. Je Seite 3 bis 5 Fragen.
- **Wahr oder falsch mit Grund:** `true-false` für Aussagen aus dem Überblick, Grund im Feedback.
- **Zuordnen:** `matching` (Jungtier ↔ Elternteil, Planet ↔ Eigenschaft, Gerät ↔ Messgröße, Vitamin/Mineralstoff ↔ Aufgabe); Daten in `src/data/*.yaml`, jede Tatsache einmal.
- **Reihenfolge:** `ordering` für Planeten nach Abstand, Weg der Luft durch den Körper, Weg des Wassers beim Recycling; nur, wo die Folge fest ist.
- **Rechnen:** `generated` für die Punktewertung (richtig, falsch, offen → Punkte, Startkapital 45) mit typischen Fehlern („Du hast den Abzug vergessen“); `number` mit `mistakes` für Schätzfragen (Größenordnungen).
- **Beschriften:** `labelled-figure` mit eigener SVG-Zeichnung für Lunge und Kreislauf, Sonnenfinsternis (Sonne, Mond, Erde), Wasserkreislauf, Windrad; Beschriftungen als Buchstaben, dazu `matching` mit `pairsFrom: material`.
- **Selbsteinschätzung:** 12 `single-choice` quer durch den Stoff, Auswertung als `note`, die je nach Punktzahl auf Themenseiten verlinkt. Zählt der Sohn selbst.
- **Komponente:** keine. Alles geht mit Blöcken; ein Timer wäre nicht möglich.
- **Abbildungen:** eigene SVG-Zeichnungen (`source: eigene Zeichnung`, `licence: CC-BY-4.0`), schematisch und ohne Antwort in der Zeichnung.
- **Fakten:** jede Sachaussage wird beim Schreiben der Seite an einer geöffneten Quelle geprüft (NASA, Planet Schule, Wikipedia, serlo, Fachseiten); was keine Quelle klärt, kommt nicht in die App.


### Completed

- [x] `grep '^phase:'` prints `phase: plan`; else set it.
- [x] Install the skills of Plan: `npx --yes skills add lernapps/practice -y -s lernapps-practice-plan` and
      `npx --yes skills add lernapps/tooling -y -s lernapps-exercise-patterns -s lernapps-explainer-design`.
- [x] Load skills `lernapps-practice-plan`, `lernapps-exercise-patterns` and `lernapps-explainer-design`. Map the
      content as skill `lernapps-explainer-design` says: chapters and pages, with the pages skill
      `lernapps-practice-plan` names for the occasion.
- [x] Choose a pattern per topic as skill `lernapps-exercise-patterns` says. Write "Content method".
- [x] Each figure: what it shows, its labels as in the material, how you make it (generated image or SVG drawing,
      as skill `lernapps-practice-photos` says). Each component: what it shows and checks, and why no block fits.
- [x] Choose richer, interactive forms for this material, as skill `lernapps-practice-plan` says, and sketch them
      roughly.
- [x] Fill "Goal" and "Key decisions": the occasion and what learners can do afterwards; each decision with its
      reason, your own choices marked "(Vorschlag)".
- [x] The facts to check: each with its source (skill `lernapps-content-research`), or marked for the creator.
- [x] Write the Code tasks under "Code": one per page or component, with its content and exercises.

## Code

<!--
- Build the app from the explainer and the confirmed plan, in this folder. Work on your own.
- A check fails → skill `lernapps-cli`. Fix from the message; never bypass a check.
- Undecidable → choose, mark "(Vorschlag)" under "Key decisions", go on.
- Creator asks for a change → first say your reading in one sentence; never narrow it silently.
- Skills: `lernapps-cli`, `lernapps-explainer`, `lernapps-content-questions`, `lernapps-practice-photos` (the
  figures), and the app's content guide `app-content`.
-->

### Tasks

- [ ] `grep '^phase:'` prints `phase: code`; else set it.
- [ ] Install the skills of Code:
      `npx --yes skills add lernapps/tooling -y -s lernapps-cli -s lernapps-explainer -s lernapps-content-questions`.
- [ ] Load skill `lernapps-cli`. Create the app in this folder as it says, with
      `npx --yes github:lernapps/tooling#main create --archetype explainer`; then `git init`, `npm install`, the
      first commit. `create` keeps this plan and the skills. Never write the app by hand.
- [ ] Fill the content guide `.agents/skills/app-content/SKILL.md` from "Notes" and "Content method". Add under
      "Rules learned from mistakes" the line: "Diese App wird über lernapps/practice eingereicht: eine Änderung ist
      ein neues ZIP im Issue; kein Push, kein Listing." `grep -c "FILL IN" .agents/skills/app-content/SKILL.md`
      prints 0.
- [ ] Load skill `lernapps-explainer` and the content guide. Questions with options and feedback: also skill
      `lernapps-content-questions`.
- [ ] Replace the example chapter "Prozent" and the example component `ProzentFeld` with the planned content.
- [ ] Chapter „Start“: Seite „So geht Heureka“ (Ablauf, Wertung +3/−1/0, Rate-Rechnung, `generated` Punkte berechnen) und Selbsteinschätzung mit 12 Fragen und Auswertung.
- [ ] Chapter „Denken wie ein Forscher“: Seiten „Falsche Aussage finden“ (Signalwörter wie alle, immer, nur) und „Schätzen und Ausschließen“ (Größenordnungen, `number` mit `mistakes`).
- [ ] Chapter „Mensch und Tier“: Seiten „Tiere und ihre Jungen“ (Verwandlung, Warmblüter/Kaltblüter, Besonderheiten), „Körper und Blut“ (Blut, Immunsystem, Nährstoffe, Vitamine, Mineralstoffe), „Atmen, Haut und Sinne“ (Lunge, Haut, Niere, Nerven; `labelled-figure` Lunge).
- [ ] Chapter „Natur und Umwelt“: Seiten „Sonne, Erde und Mond“ (Sonnenfinsternis, `labelled-figure`), „Planeten und Weltall“ (`ordering`), „Wasser und Wetter“ (Löslichkeit, Eis, Wolken, Wind, Klimazonen), „Natur schützen“ (Ökosystem, Treibhauseffekt, Nachhaltigkeit, Müll).
- [ ] Chapter „Technik und Fortschritt“: Seiten „Internet und Computer“ (IP-Adresse, WLAN, Dateiformate, Spam, KI), „Energie und Strom“ (Windkraft, Elektroauto, fossile Brennstoffe; `labelled-figure` Windrad), „Stoffe und Messgeräte“ (Metalle, Recycling, Magnetfeld, Barometer, Hygrometer, Gentechnik).
- [ ] The figures: as skill `lernapps-practice-photos` says, in `src/images/`, with `source` and `licence`.
- [ ] `npm run build` and `npm run check` pass.
- [ ] The content guide matches what was built.
- [ ] Every box of Explore, Plan and Code ticked.
- [ ] Set `phase: commit`: change the value line (`grep '^phase:'` prints `phase: commit`).
      No checkpoint here: set it before you ask or report anything, then start Commit in the same message.

### Completed

## Commit

<!--
- Hand the app over: the creator submits the ZIP file of `src/` through the form of lernapps/practice. GitHub checks
  it, builds it and comments the address.
- Skill: `lernapps-practice-submit`.
-->

### Tasks

- [ ] `grep '^phase:'` prints `phase: commit`; else set it.
- [ ] Install the skill of Commit: `npx --yes skills add lernapps/practice -y -s lernapps-practice-submit`.
- [ ] Load skill `lernapps-practice-submit`. Show the creator every page of the built app as it says.
- [ ] **Checkpoint:** pages, and the declarations. The creator has seen every page; highlight what you decided in Code
      ("(Vorschlag)" under "Key decisions"); go through the three declarations of the form with them, as the skill
      says. Stop and wait for a yes. Changes → change, build, check,
      show the changed pages again.
- [ ] Make the ZIP file of `src/` as the skill says.
- [ ] **Checkpoint:** submit. Give the creator the ZIP file and the link to the form as the skill says; wait for the
      bot's comment.
- [ ] The comment names problems → correct them in `src/`, `npm run build` and `npm run check`, a new ZIP file; the
      creator attaches it as a comment of the issue. Repeat until the comment gives the address.
- [ ] The creator asks for a change after the address → add a task here; change, build, check and attach as above.
      Done only when the bot's new comment is there and the preview shows the change.
- [ ] **Checkpoint:** address. The comment gives the address: open it, confirm the app shows, give the creator the
      address and what the skill says about two weeks and the 👍.
- [ ] Fill the retrospective.

### Completed

## Retrospective

<!-- At the end of Commit. Facts, short, no names. Read by review and evals. -->

### Phases reached

<!-- Last phase completed, checkpoints passed. E.g. "commit; submitted, address received". -->

### Creator turns after the plan

<!-- Number of creator messages after the confirmation, topic of each. -->

### Where I had to guess

<!-- Each gap in plan, skills, messages or answers, and your choice. "None" if none. -->
