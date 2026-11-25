---
name: app-content
description: Use for any content work in this app - researching, writing, extending, correcting or reviewing its competencies, chapters, pages, rounds, questions, exercises, figures, terms or sources. This app's own content decisions; they take precedence over the generic lernapps content skills. Load it before you change any content.
---

# Content guide of this app

„Meinung sagen und begründen“: Explainer (Einheiten-App `subject: englisch`, Format 2, Sprache Deutsch, englische Beispiele und Lesestücke, britisches Englisch) über Meinung und Argumentation. Der **Argument-Burger** (Opinion – Reason – Example – Opinion) trägt die App; in Kapitel 2 werden Burger gestapelt und mit Verbindungswörtern gehalten, in Kapitel 3 wird er zur **Waage** (Pro und Contra, die Schlussfolgerung zeigt, wohin sie sich neigt). Auftrag: Issue lernapps/apps#487 (Epic lernapps/apps#489, Konventionen dort, Abschnitt 8 für Stufen 7-10). Umfang der ersten Version: alle 3 Kapitel, 12 Bausteine.

## Curriculum

Englisch als erste Fremdsprache, Stufe 7-8 (Kapitel 1 und 2) und 9-10 (Kapitel 3). Kein Lehrplan: Reihenfolge und Bausteine kommen aus der Lernlandkarte `https://lernapps.net/apps/map/englisch.json` (Fokus `competency`; Einheiten-App über die Stränge `wortschatz`, `texte`, `landeskunde`). Vorwissen aus anderen Explainern (Wiederholungsseiten `das-brauchst-du`): freizeit-hobbys (englisch-alltag), konjunktionen und that-saetze (englisch-saetze-verbinden), passiv (englisch-verbketten), kleidung-einkaufen (englisch-grossbritannien). Nicht hier: Freizeit als Situation (#477), Zeitungstexte und Information/Meinung (#486, dort auch Gliederung ausführlich), Stilmittel selbst (#483), Demokratie und Menschenrechte (#484), Politik und Religion. `text-gliedern` und `stilmittel` stehen knapp auf den Seiten `kommentar` und `werbung`.

## Competencies

Alle zwölf sind Lücken der Karte. Eine Seite je Baustein; Id = Karten-Id in `competencies:` der Seite (Wiederholungsseiten haben keine).

1. Kapitel `was-ich-denke` („Was ich mag und was ich denke“, 7-8)
   - `das-brauchst-du` (recap: englisch/freizeit-hobbys, englisch/konjunktionen, englisch/that-saetze)
   - `meinung-redemittel` → `was-ich-denke/meinung-sagen`: „Ich kann meine Meinung sagen, zustimmen und widersprechen (In my opinion …, I agree because …).“
   - `meinung-begruenden` → `was-ich-denke/meinung-begruenden` (Musterseite): „Ich kann in einem kurzen Text meine Meinung zu einem Thema sagen und mit Gründen und Beispielen stützen.“
   - `sport-musik` → `was-ich-denke/sport-musik`: „Ich kann über Sportarten, Musik und Fernsehen sprechen und sagen, was ich mag.“
   - `medien` → `was-ich-denke/medien`: „Ich kann über Medien und soziale Netzwerke sprechen, auch über ihre Chancen und Gefahren.“
2. Kapitel `argumente-verbinden` („Argumente verbinden“, 7-8)
   - `das-brauchst-du` (recap: englisch/passiv)
   - `verbindungswoerter-argumentieren` → `argumente-verbinden/verbindungswoerter`: „Ich kann Gedanken mit however, therefore, moreover und on the one hand … on the other hand verknüpfen.“
   - `umwelt` → `argumente-verbinden/umwelt`: „Ich kann über Umweltschutz sprechen, zum Beispiel über Müll, Recycling und Nachhaltigkeit.“
   - `technik-fortschritt` → `argumente-verbinden/technik-fortschritt`: „Ich kann über Erfindungen und technischen Fortschritt sprechen und sagen, wann und von wem etwas erfunden wurde (was invented by …).“
   - `leserbrief` → `argumente-verbinden/leserbrief`: „Ich kann einen Leserbrief schreiben, der sich auf einen Artikel bezieht.“
3. Kapitel `pro-und-contra` („Pro und contra“, 9-10)
   - `das-brauchst-du` (recap: englisch/kleidung-einkaufen)
   - `konsum-werbung` → `pro-und-contra/konsum-werbung`: „Ich kann über Konsum, Werbung und meine Rechte als Verbraucherin oder Verbraucher sprechen.“
   - `jugendkultur` → `pro-und-contra/jugendkultur`: „Ich kann Jugendkulturen früher und heute beschreiben, auch ihre Musik.“
   - `kommentar` → `pro-und-contra/kommentar`: „Ich kann einen argumentativen Text mit Pro und Contra, klarer Gliederung und Schlussfolgerung schreiben.“
   - `werbung` → `pro-und-contra/werbung`: „Ich kann untersuchen, mit welchen sprachlichen und bildlichen Mitteln eine Werbung wirken will.“

Die „Ich kann“-Sätze sind die der Karte (nicht umformulieren); eine Seite sagt im Abschnitt „Das kannst du danach“ in eigenen Worten, was man danach kann. Übungs-IDs: Präfix = Seite (`begruenden-…`), Diktat `<präfix>-hoeren`, Nachsprechen `<präfix>-nachsprechen`, offene Aufgabe `<präfix>-schreiben`.

## Content structure

- Pfad: `src/<kapitel>/chapter.yaml`, Seiten `src/<kapitel>/<seite>.yaml`, Bilder `src/images/`, Audio `src/audio/`.
- Jede Seite (außer Wiederholungsseiten) hat die Abschnitts-IDs `einstieg` (Vorwissen-Frage als erste leichte Aufgabe, „Das kannst du danach“), `lesen` (ein Lesestück mit Randglossar als `vocabulary`), `neu` (Burger-, Barometer- oder Waage-Bild, Merke-Kasten), `uebung` (mindestens vier Übungen leicht → schwer: Verstehen, Belegen mit Zeile, Meinung; je typischem Fehler eine Meldung), `anwenden` (`speaking-task` und `open-task` mit `points` und `solution`), `weiter`. Titel sagen, was der Abschnitt tut. Wiederholungsseiten haben nur Text und höchstens zwei Übungen.
- Länge: höchstens 350 Wörter Erklärtext (das Lesestück zählt nicht dazu), höchstens 4 Textblöcke hintereinander, Bild oder Übung in den ersten vier Blöcken, höchstens etwa 25 Items und 10 Übungen. Lesestück Stufe 7-8 etwa 150 bis 300 Wörter, Stufe 9-10 etwa 300 bis 600; höchstens ein Lesestück je Seite; Zeilen zum Belegen sind im Text nummeriert (`1`, `2` …).
- Szene Kapitel 1 und 2 (Stufe 7-8): Chats und kurze Dialoge, ein Bild nur wo es etwas zeigt. Wo: die **Meinungswand** im Klassenzimmer von Mr Hill (neuer Ort, nur für diese App): links das Poster „Argument-Burger“, rechts das **Meinungsbarometer** (Skala disagree – agree, Namenskärtchen der Kinder). Kapitel 2: die Schülerzeitung der Millbrook School (namenlos: „the school newspaper“, Name aus #486 offen). Wer: Sophie, Ellie, Peter, Amir, Mr Hill, Mrs Parker (Figuren wie in #470, Zeichnungen aus `millbrook-klassenzimmer.svg` von hello-millbrook). Kein Schulfest, kein Lagerraum, keine Ausstellung „Our Millbrook“, keine Geschichtenecke.
- Kapitel 3 (Stufe 9-10): keine erfundenen Kinder, auch Sophie kommt nicht vor; reale oder realistische Fälle mit Daten und Quellen, Ton sachlich; Du-Anrede. Heikle Themen neutral mit mehreren Sichtweisen, keine Wertung der Politik Erwachsener.
- Keine Figuren-Einführung im Seitentext: keine Altersangaben, keine Familie, kein Datum; die Startseite nennt nur Namen und Rollen.
- Anrede „du“.

## Terminology

- „Ausdruck“ (fester Ausdruck), nie „Wendung“. Fachbegriffe noun, verb, adjective, sentence, tense.
- Burger: **Opinion** (Meinung, oben und unten), **Reason** (Grund), **Example** (Beispiel); die Schichten heißen immer so. Waage: **Pro**, **Contra**, **conclusion** (Schlussfolgerung). **Meinungsbarometer**, **Meinungswand**. „Verbindungswörter“ (however, therefore, moreover).
- Wörtertabellen heißen „Klassenzimmer-Poster · …“ und stehen im `vocabulary`-Block (Konvention: Tabellen mit Wörtern in den Vokabelblock); Kapitel 3 ohne Klassenzimmer: „Wörterkasten · …“.
- Britisches Englisch (favourite, colour). Englische Aufgaben enthalten kein deutsches Wort.
- Aussprache: Lesehilfe in deutscher Annäherung nur für neue schwere Wörter (betonte Silbe groß), keine Lautschrift (IPA gehört zu #482); Hörtexte nur ganze Sätze.
- Wörter: Grundwortschatz A1/A2; jedes Wort, das eine Übung abfragt, steht vorher auf der Seite; Wörter außerhalb der Liste stehen im Randglossar der Seite und unten unter „Sources“.
- „Ding“ nur für Gegenstände; Menschen und Beziehungen haben keinen „Besitzer“.

## Exercise patterns

Aufbau leicht → schwer: wählen/zuordnen → ordnen → Lücke → schreiben mit Cue → Lesen und Belegen → Diktat und Nachsprechen → freie Aufgabe. Je Übung `mistakes` mit eigener Meldung je typischem Fehler; `hint` zeigt einen Weg, nennt aber die Lösung nicht; gleichwertige Antworten als Gruppe `(a|b)` im `target`; `form: { punctuation: ok }`.

- Redemittel-Fächer (`matching` Ausdruck ↔ Fach Meinung/Zustimmung/Widerspruch); Meinungsbarometer (`single-choice` mit `info` je Option).
- Burger bauen (`ordering` der vier Schichten), Schicht erkennen (`matching` Satz ↔ Schicht), fehlende Schicht (`single-choice`).
- Satz bilden (`language-task` write mit Cue, z. B. `cue: "I · agree · because · fun"`), Lücke und Auswahl (`language-task` gap/choice: however, therefore, moreover, since/for, interested in).
- Lesestück: Frage zum Text (`single-choice`), Beleg mit Zeilennummer (`multiple-choice` oder `single-choice`), Meinung (`open-task`).
- Kapitel 2: Passiv (was invented by) als `language-task` write; Leserbrief: Teile zuordnen (`matching`), Brief schreiben (`open-task`).
- Kapitel 3: Waage füllen (`matching` Argument ↔ Pro/Contra), Absätze ordnen (`ordering`), Werbemittel zuordnen (`matching` Beispiel ↔ Mittel ↔ Wirkung), argumentativer Text (`open-task` mit Punkten).
- Hören und schreiben (`language-task` mit `audio`) und Nachsprechen (`speaking-task`): je Seite drei ganze Sätze, die im Seitentext nicht vorkommen.
- `open-task`: immer `points` und eine Musterlösung; die App bewertet den Text nicht, die Kinder prüfen ihn an den Punkten. Keine Komponenten (`prefer-built-in-block`), keine Datendateien: Burger, Barometer, Waage sind Zeichnungen.
- Jede Seite hat eine andere Menge an Übungsarten (`explainer-page-variety`).
- Typische Fehler (jeweils `mistakes`): I am agree statt I agree; I am thinking that statt I think that; Meinung ohne Grund; Grund wiederholt die Meinung; „for example“ ohne Beispiel; however mit because verwechselt; therefore ohne Folge; I am interesting in statt interested in; since/for; was invent statt was invented; Leserbrief ohne Bezug zum Artikel; Seiten der Waage vermischt; neue Argumente im Schluss; Mittel und Wirkung verwechselt.

## Figures

- Eigene SVG-Zeichnungen in `src/images/`, `CC-BY-4.0`, Hintergrund #f4efe2, Schrift mindestens 16 im viewBox, Beschriftung innerhalb des `viewBox`; keine Fotos, keine Figuren aus Büchern, Filmen oder Marken. `alt` sagt, was die Figur zeigt, nie die Lösung; die Figur zeigt nie dieselben Wörter wie die Aufgabe darunter.
- Familien (Schichtfarben fest, in allen Bildern gleich): `burger-<seite>.svg` (vier Schichten von oben nach unten: Opinion #e8743b, Reason #2c6fd8, Example #138d75, Opinion #e8743b; gestapelt mit Verbindungsschild in Kapitel 2), `barometer-<seite>.svg` (Skala disagree – agree mit Namenskärtchen), `waage-<seite>.svg` (Kapitel 3: Pro #c0392b, Contra #2c6fd8, Neigung = conclusion, keine Figuren). Szenen `szene-<seite>.svg` mit Figuren als `<g id>` aus `millbrook-klassenzimmer.svg` von hello-millbrook, gleich gelassen (nur Kapitel 1 und 2, nur wo es etwas zeigt).
- Skizze: `.vibe/sketches/burger-waage-barometer.svg`; die SVG-Dateien in `src/images/` sind die Quelle.
- Gebaut (`src/images/`): Kapitel 1: `szene-meinung-begruenden`, `burger-meinung-begruenden`, `szene-meinung-sagen`, `barometer-meinung-sagen`, `poster-sport-musik`, `burger-sport-musik`, `barometer-medien`, `burger-medien`. Kapitel 2: `schild-verbindungswoerter` und `burger-verbindungswoerter` (zwei Burger mit Verbindungsschild), `muelleimer-umwelt`, `burger-umwelt`, `erfindungen-technik-fortschritt`, `satzbau-technik-fortschritt`, `zeitung-leserbrief`, `brief-leserbrief`. Kapitel 3 (ohne Figuren): `beleg-konsum-werbung` (Kassenbon eines erfundenen Ladens), `zeitleiste-jugendkultur`, `waage-kommentar-leer`, `waage-kommentar`, vier erfundene Anzeigen `anzeige-werbung-<name>` (erfundene Marken, keine echten), `rueckblick-werbung` (Burger, gestapelt, Waage). Die Zeichenskripte liegen nicht im Repository; die SVG-Dateien sind die Quelle. Neue Zeichnungen im gleichen Stil, Figuren aus `szene-meinung-begruenden.svg` kopieren.

## Built (Stand der ersten Version)

Seiten (Übungs-IDs: Präfix = Seite; Diktat `…-hoeren`, Nachsprechen `…-nachsprechen`, offene Aufgabe `…-schreiben`):
- `was-ich-denke`: `das-brauchst-du` (Wiederholung, brauchen-verbinden, brauchen-that), `meinung-sagen` (sagen-start, -lesen, -beleg, -faecher, -luecken, -barometer, -satz), `meinung-begruenden` (begruenden-start, -lesen, -beleg, -schichten, -fehlt, -ordnen, -satz), `sport-musik` (sport-start, -lesen, -beleg, -verben, -ing, -burger, -satz), `medien` (medien-start, -lesen, -zeilen, -woerter, -praeposition, -satz).
- `argumente-verbinden`: `das-brauchst-du` (Wiederholung passiv, passiv-wahl, passiv-luecke; kein Link auf eine App, weil keine App `passiv` übt), `verbindungswoerter` (verbinden-start, -lesen, -beleg, -zuordnen, -waehlen, -ordnen, -satz), `umwelt` (umwelt-start, -wahr, -lesen, -beleg, -3r, -woerter, -satz), `technik-fortschritt` (technik-start, -lesen, -jahr, -zuordnen, -luecke, -passiv), `leserbrief` (brief-start, -lesen, -beleg, -teile, -bezug, -verbinden, -ordnen).
- `pro-und-contra`: `das-brauchst-du` (Wiederholung kleidung-einkaufen, kleidung-situationen, kleidung-schreiben), `konsum-werbung` (konsum-start, -lesen, -beleg, -rechte, -woerter, -menge, -procontra), `jugendkultur` (jugend-start, -lesen, -beleg, -zeit, -beschreiben, -procontra), `kommentar` (kommentar-start, -lesen, -beleg, -waage, -ordnen, -verbinden, -schluss, -fehler), `werbung` (werbung-start, -lesen, -beleg, -mittel, -wirkung, -frage, -untersuchen).
- Audio: alle Hörsätze stehen in `.agents/skills/app-content/scripts/audio-texte.json` (Datei → Satz, 72 Einträge, je Seite drei Diktat- und drei Nachsprechsätze, die Wiederholungsseiten keine). Prüfskript: `python3 -I .agents/skills/app-content/scripts/pruefen.py` (Hörsätze gegen den Text derselben Seite, Wörter gegen die Liste der Karte; Meldungen zu deutschen Wörtern in englischen Feldern sind Rauschen).
- Selbsteinschätzung (`selfAssessment` je `chapter.yaml`): zwei Übungen je Seite, die ohne den Text verständlich sind: `was-ich-denke` sagen-faecher, sagen-luecken · begruenden-schichten, begruenden-fehlt · sport-verben, sport-ing · medien-woerter, medien-praeposition; `argumente-verbinden` verbinden-zuordnen, -waehlen · umwelt-3r, -woerter · technik-zuordnen, -luecke · brief-teile, -verbinden; `pro-und-contra` konsum-woerter, -procontra · jugend-zeit, -procontra · kommentar-waage, -verbinden · werbung-mittel, -wirkung. Offene Aufgaben, Diktat, Sprechen und Übungen zum Lesestück sind nicht dabei.
- Lesestücke: Kapitel 1 und 2 150 bis 300 Wörter; in Kapitel 3 300 bis 600 Wörter (Konvention §8). Dort schlägt der Hinweis `explainer-text-load` an, weil das Lesestück als zu lesender Text zählt; das ist gewollt (guess).
- Belegen: Kapitel 1 und 2 über Zeilennummern, in Kapitel 3 über Absatznummern.

## Sources

Karte `https://lernapps.net/apps/map/englisch.json` und die Baustein-Seiten `https://lernapps.net/apps/map/englisch/c/<id>/`; Grundwortschatz `https://lernapps.net/apps/map/englisch/grundwortschatz/` (A1/A2). Der Argument-Burger, die Waage und das Meinungsbarometer sind Unterrichtsbilder aus dem Auftrag (Issue #487); es wird keine Quelle zitiert und kein Satz übernommen. Alle Lesestücke, Dialoge, Chats, Leserbriefe, Anzeigen und Übungssätze sind eigene Texte (CC BY 4.0); Fakten stammen aus geöffneten Quellen (Stand 2026-11-24, Wikipedia CC BY-SA: nur Fakten, keine Sätze): „Mod (subculture)“, „Punk subculture“, „Plastic pollution“ (Zusammenfassungen geöffnet). Weitere Quellen (alle geöffnet am 2026-11-24, nur Fakten, keine Sätze; Seite und Stand der Lizenz: Wikipedia CC BY-SA 4.0, gov.uk Open Government Licence v3.0):
- `umwelt`: en.wikipedia.org „Plastic pollution“ (Schätzung: etwa 8,3 Mrd. Tonnen Plastik hergestellt bis 2018, davon etwa 6,3 Mrd. Tonnen Abfall, davon etwa 9 % recycelt; Plastik zerfällt langsam), „Recycling“ (Aluminium aus Altmaterial braucht etwa 5 % der Energie; reduce, reuse, recycle).
- `technik-fortschritt`: „World Wide Web“ (Tim Berners-Lee bei CERN, Vorschlag 1989, im Internet allgemein zugänglich seit 23.08.1991, Code am 30.04.1993 freigegeben), „Paper“ (Papier in China seit mindestens dem Jahr 105, Cai Lun zugeschrieben; Entfärben von Altpapier 1774, Justus Claproth), „Bicycle“ (erstes Kettenmodell um 1885). gov.uk-Seiten zu diesen Themen antworteten mit 404; nichts davon übernommen.
- `konsum-werbung`: gov.uk „Accepting returns and giving refunds: the law“ (`https://www.gov.uk/accepting-returns-and-giving-refunds`; Rechte beim Einkauf, Reparatur oder Ersatz, Belege; aus Käufersicht umgeschrieben; „30 days“ steht dort nicht und fehlt auf der Seite), „Consumer rights“ (nur gelesen); en.wikipedia.org „Fast fashion“ (36 % der Käufe von Kleidung weltweit 2026 nach einem Marktbericht, den Wikipedia zitiert; 60 bis 70 Mio. Beschäftigte nur als Schätzung, die Wikipedia aus einem Blog übernimmt; ein Lkw Textilien je Sekunde nach UNEP; 2 bis 8 % der Treibhausgase als Schätzung; Emissionen etwa halbiert nur nach einer Ökobilanz von Polyester- und Baumwoll-T-Shirts bei längerer Nutzung; Social-Media-Werbung der Marken; Zahlen jeweils mit der dort genannten Zuschreibung. gov.uk: Rückgabe bei Fehler, Ausnahme bei bekanntem Fehler, 14 Tage online).
- `jugendkultur`: „Mod (subculture)“, „Punk subculture“, „Grime music“ (Jahrzehnte, Kleidung, Musik, Ideen; keine Titel und Bandnamen); „Hip-hop“ nur in der Musterlösung von `jugend-schreiben`.
- `kommentar`: gov.uk „Mobile phones in schools“ (Leitfaden der englischen Regierung, Stand 2026-06-29; Standard handyfreie Schule, National Behaviour Survey 2024/25: 58 % der Schüler weiterführender Schulen berichten von Handynutzung ohne Erlaubnis in mindestens einigen Stunden (misst unerlaubte Nutzung, nicht Ablenkung), zitiert aus Ofcom 2025: 31 % der 8- bis 17-Jährigen erlebten „nasty or hurtful“ über Kommunikationstechnik; Ofcom selbst war nicht erreichbar), Wikipedia „Mobile phone use in schools“ (Argumente für und gegen Verbote; Anteil der Länder mit Verbot nach UNESCO-Monitoring 23 % (2023), 40 % (2024), 58 % (2026); Studie im Quarterly Journal of Economics 2026 zu abschließbaren Handyhüllen („Lockable Pouches“), begrenzte Wirkung auf Wohlbefinden und Lernergebnisse; Studie von 2017 mit etwa 100 Studierenden einer britischen Universität: 45 % sehen Handys im Unterricht als Hilfe fürs Lernen). Die zwei 58 % im Text sind verschiedene Zahlen (Länder, Schüler).
- `werbung`: Wikipedia „Advertising“ (Stand 2026-11-19: Ausgaben 2025 über eine Billion US-Dollar, 2024 59,4 % digital und 24,9 % Fernsehen, erster Werbespruch 1859, Aufgabe der Werbung zu informieren, Werbegeld und kostenlose Angebote, Kritik und Regeln); alle Anzeigen, Produkte und Marken sind erfunden (Rovix, Glowly, Fizzlo, Pocketvolt u. a.).
Nicht geprüft und nicht benutzt: UNESCO (403) und Ofcom (403) direkt; Gutenberg. UNESCO und Ofcom waren nicht erreichbar (403): Zahlen von dort nur, wenn eine erreichbare Quelle sie belegt. Nicht geprüft und nicht benutzt: alles, was hier nicht steht. Audio: KI-Stimme `bf_emma` (britisch, weiblich), mit Skill `lernapps-audio` erzeugt und als KI-generiert markiert.

## Hörliste (Sätze, die die Ersteller:in gezielt abhört)

Hörsätze bleiben natürlich: kein Name und kein Wort wird nur wegen des Klangs angehängt. `regen_audio.py` schneidet das Ausklingen ab; Sätze, die auf ein einsilbiges Wort enden, stehen hier zum gezielten Abhören (Orchestrator-Session in der Rolle der Ersteller:in hat das Hörurteil zur Musterseite bestätigt; der Rest steht aus):
- „I think the new gym is great.“, „You are right, the bus is always late.“, „I disagree, because the room is too small.“, „Do you agree with me?“, „That is a good point.“ (`meinung-sagen`)
- „I enjoy watching a good series after school.“, „What is your favourite sport?“, „Do you like this song?“, „What kind of music do you like?“, „I post a photo once a week.“ (`sport-musik`, `medien`)
- „Our town has a new recycling centre.“ (`umwelt`), „We used to play outside after school.“ (`jugendkultur`), „Can I return this jacket if it is too small?“, „Could you check the label, please?“ (`konsum-werbung`/Recap), „Moreover, many pupils use their phones to learn new things.“, „In conclusion, we should try it for one month.“ (`kommentar`), „Think about the people the advert wants to reach.“ (`werbung`)
- Neue Sätze der Korrekturrunde mit einsilbigem Ende (`argumente-verbinden`): „… kind and funny.“, „… a lot of work.“, „… I do not agree.“, „Many pupils answered our question.“
- Der Fehllaut-Schnitt (`valley_cut`) hat bei einigen Sätzen 65 bis 85 ms entfernt (zum Beispiel „Moreover, many pupils …“, „Therefore the school …“, „It is better to buy fewer clothes and wear them longer“); gezielt auf angeschnittene Endsilben abhören. Alle 72 Sätze: `.agents/skills/app-content/scripts/audio-texte.json`.

## Adding a chapter or round

1. Baustein auf der Karte wählen; die Voraussetzungen müssen auf früheren Seiten stehen oder eine Wiederholungsseite bekommen.
2. Seite `src/<kapitel>/<seite>.yaml` mit den Abschnitten `einstieg`, `lesen`, `neu`, `uebung`, `anwenden`, `weiter` anlegen (Muster: `was-ich-denke/meinung-begruenden.yaml`), in `chapter.yaml` eintragen, Competency-Id setzen.
3. Lesestück als eigener Text nach Fakten, Quellen hier unter „Sources“; Zeichnungen aus den Familien oben im gleichen Stil.
4. Übungen aus den Mustern oben, je mit `mistakes` und `hint`; 2 bis 3 davon in `selfAssessment` des Kapitels (Skill `lernapps-explainer-self-assessment`).
5. Hörtexte: `src/audio/<satz>.mp3` mit `regen_audio.py` (Skill `lernapps-audio`), je Seite drei Diktat- und drei Nachsprechsätze, nicht zwischen Seiten wiederholen; Sätze mit einsilbigem Ende in die Hörliste.
6. Wörter gegen den Grundwortschatz, Hörsätze gegen den Text derselben Seite prüfen (Prüfskript), `npx --no -- lernapps check`, committen.

## Rules learned from mistakes

Aus den Vorgängern (#470 bis #482) und der Konvention (Abschnitte 7 und 8):
- Jede Übung fragt nur Wörter ab, die vorher auf der Seite stehen; eine Tabelle, die eine Übung beantwortet, steht nicht direkt darüber; Poster, Merke, Einstieg und Bild nennen andere Beispielsätze und Wörter als die Übungen darunter.
- Englische Aufgaben enthalten kein deutsches Wort; der Cue ist englisch, der deutsche Hinweis steht in `source` oder in der Aufgabe.
- Mit `(a|b)` gleichwertige richtige Antworten zulassen; Auswahlaufgaben zur Großschreibung zeigen alle Optionen gleich geschrieben.
- Audio: das Ausklingen am Satzende abschneiden (`regen_audio.py`), keine Namen nur für den Klang anhängen; Diktat und Nachsprechen bringen neue Sätze: kein Hörsatz steht wörtlich oder fast wörtlich im Seitentext oder in einer anderen Übung derselben Seite.
- Bilder: Beschriftung im `viewBox`; Bildunterschrift nennt, wer wer ist; das `alt` verrät nie die Lösung.
- Als Auswahl nur echte Lernerfehler, keine Unwörter; jeder Distraktor und jedes typische Fehlerbild eine eigene Meldung; ein Einstiegs-`single-choice` hat mindestens drei Optionen; Optionstexte enden ohne Punkt.
- Eine Auswahl-Übung (`mode: choice`) braucht einen deutschen Satz (`source`) als Start.
- Höchstens eine kurze Wörtertabelle (Vokabelblock) je Seite; Seiten mit mehr als etwa 25 Items oder 10 Übungen kürzen.
- `lernapps check` zählt Texte, Optionen, Infos und Meldungen zusammen (höchstens 350 Wörter): Meldungen knapp halten.
- Ein Doppelpunkt in einem Hinweis, einer Meldung oder einer `explanation` lässt das YAML scheitern: vermeiden oder in Anführungszeichen setzen.
- Offene Aufgaben: immer `points` und Musterlösung mit dem Hinweis, dass die App den Text nicht bewertet; die Musterlösung hat andere Figuren und Themen als das Lesestück.
- Die `competencies:` jeder Seite sind Karten-Ids; Wiederholungsseiten (`recap`) haben keine.
- Bekannte Eigenheiten der Vorlage: `ordering` zeigt Auswahlfelder statt Karten, `accepted` einer Sprach-Aufgabe wirkt nicht (Gruppen `(a|b)`), im Modus `choice` zeigt die App `mistakes` nicht, `punctuation: hint` meldet bei richtiger Antwort „Achte auf die Satzzeichen“ (darum `punctuation: ok`).
- Keine Figuren-Einführung im Seitentext (keine Altersangaben, keine Familie, kein Datum); die Startseite nennt nur Namen und Rollen.
- Keine Sätze aus fremden Texten; jede Faktenangabe steht mit geöffneter Quelle unter „Sources“.
