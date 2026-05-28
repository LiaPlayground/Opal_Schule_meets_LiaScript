<!--
author:   Sebastian Zug, André Dietrich

email:    sebastian.zug@informatik.tu-freiberg.de

version:  0.1.1

language: de

narrator: Deutsch Male

mode:     Presentation

date:     28/05/2026

comment:  Phase 2 des Online-Workshops "OPAL Schule meets LiaScript"
          am 28.05.2026 für die Referent:innen der Medienpädagogischen
          Zentren in Sachsen. Konzepte und Vision von LiaScript — 15 Minuten.

repository: https://github.com/LiaPlayground/Opal_Schule_meets_LiaScript

import:   https://raw.githubusercontent.com/LiaTemplates/LiveEdit-Embeddings/refs/tags/0.0.1/README.md

attribute: OPAL Schule meets LiaScript — Phase 2 (Verstehen)
           von Sebastian Zug, André Dietrich
           ist lizenziert unter [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/02_Verstehen.md)

# Konzepte und Vision hinter LiaScript

> <h3>Phase 2 des Workshops „OPAL Schule meets LiaScript"</h3>
>
> <h4>Prof. Dr. Sebastian Zug, Dr. André Dietrich</h4>
> <h4>TU Bergakademie Freiberg</h4>
>
> <h4>28. Mai 2026 — Workshop für die Medienpädagogischen Zentren</h4>

--------------------------------------------

## Worum geht es in diesen 15 Minuten?

Sie haben in [Phase 1](01_Erleben.md) erlebt, *was* mit LiaScript möglich ist — Formeln, Quizze, eingebettete Simulationen, ausführbarer Code, alles in *einer* Markdown-Datei. Jetzt geht es um das *Warum*:

- Welches Problem löst LiaScript für Lehrkräfte eigentlich?
- Warum reicht **OPAL Schule** als Lernmanagement­system nicht aus, um interaktive Materialien dauerhaft zu pflegen?
- Was sind die **drei technischen Kernideen**, die alles zusammenhalten?

> [!NOTE]
> **Hintergrund für Ihre Multiplikatorenrolle:** Diese 15 Minuten enthalten genau die Argumente, mit denen Sie später skeptische Lehrkräfte überzeugen können. Notieren Sie sich, welches Argument bei *Ihrem* Kollegium am besten zünden würde.

## Ausgangspunkt

>  <!-- Style="color:green" -->__Lehrkräfte möchten motivierende, interaktive Lehrmaterialien einsetzen — zugeschnitten auf ihre konkrete Lerngruppe — und mit Kolleg:innen anderer Schulen teilen.__

                  {{0-1}}
********************************************

**Aber in der Praxis …**

+ Die individuelle Umsetzung ist **aufwändig und zeitintensiv** — neben Unterrichtsvorbereitung, Korrekturen und Konferenzen.
+ Für jedes Format gibt es ein **eigenes Werkzeug** — LearningSnacks hier, H5P dort, GeoGebra-Aktivitäten daneben, ONYX-Tests im LMS.
+ Bestehende Inhalte sind **nicht auf die eigene Klasse zugeschnitten** — und Anpassen wird zur Click-Marathon-Aufgabe.
+ Materialien aus OPAL Schule lassen sich **kaum aus dem System lösen** — was im Kurs entstand, bleibt im Kurs gefangen.

> Welche weiteren Hemmnisse kennen Sie aus Ihrer Beratungspraxis?

********************************************

{{1}}
```ascii

       Wunsch nach                                              Wunsch nach
   einfacher Umsetzung  -----------> Konflikt <----------- spezifischen Elementen
                                                                im Material
```

### OER als Lösungsansatz — die 5V-Freiheiten

           {{0-1}}
**************************************

Der Konflikt löst sich auf, wenn Materialien **geteilt, angepasst und weiterentwickelt** werden können — statt jedes Mal bei Null anzufangen. Genau das beschreibt der OER-Gedanke:

>  **Open Educational Resources** … teaching, learning and research materials in any medium, digital or otherwise, that reside in the **public domain** or have been released under an open license that permits no-cost access, use, **adaptation** and **redistribution** by others.
>
> -- UNESCO 2002 Forum on the Impact of Open Courseware [(Link)](https://unesdoc.unesco.org/ark:/48223/pf0000128515)

**************************************

           {{1}}
**************************************

| 5V-Freiheit                  | Bedeutung für die Schule                                                  |
| ---------------------------- | ------------------------------------------------------------------------- |
| `verwahren/vervielfältigen ` | Download auf Schulserver, USB-Stick, lokaler Cache fürs WLAN-lose Zimmer  |
| `verwenden`                  | Einsatz im Klassenraum, in der Vertretungsstunde, als Hausaufgabe         |
| `verarbeiten`                | Anpassen an die eigene Lerngruppe — Differenzierung, DaZ, Inklusion       |
| `vermischen`                 | Kombinieren von eigenen Aufgaben mit PhET-Sims, YouTube-Videos, Sodix     |
| `verbreiten`                 | Teilen mit dem Fachkollegium, dem MPZ-Netzwerk, OPAL Schule oder GitHub   |

*„5 V-Freiheiten für Offenheit" von Jöran Muuß-Merholz und Jörg Lohrer für [open-educational-resources.de](https://open-educational-resources.de)*

> **Die entscheidende Frage:** In welchem *Format* speichere ich meine Materialien, damit alle fünf V-Freiheiten technisch überhaupt möglich sind?

**************************************

### Warum nicht einfach eine Word-Datei?

DOCX, PowerPoint, ein Wiki im Schulnetz — alles theoretisch denkbar. In der Praxis scheitern sie an konkreten Schul-Anforderungen:

| Format          | Was fehlt für interaktive Lehre?                                                  |
| --------------- | --------------------------------------------------------------------------------- |
| DOCX / PDF      | keine Interaktion, keine Lernstands­erfassung, kein Quiz mit Rückmeldung           |
| PowerPoint      | wie DOCX — plus: Lernen heißt nicht Folien klicken                                 |
| Schulwiki       | nahe dran — aber Quizze, Code, Simulationen nicht ohne Plugin-Wartung              |
| ONYX in OPAL    | Quizze ja — aber an OPAL gebunden, kein OER, nicht teilbar                         |
| H5P             | interaktiv — aber proprietäres JSON-Format, in jedem System anders gepflegt        |

> **Die Lücke:** Wir brauchen ein Format, das *so einfach wie eine Textdatei* ist — und Interaktion, Lernpfade und LMS-Anschluss von Haus aus mitbringt.

## LiaScript — die Kernidee in einem Satz

> [!IMPORTANT]
> **LiaScript ist Markdown — erweitert um genau die Elemente, die für interaktive Lehre fehlen.**

Markdown kennen viele bereits — aus GitHub-READMEs, aus Obsidian, oder über die ein-Stern-zwei-Stern-Schreibweise auf WhatsApp. LiaScript nimmt diese vertraute Textsprache und ergänzt sie um **drei Kernkonzepte**.

### Konzept 1 — Trennung von Inhalt und Darstellung

> __Alles, was geht, wird als reiner Text geschrieben. Wie es am Ende aussieht, entscheidet der Player — nicht der Autor.__

```markdown @embed.style(height: 600px; min-width: 100%; border: 1px black solid)
# Vom Text zur Darstellung

__Formatierter Text__

Die kinetische Energie ist eine **Schlüsselgröße** der Mechanik.

__Mathematik__ — einfach in `$...$` setzen:

$E_\text{kin} = \tfrac{1}{2}\, m\, v^2$

__Tabellen__ — wie in Markdown gewohnt:

| Energieart   | Beispiel aus dem Alltag         |
| ------------ |:--------------------------------|
| kinetisch    | fahrendes Auto                  |
| potentiell   | Werkzeug am Kran                |
| Spannenergie | gespannter Bogen                |
```

> [!NOTE]
> **Warum das für die Schule zentral ist:** Wer den Quelltext hat, hat alles. Keine versteckten Formate, kein „nur in OPAL editierbar", keine Layout-Reste beim Export. Der Markdown-Text *ist* das Material — und passt in jedes Git-Repo, jeden Mail-Anhang, jeden USB-Stick.

### Konzept 2 — Interaktion gehört zum Inhalt

> __Quizze, Animationen, Selbsttests sind keine Plugins — sie sind Teil der Auszeichnungssprache selbst.__

In [Phase 1](01_Erleben.md) haben Sie drei Quiz-Formate gesehen (Einfachauswahl, Zahleneingabe, Mehrfachauswahl). Im Quelltext sind das **wenige Zeilen Markdown** — keine Plugin-Installation, keine ONYX-Datenbank, keine ID-Verwaltung.

```markdown @embed.style(height: 600px; min-width: 100%; border: 1px black solid)
# Lehre lebt von Interaktion

__Quiz mit automatischer Rückmeldung__

Ein Ball mit Masse $m = 4$ kg und Geschwindigkeit $v = 27$ m/s.
Wie groß ist $E_\text{kin}$ in Joule?

[[1458]]
[[?]] Hinweis: $E_\text{kin} = \tfrac{1}{2}\, m\, v^2$ — auf das Quadrat achten!

__Animationsstufen__ — wie bei einer Tafel-Erklärung:

{{1}} 
Erst kommt die Formel:  $E = \tfrac{1}{2}\, m\, v^2$,

{{2}} 
dann ein Zahlenbeispiel: $m = 4, v = 27 \Rightarrow E = 1458$ J,

{{3}} 
schließlich die Pointe:  Doppeltes $v$ → vierfaches $E$.
```

> [!NOTE]
> **Vergleich zum LMS-Ansatz:** Ein ONYX-Quiz lebt *in* OPAL. Verlassen Sie OPAL, ist die Aufgabe weg. Ein LiaScript-Quiz lebt im Markdown-Text — und reist überall mit. Auf dem Smartboard, im Tablet der Schülerin, im Mail-Anhang an die Vertretungslehrkraft.

### Konzept 3 — Der Browser ist die Laufzeitumgebung

> __Was der Browser kann, kann LiaScript. Und der Browser kann heute erstaunlich viel.__

Erinnern Sie sich an den Python-Code in [Phase 1](01_Erleben.md)? Da lief **echtes Python** — im Browser, ohne Installation, ohne Server. Das ist kein LiaScript-Feature im engeren Sinn, sondern moderner Browser-Standard (WebAssembly, Pyodide). LiaScript bindet diese Fähigkeiten konsequent ein:

+ **Code ausführen** — Python, JavaScript, R, SQL, C++ … direkt in der Aufgabe.
+ **Sprachausgabe** — Texte vorlesen lassen (Inklusion, DaZ).
+ **Lernstand speichern** — im Browser, ohne Server-Datenbank.
+ **3D-Modelle, Simulationen, Notenschrift, Schaltkreise** — über offene Templates beliebig erweiterbar.

```markdown @embed.style(height: 600px; min-width: 100%; border: 1px black solid)
# Der Browser als Plattform

__Sprachausgabe__ — einfach per Tag:

> {{|> Deutsch Female}}
> Willkommen im Physik-Unterricht der 11. Klasse!

__3D-Modell — direkt eingebettet__

??[Mineralien-Modell](https://sketchfab.com/3d-models/familienschacht-freiberg-germany-7c7d30506c554385a4a4321366e2e601)
```

> [!NOTE]
> **Warum das für Schule besonders zählt:** *Kein lokales Setup* heißt — die Schülerin am Smartboard, der Schüler zu Hause auf dem ältesten Laptop, die DaZ-Klasse mit gemischten Geräten: alle sehen denselben Kurs. Nur einen Browser braucht es.

## Und wie verträgt sich das mit OPAL Schule?

Wie funktioniert das aber technisch? Ein LiaScript-Kurs ist eine **Markdown-Datei**, die von einem **Player** im Browser ausgeführt wird. Der Player liest den Text und macht ihn interaktiv. Das heißt:

1. **Es gibt keinen „LiaScript-Server"** — der Kurs läuft komplett im Browser, ohne Installation, ohne Internet (nach dem ersten Laden).
2. **Der Kurs ist eine einzelne Markdown-Datei** — keine Datenbank, kein proprietäres Format, keine versteckten Metadaten.
3. **Der Interpreter ist Open Source** — keine „Black Box", die das Material gefangen hält.

> [!IMPORTANT]
> **OPAL Schule und LiaScript stehen nicht in Konkurrenz — sie arbeiten auf verschiedenen Ebenen.**

           {{0-1}}
**************************************

| Ebene                  | Verantwortlich für                                       | Vertreter (Schule)      |
| ---------------------- | -------------------------------------------------------- | ----------------------- |
| **Inhalt**             | Was wird vermittelt? Wie wird es dargestellt?            | **LiaScript**, H5P      |
| **Distribution / LMS** | Wer sieht was wann? Klassenverwaltung, Noten, Zugriff    | **OPAL Schule**, Moodle |

**************************************

           {{1}}
**************************************

Konkret: Ein LiaScript-Kurs lässt sich **als SCORM- oder xAPI-Paket exportieren** und in OPAL Schule einspielen. OPAL übernimmt dann Anmeldung, Klassenraum, Notenvergabe — der eigentliche *Inhalt* bleibt aber im offenen Markdown-Format erhalten und kann jederzeit aus dem LMS herausgelöst, angepasst und woanders wiederverwendet werden.

> **Der entscheidende Unterschied zu „nativen" OPAL-Inhalten:** Eine ONYX-Aufgabe ist *in* OPAL. Ein LiaScript-Kurs *läuft* in OPAL — aber wohnt nicht dort. Genau das macht ihn zur echten OER.

**************************************

> [!NOTE]
> **Wie konkret kommt der Kurs nach OPAL Schule?** Genau das schauen wir uns in **[Phase 4 (Verbreiten)](04_Verbreiten.md)** an — gemeinsam mit den Themen KI-Generator und produktive Werkzeugkette (VS Code, GitHub).

## Eine Stimme aus der Schule

> [!TIP]
> Eine vollständige Materialsammlung in LiaScript — von einer Lehrkraft, im Alltag entstanden — findet sich unter [mint-the-gap.github.io/Aufgabensammlung](https://mint-the-gap.github.io/Aufgabensammlung/). - **Martin Lommatzsch**, Geschwister-Scholl-Gymnasium Freiberg, Mathematik

## Zusammengefasst

> [!TIP]
> 1. **Format:** LiaScript ist erweitertes Markdown — ein offenes, textuelles Quellformat.
> 2. **Interaktion:** Quizze, Code, Animationen sind Teil der Sprache, nicht Plugins eines Systems.
> 3. **Plattform:** Der Browser führt aus — kein Server, kein lokales Setup, keine IT-Tickets.
> 4. **LMS-Anschluss:** SCORM/xAPI-Export macht den Kurs OPAL-Schule-kompatibel, ohne dass OPAL den Inhalt „besitzt".
>
> **Die OER-Pointe:** Wer den Quelltext hat, kann alle fünf V-Freiheiten umsetzen — *verwahren, verwenden, verarbeiten, vermischen, verbreiten*. Das gilt mit LiaScript für *interaktive* Materialien genauso wie für reinen Text.

Sie haben jetzt das *Warum*. In der nächsten Phase bauen Sie diesen Quelltext selbst — Schritt für Schritt — aus dem Energie-Stoff, den Sie in Phase 1 erlebt haben.

> [!IMPORTANT]
> **Material für die praktische Phase**
>
> Öffnen Sie die Arbeitsvorlage direkt im **LiveEditor** — Quelltext links, gerendertes Ergebnis rechts, kein lokales Setup:
>
> 👉 [**Phase 3 im LiveEditor öffnen**](https://liascript.github.io/LiveEditor/?/show/file/https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/03_Anwenden_Vorlage.md)
>
> Halten Sie zusätzlich das zweiseitige [**Cheatsheet**](https://github.com/LiaPlayground/Opal_Schule_meets_LiaScript/blob/main/cheatSheet/cheatsheet.pdf) griffbereit — jede Aufgabe verweist über `Cheatsheet-Abschnitt: …` auf die passende Karte.

> **Auf zu [Phase 3 — Anwenden](03_Anwenden_Vorlage.md).**
