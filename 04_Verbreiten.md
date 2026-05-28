<!--
author:   Sebastian Zug, André Dietrich

email:    sebastian.zug@informatik.tu-freiberg.de

version:  0.1.0

language: de

narrator: Deutsch Male

mode:     Presentation

date:     28/05/2026

comment:  Phase 4 des Online-Workshops "OPAL Schule meets LiaScript"
          am 28.05.2026 für die Referent:innen der Medienpädagogischen
          Zentren in Sachsen. KI-Unterstützung, Verbreitung und
          Einbettung in OPAL Schule — 20 Minuten.

repository: https://github.com/LiaPlayground/Opal_Schule_meets_LiaScript

attribute: OPAL Schule meets LiaScript — Phase 4 (Verbreiten)
           von Sebastian Zug, André Dietrich
           ist lizenziert unter [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/04_Verbreiten.md)

# KI-Unterstützung, Verbreitung und OPAL-Schule-Integration

> <h3>Phase 4 des Workshops „OPAL Schule meets LiaScript"</h3>
>
> <h4>Prof. Dr. Sebastian Zug, Dr. André Dietrich</h4>
> <h4>TU Bergakademie Freiberg</h4>
>
> <h4>28. Mai 2026 — Workshop für die Medienpädagogischen Zentren</h4>

--------------------------------------------

## Worum geht es in diesen 20 Minuten?

In [Phase 3](03_Anwenden_Vorlage.md) haben Sie mit der Hand gespürt, *wie* ein LiaScript-Kurs aufgebaut wird. Jetzt geht es um die zwei Fragen, die sich danach unweigerlich stellen:

1. **Muss eine Lehrkraft das jedes Mal so machen?** — Stichwort: KI-Werkzeuge, die genau diese Arbeit übernehmen.
2. **Wie kommt der fertige Kurs zu den Lernenden?** — Stichwort: fünf Verbreitungswege, **mit zwei expliziten OPAL-Schule-Pfaden** (nativ und via SCORM).

> [!IMPORTANT]
> **Für Ihre Multiplikator:innen-Rolle:** Diese 20 Minuten enthalten *zwei* Argumente, die Sie an Ihre Lehrkräfte weitergeben können — *„Sie müssen das nicht von Hand schreiben"* und *„Es passt in Ihre bestehende OPAL-Welt"*. Beides senkt typische Einstiegshürden dramatisch.

## Teil A — KI als Co-Autorin für LiaScript-Kurse

Vor zwei Jahren hieß die Antwort auf „Wie schreibe ich einen LiaScript-Kurs?" noch: *„Cheat Sheet öffnen, Syntax nachschlagen, ausprobieren."* Heute heißt sie zunehmend: *„Beschreiben Sie der KI, was Sie unterrichten wollen — und prüfen Sie die Vorlage."*

> [!NOTE]
> **Was sich nicht geändert hat:** Die Lehrkraft entscheidet, *was* unterrichtet wird, *welches Beispiel* gewählt wird, *welche Differenzierung* sinnvoll ist. Die KI nimmt nur die **Syntax-Last** ab — sie weiß, wie ein Quiz, eine Formel oder eine Animation in LiaScript geschrieben werden.

### Zwei Stufen der KI-Nutzung

           {{0-1}}
**************************************

**Stufe 1 — Web-KI mit angehängter Skill-Datei**

Die niedrigschwellige Variante: Eine einzige Markdown-Datei, [**LiaSkill**](https://github.com/LiaScript/LiaSkill), wird einer Web-KI als Kontext mitgegeben — Claude, ChatGPT, Gemini oder Mistral, egal welche. Die KI „lernt" daraus die vollständige LiaScript-Syntax und kann anschließend komplette Kurse aus Klartext-Beschreibungen erzeugen.

| Schritt | Was tun?                                                                                            |
| ------- | --------------------------------------------------------------------------------------------------- |
| 1       | [SKILL.md](https://github.com/LiaScript/LiaSkill/blob/main/SKILL.md) als Datei in den Chat ziehen   |
| 2       | Beschreiben: *„Erstelle einen Kurs zu …, Klassenstufe …, mit … Quizzen und … Differenzierung."*    |
| 3       | Ergebnis im [LiveEditor](https://liascript.github.io/LiveEditor/) prüfen, anpassen                  |

> **Geeignet für:** Lehrkräfte, die heute schon ChatGPT oder Copilot nutzen — kein neues Werkzeug, nur ein angehängtes Dokument.

**************************************

           {{1}}
**************************************

**Stufe 2 — Geführter Prozess in VS Code: der Teaching-Agent**

Die professionelle Variante: [**Teaching-Agent**](https://github.com/LiaScript/teaching-agent) führt Sie in **VS Code mit GitHub Copilot** durch einen vollständigen, strukturierten Kursentwurf — vom Lernziel über die Didaktik bis zum fertigen Material. Statt eines einzelnen Prompts entsteht ein iterativer Dialog mit definierten Phasen:

```ascii
  ┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
  │  FOUNDATION     │ →  │  DIDACTICS      │ →  │  PLANNING       │
  │  Zielgruppe,    │    │  Lehrmethoden,  │    │  Agenda,        │
  │  Lernziele,     │    │  Persona,       │    │  Sitzungs-      │
  │  Umfang         │    │  Stil           │    │  struktur       │
  └─────────────────┘    └─────────────────┘    └─────────────────┘
            │                                              │
            ↓                                              ↓
  ┌─────────────────┐    ┌─────────────────┐
  │  DEVELOPMENT    │ ←  │  FINALIZATION   │
  │  Sitzungen      │    │  Validierung,   │
  │  ausarbeiten    │    │  Export-Bundle  │
  └─────────────────┘    └─────────────────┘
```

> **Geeignet für:** Lehrkräfte, die regelmäßig Material entwickeln und Wert auf didaktische Konsistenz legen — Schul-Curricula, Fortbildungsreihen, fachübergreifende Module.

**************************************

### Beispiel: Energie.md mit KI in einen LiaScript-Kurs verwandeln

> [!TIP]
> **Live-Demo am Workshop-Stoff.** Genau die Transformation, die Sie in [Phase 3](03_Anwenden_Vorlage.md) per Hand geübt haben — von `Energie.md` zu einem nutzbaren Kurs — schauen wir uns jetzt mit KI-Unterstützung an.

           {{0-1}}
**************************************

**Ein einziger Prompt für Stufe 1 (LiaSkill an Claude/ChatGPT):**

```text
Hier ist der Rohstoff Energie.md aus einem OPAL-Schule-Kurs der 11. Klasse Physik:

  <Inhalt von Energie.md einfügen>

Bitte daraus einen LiaScript-Kurs erstellen mit:
- sauber gesetzten LaTeX-Formeln (statt der zerlegten Unicode-Schnipsel),
- der PhET-Federpendel-Simulation als ?? - Einbettung,
- den drei Selbsttests als LiaScript-Quizze (Einfachauswahl, Mehrfachauswahl,
  Zahleneingabe) mit Hinweisen und ausklappbaren Lösungen,
- einer Differenzierungs-Aufgabe für leistungsstärkere SuS,
- Vorlese- und Übersetzungs-Aktivierung im Frontmatter.
```

Die KI liefert in einer Antwort ein vollständiges, sofort renderbares `.md` — vergleichbar mit unserer [03_Anwenden_Loesung.md](03_Anwenden_Loesung.md), die in Phase 3 von Hand entstanden ist.

**************************************

           {{1-2}}
**************************************

**Was bleibt für die Lehrkraft zu tun?**

+ **Fachliche Prüfung** — Sind die physikalischen Aussagen korrekt? Stimmen die Lösungen?
+ **Didaktische Anpassung** — Passt die Aufgabe zur eigenen Lerngruppe? Brauchen wir mehr Hinweise?
+ **Kontext** — Welche externen Medien (edupool, eigene Bilder) sollen rein, die die KI nicht kennen kann?
+ **Lizenz und Quellen** — Stimmen die Verweise? Ist die Eigenarbeit als CC-BY-SA gekennzeichnet?

> [!NOTE]
> **Diese vier Schritte sind unverzichtbar — und sie sind genau das, was Lehrkräfte am besten können.** Die KI nimmt die *Syntax-Mühen* ab. Die *fachliche Verantwortung* bleibt bei der Lehrkraft.

**************************************

### Datenschutz und Lizenz-Fragen

> [!WARNING]
> **Was übersieht man leicht?** Wenn Sie Schul-Material in eine externe Web-KI füllen, prüfen Sie vorab:
>
> + Enthält der Stoff **personenbezogene Daten** (Namen von Schüler:innen, Klassenbezeichnungen)? → entfernen.
> + Sind die Quellen, die Sie einspeisen, **lizenzrechtlich teilbar**? Ein Auszug aus dem Schulbuch ist es meistens **nicht**.
> + Welche Datenschutz­erklärung hat der KI-Anbieter? Lokale Modelle (z. B. via Ollama) oder behördlich genehmigte Lösungen können hier eine Antwort sein.

Für sensiblere Kontexte ist der Teaching-Agent in VS Code mit lokal laufenden Modellen die robustere Wahl.

## Teil B — Fünf Verbreitungswege

In [Phase 2](02_Verstehen.md) haben wir festgehalten: Ein LiaScript-Kurs ist eine einzelne Markdown-Datei, die im Browser ausgeführt wird. Diese Eigenschaft eröffnet fünf sehr unterschiedliche Verbreitungswege — von der schnellen URL bis zum vollintegrierten SCORM-Paket mit OPAL-Lernstandserfassung.

| Weg                       | Was wird geteilt?                      | Wofür geeignet?                                                          |
| ------------------------- | -------------------------------------- | ------------------------------------------------------------------------ |
| **Data-URI**              | Ein Link, der den Kurs enthält         | Schnelle Vorschau, kurze Materialien, Versand per Mail                   |
| **ZIP-Export**            | Alle Dateien als Archiv                | Vollständige Kurse mit Bildern, Offline-Nutzung im Klassenraum           |
| **OPAL Schule nativ**     | ZIP-Datei im OPAL-Kursbaustein         | Einbettung in OPAL — **schnell, ohne Konvertierung**, ohne Lernstand     |
| **OPAL Schule via SCORM** | SCORM-Paket im OPAL-Kursbaustein       | Einbettung in OPAL — **mit Lernstand-Erfassung** im OPAL-Notenheft       |
| **Git-Repository**        | Quelle auf GitHub/GitLab               | Kollaborative Pflege, Versionierung, stabiler Link                       |

### 1. Verbreitung per Data-URI

> [!TIP]
> **Definition:** Eine Data-URI ist ein Link, der den vollständigen Kursinhalt direkt in der URL transportiert — keine zusätzliche Datei, kein Server, kein Hosting nötig.

Im LiveEditor lassen Sie sich aus dem Menü eine **Data-URI** erzeugen. Diese URL können Sie per E-Mail, Chat oder QR-Code weitergeben — beim Öffnen erscheint der Kurs sofort im LiaScript-Player.

> [!NOTE]
> **Wofür im Schulalltag besonders nützlich:** Schnelle Vertretungsstunden-Materialien, ein kurzer Selbsttest per Beamer-QR-Code, ein Mail-Anhang an eine kranke Kollegin. **Grenze:** Data-URIs werden mit Kurslänge sehr lang — für umfangreichere Materialien wechseln Sie auf Weg 2 oder 5.

### 2. Verbreitung per ZIP-Datei

Im LiveEditor können Sie Ihren Kurs als **ZIP-Datei** exportieren. Diese Archivdatei enthält die Markdown-Quelle plus alle eingebetteten Bilder und lokal referenzierten Ressourcen. Die ZIP-Datei können Sie beliebig verbreiten — per Mail, über Schul-Cloud, USB-Stick, internes Schulnetz oder Cloudanbieter wie NextCloud, OneDrive usw.

> [!IMPORTANT]
> **So öffnen die Empfänger:innen das ZIP:** **Nicht entpacken.** Stattdessen die LiaScript-Player-Seite [**liascript.github.io/course/**](https://liascript.github.io/course/) öffnen und das ZIP-Archiv unter **„Courses"** importieren. Der Player liest das Archiv ein und startet den Kurs direkt.

Bei der Distribution via Cloud gibt es einige Fallstricke zu beachten. Je nach Anbieter müssen Sie die ZIP-Datei entweder öffentlich freigeben oder einen speziellen Link-Format verwenden, damit der Player sie lesen kann. Hier lohnt sich ein kurzer Testlauf mit einem Kollegen, bevor Sie den Link an die ganze Klasse oder Schule weitergeben.

> [!NOTE]
> Gegenwärtig funktioniert das Teilen über DropBox sehr zuverlässig. Dazu muss beim Link zum ZIP-Archiv die Endung `?raw=1` beigefügt werden. Beispiel: `https://www.dropbox.com/s/abc123/MeinKurs.zip?raw=1`. Diese URL wird dann einfach auf https://liascript.github.io/course/ als Adresse angegeben.

An Lösungen für NextCloud und OneDrive wird gearbeitet — hier ist die Lage aktuell etwas uneinheitlich, je nach Version und Konfiguration des Cloud-Servers.

### 3. OPAL Schule nativ

> [!IMPORTANT]
> **Die gute Nachricht für sächsische Lehrkräfte:** OPAL Schule kann LiaScript-Kurse **direkt rendern** — kein SCORM-Export nötig, keine Konvertierung. Ein ZIP aus dem LiveEditor (wie in Weg 2 beschrieben) lässt sich in einen OPAL-Kursbaustein hochladen, und der eingebaute Renderer zeigt den Kurs in der gewohnten OPAL-Umgebung an.

           {{0-1}}
**************************************

**Die native OPAL-Einbettung Schritt für Schritt**

| Schritt | Was tun?                                                                                                       |
| ------- | -------------------------------------------------------------------------------------------------------------- |
| 1       | Im LiveEditor den Kurs als **ZIP-Datei** exportieren (gleiches Format wie in Weg 2)                            |
| 2       | In OPAL Schule den Kurs-Editor öffnen → **Kursbaustein „Einzelne Seite" oder „CP-Lerninhalt" hinzufügen**       |
| 3       | ZIP-Datei hochladen → die Markdown-Datei als Startseite auswählen → Bezeichnung vergeben → speichern           |
| 4       | Baustein freigeben — Lernende sehen den LiaScript-Kurs ab jetzt **direkt im OPAL-Schule-Klassenraum**           |

**************************************

           {{1}}
**************************************

**Was funktioniert — und was nicht**

| Aspekt                            | Nativer LiaScript-Renderer in OPAL                       |
| --------------------------------- | -------------------------------------------------------- |
| Vollständige Darstellung des Kurses | ✓ Formeln, Animationen, Embeds, Quizze, Code, Vorlesen   |
| Lernende arbeiten Selbsttests durch | ✓ Quiz-Feedback erscheint direkt im Browser              |
| **Erfassung der Quiz-Ergebnisse** im OPAL-Notenheft | ✗ kein Tracking — was die Schülerin geantwortet hat, weiß OPAL nicht |
| **Sichtbarkeit für die Lehrkraft**, wer welchen Stand hat | ✗ ebenfalls nicht                                        |

> **Wann reicht das?** Für **formatives** Selbstlernen ohne Notenrelevanz, für Vertretungsstunden, für Übungsphasen, für Differenzierungsangebote. Genau das, was Lommatzsch in [Phase 2](02_Verstehen.md) beschrieben hat — *„Schülerinnen und Schüler bekommen die Rückmeldung sofort, ohne dass die Lehrkraft jeden Tisch ablaufen muss."*

> **Wann reicht es nicht?** Sobald Sie als Lehrkraft **summativ** prüfen wollen oder einen *Klassenüberblick* über den Lernstand brauchen. Dann führt Weg 4 (SCORM) zum Ziel.

**************************************

### 4. OPAL Schule via SCORM

Wenn Sie die Quiz-Ergebnisse Ihrer Schüler:innen **im OPAL-Notenheft sehen** möchten, exportieren Sie den Kurs als **SCORM-Paket** und laden es in den entsprechenden OPAL-Kursbaustein. Damit erhält LiaScript die volle Anbindung an die OPAL-Klassenraumfunktionen — wie eine ONYX-Aufgabe, aber mit der ganzen LiaScript-Mächtigkeit dahinter.

> [!NOTE]
> **Was SCORM bedeutet:** SCORM ist der Industriestandard, mit dem Lernmanagementsysteme Inhalte einlesen *und gleichzeitig Lernstand erfassen* — ob ein Quiz bearbeitet wurde, welche Antworten kamen, ob ein Kurs als „abgeschlossen" gilt.

           {{0-1}}
**************************************

**Die SCORM-Einbettung Schritt für Schritt**

| Schritt | Was tun?                                                                                          |
| ------- | ------------------------------------------------------------------------------------------------- |
| 1       | LiaScript-Kurs als SCORM-Paket exportieren (per [LiaScript-Exporter](https://github.com/LiaScript/LiaScript-Exporter) - aktuell noch ein Zusatzprogramm) |
| 2       | In OPAL Schule den Kurs-Editor öffnen → **Kursbaustein „SCORM-Lerninhalt" hinzufügen**             |
| 3       | SCORM-ZIP hochladen → Bezeichnung vergeben → speichern                                            |
| 4       | Baustein freigeben — Quiz-Ergebnisse erscheinen jetzt im **OPAL-Bewertungswerkzeug**               |

**************************************

           {{1}}
**************************************

**Welcher der beiden OPAL-Wege passt wann?**

| Szenario                                                              | Empfohlener Weg               |
| --------------------------------------------------------------------- | ----------------------------- |
| Differenzierungs-Material, Vertretungsstunde, freiwillige Übung       | Weg 3 — nativer ZIP-Upload    |
| Erste Begegnung der Lehrkraft mit LiaScript-in-OPAL                   | Weg 3 — nativer ZIP-Upload    |
| Bewertete Übungssequenz, Vorbereitung Klassenarbeit, Lernstandsdiagnose | Weg 4 — SCORM-Paket           |
| Materialien, die später auch außerhalb OPAL laufen sollen             | beide funktionieren           |

> [!IMPORTANT]
> **Der entscheidende Unterschied zu „klassischen" OPAL-Inhalten:** Eine ONYX-Aufgabe ist *in* OPAL. Ein LiaScript-Kurs *läuft* in OPAL Schule — aber **wohnt nicht dort**. Wenn Sie nächstes Jahr den Kurs überarbeiten, ändern Sie ihn in der Markdown-Quelle (oder lassen die KI helfen), erzeugen ein neues ZIP bzw. SCORM und laden es hoch — die Quelle bleibt unter Ihrer Kontrolle, in jedem System.

**************************************

> [!TIP]
> **Empfehlung für Ihre Multiplikatoren-Praxis:** Starten Sie mit Lehrkräften *immer* über Weg 3 (nativ). Der erste Klickerfolg — "es funktioniert tatsächlich in OPAL!" — ist die wichtigste Hürde. SCORM kommt erst dann ins Spiel, wenn die Lehrkraft konkret Tracking braucht.


### 5. Verbreitung über GitHub oder GitLab

Der schmalste Bauplan eines LiaScript-Kurses ist eine einzige Markdown-Datei — und genau das macht **GitHub** und **GitLab** zum natürlichen Zuhause für Ihre Materialien. Sie legen den Kurs als Datei in ein Repository, und der LiaScript-Player rendert ihn direkt aus der **Raw-URL** des Repositorys.

> [!TIP]
> **Das Muster:** Hängen Sie die Raw-URL Ihrer Markdown-Datei an den Player-Pfad an:
>
> `https://liascript.github.io/course/?` + Raw-URL
>
> Genau dieses Muster nutzt auch der Badge oben auf jeder Workshop-Phase — schauen Sie sich den Link genauer an.

           {{0-1}}
**************************************

**Was Sie dadurch gewinnen:**

+ **Versionierung** — Jede Änderung ist nachvollziehbar. Sie können jederzeit zur Fassung „vom letzten Schuljahr" zurückkehren.
+ **Kollaboration** — Kolleg:innen anderer Schulen schlagen per *Pull Request* Verbesserungen vor, ohne dass Sie ihnen Schreibrechte geben.
+ **Dauerhafter Link** — Die URL ändert sich nicht. Lehrkräfte, die den Link in OPAL Schule eingebettet haben, müssen *nichts* nachpflegen, wenn Sie den Inhalt aktualisieren.
+ **Tag-basierte Stabilität** — Verlinken Sie auf einen Git-*Tag* statt auf `main`, bekommen Lernende eine eingefrorene Fassung — auch wenn Sie parallel weiterarbeiten.

**************************************

           {{1}}
**************************************

> [!IMPORTANT]
> **Der OER-Königsweg.** Repository = Quelle + Historie + Lizenz + Zusammenarbeitsplattform in einem. Die fünf V-Freiheiten aus [Phase 2](02_Verstehen.md) greifen hier *vollständig* — und das **kollaborativ**, nicht nur als einseitige Weitergabe.

Lommatzschs Aufgabensammlung auf [mint-the-gap.github.io/Aufgabensammlung](https://mint-the-gap.github.io/Aufgabensammlung/) ist ein laufendes Beispiel: ein einziges GitHub-Repository, an dem eine Lehrkraft seit Jahren wächst — und das mehrere Klassen versorgt.

**************************************

## Teil C — Was Sie an Ihre Lehrkräfte weitergeben

Sie sind die Multiplikator:innen. Was Sie in den vergangenen zwei Stunden gesehen und gemacht haben, geben Sie an Lehrer:innen weiter — und zwar in deutlich kürzerer Zeit. Drei Dinge nehmen Sie idealerweise mit:

           {{0-1}}
**************************************

**1. Das Repository als Vorlage**

Alles, was Sie heute gesehen haben, liegt unter [github.com/LiaPlayground/Opal_Schule_meets_LiaScript](https://github.com/LiaPlayground/Opal_Schule_meets_LiaScript) als CC-BY-SA-Material. Sie dürfen es als Grundlage für Ihre eigenen Fortbildungen verwenden, ergänzen, kürzen, ummontieren.

**************************************

           {{1-2}}
**************************************

**2. Die 4-Phasen-Choreografie**

```ascii
  ┌──────────────┐   ┌──────────────┐   ┌──────────────┐   ┌──────────────┐
  │   ERLEBEN    │ → │  VERSTEHEN   │ → │   ANWENDEN   │ → │  VERBREITEN  │
  │              │   │              │   │              │   │              │
  │  20 min      │   │  15 min      │   │  45 min      │   │  20 min      │
  │  Demo-Kurs   │   │  Vortrag     │   │  Hands-on    │   │  KI + OPAL   │
  └──────────────┘   └──────────────┘   └──────────────┘   └──────────────┘
```

Diese Choreografie ist robust: Sie funktioniert für 90 Minuten an einer einzigen Schule genauso wie für drei Halbtage in einer ganzen Region. Skalieren Sie über die Hands-on-Phase — Sie ist das Herzstück.

**************************************

           {{2}}
**************************************

**3. Die zwei Antworten auf die häufigsten Lehrkraft-Einwände**

> *„Das ist mir zu technisch."*
> → **„Sie schreiben nichts mehr selbst. Die KI macht das. Sie sagen ihr nur, *was* Sie unterrichten wollen — und prüfen, ob das Ergebnis Ihrer Klasse gerecht wird."**

> *„Das passt nicht in unsere bestehende OPAL-Struktur."*
> → **„Doch — OPAL Schule kann LiaScript sogar nativ rendern: ZIP-Upload in den passenden Kursbaustein, fertig. Wenn Sie Quiz-Ergebnisse im OPAL-Notenheft brauchen, geht das zusätzlich via SCORM. Aber der Quelltext bleibt in beiden Fällen offen und teilbar."**

**************************************

## Zusammengefasst

> [!TIP]
> 1. **KI als Co-Autorin:** Zwei Stufen — LiaSkill für Schnelle, Teaching-Agent für Strukturierte. Beides offen verfügbar, beides reduziert die Einstiegshürde drastisch.
> 2. **Fünf Verbreitungswege:** Data-URI (Klick-Demo) → ZIP (offline) → **OPAL nativ** (ZIP-Upload, kein Tracking) → **OPAL via SCORM** (mit Lernstand-Erfassung) → GitHub (kollaborativ). Empfehlung: Lehrkräfte zuerst über den nativen Weg ins OPAL bringen.
> 3. **OER bleibt erhalten:** In allen fünf Wegen reist der Markdown-Quelltext mit. Wer den Kurs erhält, kann ihn anpassen, weiterentwickeln, in eigenen Kontexten wiederverwenden.
> 4. **Sie sind dran.** Diese Argumentation tragen Sie weiter — an Schulen, an Fachschaften, an Schulleitungen.

## Kontakt und Material

- **Repository:** [github.com/LiaPlayground/Opal_Schule_meets_LiaScript](https://github.com/LiaPlayground/Opal_Schule_meets_LiaScript)
- **LiaScript-Community-Chat:** [gitter.im/LiaScript/community](https://gitter.im/LiaScript/community)
- **Kontakt:** sebastian.zug@informatik.tu-freiberg.de · andre.dietrich@informatik.tu-freiberg.de

> **Vielen Dank — und viel Erfolg bei Ihren eigenen Workshops!**

> [!TIP]
> Kommen Sie bei Unklarheiten gern auf uns zu - wir unterstützen Sie bei der Vorbereitung Ihrer eigenen Workshops, bei der Anpassung des Materials oder bei Fragen zu KI und OPAL Schule.

## Lizenz

Dieses Material steht unter [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.de).
