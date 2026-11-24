---
# Read by the hooks, the review, the evals. Schema: @lernapps/tooling/guidance/plan-front-matter.v1.schema.json
# Written by `lernapps plan` and the hooks. Never change a key or a value by hand.
# Archetype, null until chosen in Explore. Allowed values: explainer, interactive, quiz.
archetype: explainer
# Current phase. Allowed values: explore, plan, code, commit.
phase: explore
# prePushFailures: failed pre-push runs, written by the hook.
prePushFailures: 0
# failedChecks: failed rules and runs, written by lernapps check and the hooks.
failedChecks: {}
---

# Plan: englisch-meinung, first version

<!--
For you, the assistant. The process is in AGENTS.md; this plan holds the method.
- `npx --no -- lernapps plan next` prints the task to do now, `plan done` ticks it and prints the next one.
- You write only below Goal, Key decisions, Notes, Answers, Entry draft, Content method and Retrospective, in the
  creator's language. Delete the comment of a section once the section is filled.
- Work on the branch `work`, locally: push nothing before Commit.
-->

*Started 2026-11-24. Explore, Plan, Code, Commit.*

## Goal

Jugendliche lernen, zu Themen aus ihrem Leben (Musik, Medien, Umwelt, Technik, Konsum) ihre Meinung auf Englisch zu sagen, zu begründen und in einem Text Argumente dafür und dagegen abzuwägen. Der Argument-Burger (Opinion – Reason – Example – Opinion) trägt die App; in Kapitel 3 wird er zur Waage (Pro und Contra).

## Key decisions

- Archetyp: explainer, Einheiten-App `subject: englisch` (Format 2, Fokus `competency`). Grund: Die Lernenden brauchen Erklärungen, Lesestücke und Bilder (Burger, Waage), dazwischen Übungen; ein Quiz erklärt nicht, ein interactive-Spiel brauchen wir nicht.
- Sprache: nur Deutsch (Erklärtexte), englische Beispiele und Lesestücke, britisches Englisch (Auftrag der Orchestrator-Session, Konvention der Reihe).
- Kapitelzuschnitt wie im Auftrag (3 Kapitel, 12 Bausteine, je eine Seite) plus je Kapitel eine Wiederholungsseite „Das brauchst du hier“ für Bausteine anderer Explainer.
- Hauptfigur Sophie in Kapitel 1 und 2 (Stufe 7-8, Chats und kurze Dialoge, ein Bild nur wo es etwas zeigt); in Kapitel 3 (Stufe 9-10) keine erfundenen Kinder, reale Fälle mit Daten und Quellen (guess: Sophie kommt dort nicht vor; Konvention §2 verbietet erfundene Kinder).
- Kein Alter, keine Familie, kein Datum der Figuren im Seitentext; die Startseite nennt nur Namen und Rollen.
- Ort für Kapitel 1: die „Meinungswand“ im Klassenzimmer von Mr Hill mit dem Meinungsbarometer (Skala agree – disagree, Namenskärtchen) und dem Argument-Burger als Poster. Neuer Ort, nur für diesen Explainer (guess; muss in den Konventionen als Kommentar eingetragen werden).
- Kapitel 2: Die Schülerzeitung der Millbrook School (aus #486) nimmt den Leserbrief auf; ihr Name bleibt offen („the school newspaper“), damit #486 nicht widersprochen wird (guess).
- Look and feel: fixed by the archetype.

## Notes

**Fach/Strang:** `subject: englisch`, Einheiten-App (Karte `https://lernapps.net/apps/map/englisch.json`, `explainerFocus: competency`); Stränge `wortschatz`, `texte`, `landeskunde`. Kein Lehrplan nötig (Auftrag und Karte geben Bausteine und Ordnung).

**Bausteine nach Kapitel (Karten-Ids, Reihenfolge nach `requires`, eine Seite je Baustein):**
1. `was-ich-denke` (Stufe 7-8): Wiederholungsseite `das-brauchst-du` (recap: `freizeit-hobbys` aus englisch-alltag, `konjunktionen` und `that-saetze` aus englisch-saetze-verbinden) · `meinung-redemittel` (Redemittel für die Meinung) · `meinung-begruenden` (Meinung begründen, der Argument-Burger) · `sport-musik` · `medien`.
2. `argumente-verbinden` (7-8): Wiederholungsseite (recap: `passiv`) · `verbindungswoerter-argumentieren` · `umwelt` · `technik-fortschritt` · `leserbrief`.
3. `pro-und-contra` (9-10): Wiederholungsseite (recap: `kleidung-einkaufen` aus englisch-grossbritannien; `text-gliedern` und `stilmittel` siehe Lücken) · `konsum-werbung` · `jugendkultur` · `kommentar` (Argumentativer Text, Waage) · `werbung` (Werbung analysieren).
Alle zwölf sind Lücken der Karte (`practisedBy` leer).

**Lücken und Befunde zur Karte (an den Orchestrator, nicht selbst ändern):** (a) `passiv` (7-8, Voraussetzung von `technik-fortschritt`) wird von keiner App geübt: Inkrement von #480 steht aus; es gibt keine App, auf die die Wiederholungsseite verweisen könnte. Vorschlag: kurze Wiederholungsseite mit dem festen Muster „was invented by …“. (b) `text-gliedern` (7-8, Voraussetzung von `kommentar`) und `stilmittel` (9-10, Voraussetzung von `werbung`, aus #483) sind ebenfalls ungeübt/unfertig; ihre Wiederholung am Kapitelanfang bleibt ohne Verweis auf eine App, die Seite erklärt sie knapp (Einleitung, Hauptteil, Schluss; repetition, rhetorical question, comparison). (c) `kleidung-einkaufen` und `freizeit-hobbys`, `that-saetze`, `konjunktionen` sind in Apps (#478, #477, #481) geübt: Wiederholungsseiten verlinken dorthin.

**Didaktik:** Der Argument-Burger (Opinion, Reason, Example, Opinion) wird in Kapitel 1 zur Kernfigur (Poster an der Meinungswand); in Kapitel 2 werden mehrere Burger gestapelt und mit Verbindungswörtern gehalten; in Kapitel 3 liegen zwei Burger als Pro und Contra auf einer Waage, die Schlussfolgerung zeigt, wohin sie sich neigt. Farben der Schichten bleiben in allen Bildern gleich. Themen aus dem Leben der Kinder (Musik, Serien, soziale Medien, Müll, Technik, Kleidung, Werbung); keine Politik, keine Religion, keine Streitthemen der Erwachsenen.

**Form:** jede Seite hat ein Lesestück als Kern (Stufe 7-8 etwa 150 bis 300 Wörter, Stufe 9-10 etwa 300 bis 600; Chats, Nachrichten, kurze Dialoge, ein Artikel, ein Interview), Vorwissen-Frage, Abschnitte mit Randglossar (Vokabelblock), Aufgaben Verstehen – Belegen – Meinung, dann Schreib- oder Sprechauftrag. Höchstens ein Lesestück je Seite, höchstens etwa 25 Items. Hörtexte nur als kurze ganze Sätze mit `bf_emma`.

**Üben (Muster, Kapitel `foreign-languages.md`):** Redemittel zuordnen und ergänzen (`language-task` choice/gap), Burger-Schichten ordnen (`ordering`), Schicht erkennen (`matching`), Satz schreiben mit Cue (`language-task` write), Verbindungswörter einsetzen (choice/gap), Lesestück verstehen (Fragen, Belegzeile `single-choice`), Diktat und Nachsprechen (`language-task` mit `audio`, `speaking-task`), offene Aufgabe mit Punkten und Musterlösung (die App bewertet den Text nicht), Werbung untersuchen (Zuordnung Mittel – Wirkung, Raster).

**Quellen (nur Fakten, keine Sätze; geöffnet am 2026-11-24):** Wikipedia „Mod (subculture)“, „Punk subculture“, „Plastic pollution“ (Zusammenfassungen abgerufen, CC BY-SA: nur Fakten); erreichbar und beim Bau zu öffnen: weitere Wikipedia-Artikel (Hip hop, Grime, World Wide Web, Fast fashion), gov.uk (Fakten zu Plastiktüten-Gebühr, Offene Regierungslizenz OGL), VOA Learning English (nur exklusiv von VOA erstellte Texte, Public Domain; Lizenzseite beim Bau öffnen), Wikinews (CC BY). Nicht erreichbar: UNESCO (403), Ofcom (403): Zahlen daraus nur, wenn eine erreichbare Quelle sie belegt. Jede Faktenangabe steht im Inhaltsführer unter „Sources“ mit Stand; was nicht geöffnet wurde, bleibt als „nicht geprüft“ draußen.

**Wörter:** Grundwortschatz A1/A2 (`https://lernapps.net/apps/map/englisch/grundwortschatz/`); Wörter außerhalb (opinion, argument, reason, advertisement …) im Vokabelblock mit Bedeutung; Liste im Inhaltsführer.

**Seiten und nicht geübte Voraussetzungen:** `meinung-redemittel` (needs: that-saetze → Wiederholungsseite); `meinung-begruenden` (meinung-redemittel, geübt); `sport-musik`, `medien` (freizeit-hobbys → Wiederholungsseite); `verbindungswoerter-argumentieren` (konjunktionen → Wiederholungsseite Kapitel 1, in Kapitel 2 nur Verweis); `umwelt` (keine); `technik-fortschritt` (passiv → Wiederholungsseite Kapitel 2); `leserbrief` (meinung-begruenden, geübt); `konsum-werbung` (kleidung-einkaufen → Wiederholungsseite Kapitel 3; umwelt geübt); `jugendkultur` (sport-musik, geübt); `kommentar` (meinung-begruenden, verbindungswoerter: geübt; text-gliedern: Lücke, auf der Seite erklärt); `werbung` (konsum-werbung geübt; stilmittel: Lücke, auf der Seite erklärt).

**Wie sie dorthin kommen (eine Zeile je Baustein) und welcher Fehler die Rückmeldung fängt:**
- `meinung-redemittel`: Sie sortieren Ausdrücke in drei Fächer (Meinung, Zustimmung, Widerspruch) und stellen ihren Namen auf dem Meinungsbarometer ein, bevor die Ausdrücke erklärt sind; Fehler: I am agree, I am thinking that, In my opinion I think (doppelt).
- `meinung-begruenden`: Sie bauen aus vier gemischten Schichten einen Burger und erkennen, welche Schicht fehlt (Grund fehlt, Beispiel fehlt); Fehler: Meinung ohne Grund, Grund = Meinung wiederholt, „for example“ ohne Beispiel.
- `sport-musik`: Sie lesen einen Chat über Lieblingsmusik und eine Serie, belegen Meinungen mit Zeile und bauen eigene Burger-Sätze; Fehler: like/likes, favourite vs. my favourite sport is, play/do/go bei Sportarten.
- `medien`: Sie lesen einen Chat über soziale Medien, trennen Chance und Gefahr und sagen ihre Meinung auf dem Barometer; Fehler: Wortschatz (post, follow, share), „I am interesting in“ statt interested, since/for.
- `verbindungswoerter-argumentieren`: Sie setzen however, therefore, moreover, on the one hand … on the other hand in Burger ein und ordnen Sätze nach der Beziehung (Gegensatz, Folge, Ergänzung); Fehler: however = because verwechselt, Komma nach however fehlt, but und however vermischt.
- `umwelt`: Sie lesen einen kurzen Artikel über Müll und Recycling (nur Fakten aus geöffneten Quellen) und sagen, was man tun kann; Fehler: should/must, recycle/reuse/reduce, much/many.
- `technik-fortschritt`: Sie ordnen Erfindungen Erfindern und Jahren zu und bilden Passivsätze (was invented by); Fehler: was invent, invented from, fehlendes was/were.
- `leserbrief`: Sie lesen einen Artikel und einen Leserbrief, finden Anrede, Bezug, Meinung mit Burger, Schluss und schreiben selbst einen; Fehler: Anrede (Dear Sir or Madam) und Schluss (Yours faithfully), Bezug zum Artikel fehlt.
- `konsum-werbung`: Sie lesen einen sachlichen Text mit Zahlen zu Kleidung und Konsum, sagen ihre Rechte als Käufer und äußern eine Meinung; Fehler: Wortschatz (refund, receipt, warranty), consumer vs. customer.
- `jugendkultur`: Sie lesen kurze Beschreibungen von Jugendkulturen früher und heute (Mods, Punks, Hip-Hop; Fakten aus Wikipedia) und beschreiben eine mit simple past und present; Fehler: Zeitform beim Früher/Heute, fashion/music-Wortschatz.
- `kommentar`: Sie legen Pro und Contra auf die Waage, ordnen Absätze (Einleitung, Hauptteil, Schluss) und schreiben die Schlussfolgerung; Fehler: Seiten vermischt, Schluss ohne Entscheidung, neue Argumente im Schluss.
- `werbung`: Sie untersuchen eine erfundene Werbung (Markenname erfunden, keine echte Marke) auf Mittel (slogan, rhetorical question, repetition, comparison) und Wirkung; Fehler: Mittel und Wirkung verwechselt, Information und Werbeversprechen vermischt.

**Umfang (Scope):** drin: Meinung sagen, zustimmen, widersprechen, begründen, Beispiele, Verbindungswörter, Leserbrief, argumentativer Text mit Pro und Contra, Wortschatz zu Sport, Musik, Fernsehen, Medien, Umwelt, Technik, Konsum, Werbung, Jugendkulturen. Draußen: Freizeit als Situation (#477), Zeitungstexte und Information/Meinung (#486), Stilmittel selbst (#483), Demokratie (#484), Politik und Religion, Bewertung freier Texte und der Aussprache durch die App. Daten: Zahlen nur aus geöffneten Quellen, Stand genannt; Sprache: Deutsch, englische Beispiele und Lesestücke (britisch).

## Explore

<!--
- Find out what the app teaches, for whom, how much and how it looks. Ask; write no code, run no `create`.
- An answer counts only in the creator's words under "Answers". At most 2 questions per message, one topic each.
-->

### Tasks

- [x] Check the start: the folder `.agents/skills/lernapps-app` exists (else stop and tell the creator that the folder
      was not started with `init`), and `git branch --show-current` prints `work` (else `git switch -c work`).
- [x] Load skill `lernapps-app`. Tell the creator in two sentences what a lernapps app is and where it will live: at
      their own address, free and public, and once listed as a copy on lernapps.net. Say that the technical part
      (GitHub) comes at the end and that you do it.
- [x] Interview: ask the topics "Goal" and "Learners" of "Answers".
- [x] Load skill `lernapps-map-assignment` and read the learning map of the subject as it says. The creator brings
      the content themselves (material, a word list, the pages): note under "Notes" which competencies of the map it
      covers. Else write the skill's assignment, with its story; the creator's yes answers the topics Content and
      Amount. A subject without a map: skip this task and say so.
- [x] Load skill `lernapps-exercise-patterns` and read its reference for the subject. Note under "Notes" how learners
      will practise what the goal names.
- [x] Choose the archetype as skill `lernapps-app` says: read the README of each archetype in question, then tell the
      creator in plain words what the chosen one can and cannot do. Write the archetype and its reason under "Key
      decisions".
- [x] Run `npx --no -- lernapps skills --archetype <name>` with the chosen archetype. It installs the archetype's
      skills and adds the archetype's tasks to this plan.
- [x] Load skill `lernapps-explainer-design`. An explainer has the look of the runtime: write "fixed by the
      archetype" under the topic "Look and feel" of "Answers".
- [x] Interview: ask every other topic of "Answers", in order. Leave out only a topic that an answer of the creator
      already covers, and note which answer. A topic nobody answered is asked once before you write an assumption
      with "(guess)".
- [x] Load skill `lernapps-content-research` and research as it says. Write under "Notes": the strand or subject, the
      competencies by chapter with their ids, the sources you opened.
- [x] Write under "Notes" which competency goes on which page and which pages form a chapter, as "Map the content" of
      skill `lernapps-explainer-design` says. Per page, name the prerequisites the app does not practise.
- [x] Write under "Notes", one line per competency: how learners get there (they derive it, they do not only read it
      off), and which misconception the feedback catches.
- [x] Write under "Notes" the scope: what is in, what is out and why, the data range (for example "all main-group
      elements", never a silent "1–20"), the languages.
- [ ] **Checkpoint:** research. Show in plain words: the strand or why none, the competencies by chapter, the didactic
      approach, the scope, every "(guess)", the sources and what is unchecked, the archetype and its reason. Stop and
      wait. Changes: change them, then ask again.

### Answers

<!-- The interview: per topic the creator's answer, in their words. Keep the topics. -->

- Goal: Auftrag lernapps/apps#487 (Orchestrator-Session in der Rolle der Ersteller:in): Meinung sagen, begründen, Argumente abwägen; Themen aus dem Leben der Jugendlichen, keine Streitthemen der Erwachsenen (Politik, Religion).
- Learners: Englisch als erste Fremdsprache, Stufe 7-8 (Kapitel 1-2) und 9-10 (Kapitel 3); Vorwissen: Explainer #471-#482 der Reihe, A1/A2-Wortschatz.
- Model and focus: die fertigen Vorgänger #481, #476, #479, #471 (Lesestück, Chat, Hörsätze); Schwerpunkt Lesestück und Schreiben mit Punkten.
- Hurdles: typische Fehler (Auftrag und Karte): I am agree statt I agree; „because“ ohne Grund (Meinung ohne Begründung); Meinung wiederholen statt Beispiel; however/therefore falsch gesetzt oder mit Komma-Spleiß; „I am interesting in“ statt interested in; Passiv (was invented by); Werbung für Information halten.
- Content: die Orchestrator-Session (Ersteller:in) liefert nur den Auftrag; Texte schreibt Claude aus Fakten mit geöffneten Quellen (Konvention §8), alle Lesestücke eigene Texte.
- Amount: ganzer Explainer, 3 Kapitel, 12 Bausteine plus Wiederholungsseiten (Auftrag der Startnachricht).
- Languages: German only (Erklärtexte), englische Beispiele.
- Look and feel: fixed by the archetype.
- Terms: Argument-Burger (Opinion, Reason, Example, Opinion), Waage (Pro, Contra, Schlussfolgerung), Meinungsbarometer, Verbindungswörter, „Ausdruck“ nie „Wendung“, Klassenzimmer-Poster (Wörter).
- Finding the app: Meinung auf Englisch sagen und begründen, Argumente, Pro und Contra, Leserbrief, Erörterung (englisch).

## Plan

<!--
- Map the confirmed content onto the archetype. No new content questions: a gap in the content goes back to Explore.
- The creator confirms the plan in one read. After the yes you work on your own.
-->

### Tasks

- [ ] Map the content as "Map the content" of skill `lernapps-explainer-design` says, and write the result under
      "Content method".
- [ ] Choose a pattern per competency as skill `lernapps-exercise-patterns` says, and add it to "Content method".
- [ ] Add to "Content method" one line per page, as "Engagement" of skill `lernapps-explainer-design` says: the
      opening task, the change of activity, the reward, the story.
- [ ] Add the tasks of Code, each one a piece of work that ends in a commit. First the pattern: one complete page or
      screen, `npx --no -- lernapps plan add --at pattern "<task>"`. Then the others, one call each:
      `npx --no -- lernapps plan add --at pages "<task>"`. Each task says what it builds and what it shows.
- [ ] Draw a sketch of each screen, component or interactive exercise: a static SVG or image, or the steps with what
      learners see after each. Keep the files in `.vibe/sketches/`.
- [ ] Show the creator, short: goal, competencies by chapter, the Code tasks, the sketches, and the content method in
      plain words (what learners see and do, what the app cannot do). At most 2 questions.
- [ ] **Checkpoint:** confirm the plan and the content method. Stop and wait for an explicit yes. Changes: change
      them, then ask again.

### Content method

<!-- One line each: the patterns and where; the figures and how they are made; the data files; each component, what it
checks and what it cannot; how a later agent adds a chapter. It becomes the content guide in Code. -->
<!-- An explainer: per figure, model and component its learning action in two to four sentences
(`explainer-representation-explained`); per page its prerequisites the app does not practise, and which get a recap
page, which a link. -->

## Code

<!--
- Build the app, locally on `work`, on your own. After each task: `plan done`, then one commit with the work and this
  plan. The hooks check each commit; a failing check is fixed from its message, as skill `lernapps-cli` says.
- What you cannot decide: choose, write it under "Key decisions" with "(guess)", go on.
- The creator asks for a change: say your reading in one sentence first, then change every place it holds for
  (`feedback-applied-everywhere`).
-->

### Tasks

- [ ] Load skill `lernapps-cli`. Create the app as its section "Create" says:
      `npx --no -- lernapps create --archetype explainer`.
- [ ] Fill the content guide `.agents/skills/app-content/SKILL.md` from "Notes" and "Content method": every heading,
      no "FILL IN" left. Commit it before any content.
- [ ] Load skill `lernapps-explainer`.
- [ ] Load skill `lernapps-content-questions`. Read whole, with your file tool:
      `.agents/skills/lernapps-explainer/references/blocks.md` and
      `.agents/skills/lernapps-explainer/references/exercises.md`. A foreign language: also
      `references/language-tasks.md` in the same folder. A component in the plan: also `references/components.md`.
- [ ] Decide whether the app needs `scope`, as "`scope`" in
      `.agents/skills/lernapps-explainer/references/structure.md` says. Write the choice under "Key decisions".
<!-- tasks: pattern: the one page or screen that is the pattern for the others -->
- [ ] **Checkpoint:** the pattern page. Load skill `lernapps-learner-check` and do its learner check on the page. Fix
      what it finds. Then show the creator the page and ask whether the others may follow it. Stop and wait. A
      change: change the pattern first.
<!-- tasks: pages: the other pages or screens, after the pattern -->
- [ ] Update the content guide so that it describes the app as built (`app-content-matches`).
- [ ] Run `npx --no -- lernapps check` until it passes.
- [ ] Look at every screen and state, at 360 px and on a desktop, as "Look at the app" of skill `lernapps-cli` says.
      Compare each with its sketch.
- [ ] Do the whole-app check of skill `lernapps-learner-check`. Fix what it finds and write under "Notes" what you
      fixed.

## Commit

<!--
- Put the app on GitHub, publish it with the creator's yes, then list it. A push to `main` publishes.
- Open the pull requests (to `main`, to the catalog) without asking: they publish nothing.
- The creator asked to stop before publishing (a trial): stop here and say so.
-->

### Tasks

- [ ] Load skill `lernapps-explainer-self-assessment`. Add the self-assessment as it says, or write under "Key
      decisions" why the app has none. Commit.
- [ ] Load skill `lernapps-github`. Set up the repository and Pages as it says. Ask for the repository's name and
      every click only the creator can make, in one message.
- [ ] Push `work`, open the preview pull request and see its checks to green, as skill `lernapps-github` says.
- [ ] **Checkpoint:** publish. Show what the app does and the preview link from the comment "Vorschau der App". Ask
      whether it may go online. Stop and wait for the yes.
- [ ] Load skill `lernapps-commit`. Publish as skill `lernapps-github` says: `work` into `main` as one squash commit,
      the run of `Pages` watched to its end.
- [ ] Open the address the job `deploy` printed and confirm that the app shows. Never use a derived address.
- [ ] Load skill `lernapps-listing`. Write the entry under "Entry draft" as it says, with the creator's answer to
      "Finding the app".
- [ ] Fill the retrospective.
- [ ] Commit this plan on `main` and push it: the listing check and the review read it there.
- [ ] **Checkpoint:** list. Open the listing pull request as skill `lernapps-listing` says, without asking first: the
      pull request is the review. See it to "bestanden", then show the creator the pull request and its result.
- [ ] If the plan changed since its last push, commit it on `main` and push again.

### Entry draft

<!-- YAML valid against the entry schema the listing skill names. Only known values, never invented. -->

```yaml
```

## Retrospective

<!-- At the end of Commit, before the listing pull request. Facts, short, no names. Read by review and evals. -->

### Phases reached

<!-- Last phase completed, checkpoints passed. E.g. "commit; confirmed, published". -->

### Creator turns after the plan

<!-- Number of creator messages after the confirmation, topic of each. Target: at most 3. -->

### Where I had to guess

<!-- Each gap in plan, skills, messages or answers, and your choice. "None" if none. -->
