# OPAL Schule meets LiaScript

> Online-Workshop für die Referent:innen der **Medienpädagogischen Zentren in Sachsen**
> **28. Mai 2026, 13:00–15:00 Uhr** · Prof. Dr. Sebastian Zug, Dr. André Dietrich (TU Bergakademie Freiberg)

## Worum geht es?

Lehrkräfte möchten **motivierende, interaktive Materialien** einsetzen — zugeschnitten auf ihre Lerngruppe — und sie mit Kolleg:innen teilen. In der Praxis ist das mühsam: jedes Format ein eigenes Werkzeug, kaum etwas lässt sich aus OPAL Schule herauslösen, und individuelle Anpassung wird zur Click-Marathon-Aufgabe.

Dieser Workshop präsentiert die Möglichkeiten von **[LiaScript](https://liascript.github.io)** — erweitertes Markdown, das Formeln, Quizze, eingebettete Simulationen und ausführbaren Code in *einer einzigen Textdatei* zusammenführt, die im Browser läuft und sich als echte OER teilen lässt.

Als roter Faden dient ein **realer Stoff aus OPAL Schule**: das Energie-Kapitel aus „BGY — 11. Klasse Physik". Sie sehen, wie aus dem Copy-Paste-Rohmaterial (zerfallene Formeln, Plaintext-Quizze) ein vollwertiger, interaktiver LiaScript-Kurs wird — und bauen diese Transformation selbst nach.

> **Sie sind Multiplikator:innen.** Alles, was Sie hier erleben, geben Sie später an Lehrkräfte an Ihren Schulen weiter. Achten Sie deshalb nicht nur auf das *Was*, sondern auch auf das *Wie würde ich das im Kollegium erklären*.

## Das weitere Vorgehen — vier Phasen

Der Workshop folgt der Choreografie **Erleben → Verstehen → Anwenden → Verbreiten**. Klicken Sie auf den jeweiligen Badge, um die Phase direkt im LiaScript-Player zu öffnen.

### Phase 1 · Erleben *(20 min)*

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/01_Erleben.md)

Sie durchlaufen einen **fertigen Demo-Kurs** zum Energiebegriff und probieren alle interaktiven Elemente selbst aus — Video, eingebettete PhET-Simulation, ausführbarer Python-Code, drei Quizformate mit Lösungswegen. Am Ende das Reveal: *woher* dieser Stoff stammt.

### Phase 2 · Verstehen *(15 min)*

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/02_Verstehen.md)

Kurzvortrag zum *Warum*: Welches Problem löst LiaScript für Lehrkräfte? Was sind die **drei technischen Kernideen** (Trennung von Inhalt und Darstellung, Interaktion als Teil der Sprache, der Browser als Laufzeitumgebung)? Und wie verträgt sich das mit OPAL Schule?

### Phase 3 · Anwenden *(45 min — das Herzstück)*

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/03_Anwenden_Vorlage.md)

**Hands-on.** Sie bekommen das Rohmaterial [`Energie.md`](original_material/Energie.md) als Skelett mit 15 progressiven Aufgaben und bauen daraus Schritt für Schritt selbst einen LiaScript-Kurs — von Formeln über Quizze bis zur eingebetteten Simulation.

- ✏️ **Arbeitsvorlage im LiveEditor:** [Phase 3 zum Bearbeiten öffnen](https://liascript.github.io/LiveEditor/?/show/file/https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/03_Anwenden_Vorlage.md) *(Quelltext + Rendering nebeneinander — sofort losschreiben, kein lokales Setup)*
- 👁 **Nur ansehen:** [Vorlage im Player](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/03_Anwenden_Vorlage.md)
- ✅ **Musterlösung:** [03_Anwenden_Loesung.md im Player](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/03_Anwenden_Loesung.md) *(erst nach dem eigenen Versuch ansehen)*
- 📄 **Cheatsheet zum Ausdrucken:** [cheatSheet/cheatsheet.pdf](cheatSheet/cheatsheet.pdf) — zweiseitige Syntax-Handreichung (Markdown + LiaScript). Jede Aufgabe verweist über `Cheatsheet-Abschnitt: …` auf die passende Karte.

### Phase 4 · Verbreiten *(20 min)*

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/04_Verbreiten.md)

Die zwei Fragen, die danach kommen: **Muss man das jedes Mal von Hand schreiben?** (KI als Co-Autorin — LiaSkill und Teaching-Agent) und **Wie kommt der Kurs zu den Lernenden?** (fünf Verbreitungswege, inklusive zweier OPAL-Schule-Pfade: nativ per ZIP-Upload und via SCORM mit Lernstand-Erfassung).

## So arbeiten Sie mit diesem Repository

- **Direkt loslegen:** Es ist keine Installation nötig. Jeder Phasen-Badge öffnet den Kurs im Browser. Mit den **Pfeiltasten** (← / →) blättern Sie, über das **🌐-Symbol** schalten Sie die Sprache um, über das **Lautsprecher-Symbol** das Vorlesen.
- **In den Quelltext schauen:** Jede Phase ist eine einzelne `.md`-Datei in diesem Repository — öffnen Sie sie, um zu sehen, wie wenig Text hinter der Interaktion steckt.
- **Selbst bearbeiten:** Ziehen Sie eine `.md`-Datei in den [LiveEditor](https://liascript.github.io/LiveEditor/), um sie live zu verändern und das Ergebnis sofort zu sehen.

## Dateien im Überblick

| Datei | Inhalt |
| ----- | ------ |
| [`01_Erleben.md`](01_Erleben.md) | Phase 1 — fertiger Demo-Kurs zum Energiebegriff |
| [`02_Verstehen.md`](02_Verstehen.md) | Phase 2 — Konzepte und Vision hinter LiaScript |
| [`03_Anwenden_Vorlage.md`](03_Anwenden_Vorlage.md) | Phase 3 — Arbeitsvorlage mit 15 Aufgaben |
| [`03_Anwenden_Loesung.md`](03_Anwenden_Loesung.md) | Phase 3 — kommentierte Musterlösung |
| [`cheatSheet/cheatsheet.tex`](cheatSheet/cheatsheet.tex) | Quelle der Syntax-Handreichung (PDF mit `pdflatex` bauen, 2× für korrekte Boxen) |
| [`04_Verbreiten.md`](04_Verbreiten.md) | Phase 4 — KI-Unterstützung, Verbreitung, OPAL-Integration |
| [`original_material/Energie.md`](original_material/Energie.md) | Das Roh-Material aus OPAL Schule (Copy-Paste-Stand) |

## Lizenz

Dieses Material steht unter [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.de) — Sie dürfen es als Grundlage für Ihre eigenen Fortbildungen verwenden, ergänzen, kürzen und weitergeben.

**Kontakt:** sebastian.zug@informatik.tu-freiberg.de · andre.dietrich@informatik.tu-freiberg.de
