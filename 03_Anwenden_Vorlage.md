<!--
author:   IHR NAME
email:    ihre.mail@medienzentrum.de
version:  0.1.0
language: de
narrator: Deutsch Male

comment:  Mini-Lerneinheit "Energie — kinetische und potentielle Energie"
          — entstanden im Rahmen des Workshops
          "OPAL Schule meets LiaScript" am 28.05.2026.

-->

# Energie — kinetische und potentielle Energie

> [!TIP]
> **Ihre Werkzeug-Handreichung:** Zu jeder Aufgabe gehört ein Abschnitt auf dem zweiseitigen **[LiaScript-Cheatsheet](cheatSheet/cheatsheet.pdf)** (Seite 1 = Markdown, Seite 2 = LiaScript-Erweiterungen). Die Zeile `Cheatsheet-Abschnitt: …` in jeder Aufgabe nennt die passende Karte — dort finden Sie Syntax *und* Wirkung nebeneinander. Halten Sie das Blatt während der Hands-on-Phase griffbereit.


<!---
============================================================
TEIL 1 — DEN KURS IN BETRIEB NEHMEN
============================================================

------------------------------------------------------------
AUFGABE 1 — Header personalisieren
Cheatsheet-Abschnitt: YAML-Header

Öffnen Sie den Kommentar-Block ganz oben und tragen Sie ein:
  • Ihren Namen
  • Ihre E-Mail-Adresse
  • Ihre Einrichtung (im comment-Feld)

Speichern und Vorschau prüfen.
------------------------------------------------------------
--->


<!---
------------------------------------------------------------
AUFGABE 2 — Einleitungsabsatz formatieren
Cheatsheet-Abschnitt: Textauszeichnung

Formatieren Sie den nachfolgenden Absatz so, dass die zentralen
Begriffe **fett** und alltagssprachliche Wendungen *kursiv* sind.
Experimentieren Sie auch mit neuen Paragraphen über Leerzeilen.
------------------------------------------------------------
--->

Energie im physikalischen Sinne ist streng vom alltagssprachlichen Gebrauch zu unterscheiden. Im Alltag wird sie eher als Stimmungszustand verstanden, etwa in Sätzen wie Ich habe keine Energie oder Wir verbrauchen zu viel Energie. Im physikalischen Sinne gibt Energie die Fähigkeit an, etwas zu verrichten. Energie ist eine Zustandsgröße und wird in der Einheit Joule (J) gemessen, benannt nach James Prescott Joule.


<!---
------------------------------------------------------------
AUFGABE 3 — Überschriften und Subüberschriften
Cheatsheet-Abschnitt: Überschriften

Texte werden durch Überschriften strukturiert. Die Hauptüberschrift
(`#`) steht bereits oben. Ergänzen Sie nun `##` vor den passenden
Zeilen weiter unten, um Abschnitte zu bilden. Speichern Sie und
beobachten Sie, wie sich die Navigation in der Vorschau aufbaut.
------------------------------------------------------------
--->

Worum geht es?


<!---
------------------------------------------------------------
AUFGABE 4 — Lernziele als Liste
Cheatsheet-Abschnitt: Listen

Ersetzen Sie diesen Kommentar durch eine ungeordnete Liste mit
drei bis vier Lernzielen. Vorschläge:
  • Den Begriff Energie definieren
  • Kinetische und potentielle Energie unterscheiden
  • Die zugehörigen Formeln anwenden
  • Die Einheit Joule benennen

Experimentieren Sie auch mit nummerierten Listen (1. 2. 3.).
------------------------------------------------------------
--->


<!---
---------------------^---------------------------------------
AUFGABE 5 — Tabelle der Energiearten
Cheatsheet-Abschnitt: Tabellen

Bauen Sie eine Tabelle mit drei Spalten:
  Energieart | Formel | Anwendung im Alltag

Drei Zeilen: kinetische, potentielle, Spannenergie.
Tipp: Die Pipe `|` trennt Spalten. Die zweite Zeile mit
`---` definiert die Trennlinie.
------------------------------------------------------------
--->

Die drei Energiearten im Überblick

| Energieart              | Formel                                  | Anwendung im Alltag                                |
| ----------------------- | --------------------------------------- | -------------------------------------------------- |
| **Kinetische Energie**  | $E_\text{kin} = \tfrac{1}{2}\, m\, v^2$ | fahrendes Auto, fliegender Ball, rotierende Welle |


<!---
------------------------------------------------------------
AUFGABE 6 — Mathematische Formeln
Cheatsheet-Abschnitt: Mathematische Formeln (LaTeX)

Fügen Sie die folgenden Formeln als LaTeX ein, eingerahmt von
einfachen Dollarzeichen $...$ (Inline) bzw. doppelten $$...$$
(als Block, mittig gesetzt).

Ersetzen Sie weiter unten den Unicode-Schnipsel durch saubere
LaTeX-Formeln.
------------------------------------------------------------
--->

Kinetische Energie:  $E_\text{kin} = \tfrac{1}{2}\, m\, v^2$

Potentielle Energie:  𝐸p𝑜𝑡=𝑚⋅𝑔⋅ℎ


<!---
------------------------------------------------------------
AUFGABE 7 — Hinweis-Boxen (Callouts)
Cheatsheet-Abschnitt: Hinweise / Callouts

LiaScript kennt mehrere Hinweis-Typen:

  > [!TIP]   gelb: Definitionen, Hinweise
  > [!NOTE]  blau: Lese-Empfehlungen
  > [!WARNING]  rot: Stolperfallen

Wandeln Sie den folgenden Absatz in einen `[!TIP]`-Block um,
der die Besonderheit der kinetischen Energie hervorhebt.
------------------------------------------------------------
--->

Eine Besonderheit der kinetischen Energie ist, dass die Geschwindigkeit quadratisch eingeht. Eine Verdopplung der Geschwindigkeit führt zu einer Vervierfachung der Energie.


<!---
============================================================
TEIL 2 — INTERAKTIVE ELEMENTE
============================================================

------------------------------------------------------------
AUFGABE 8 — Bild einbinden
Cheatsheet-Abschnitt: Bilder

Fügen Sie ein Bild ein, das eine Form von kinetischer oder
potentieller Energie illustriert. Vorschlag aus Wikimedia
Commons (frei lizenziert):
  https://upload.wikimedia.org/wikipedia/commons/thumb/4/4f/Pendulum.svg/200px-Pendulum.svg.png

Syntax:  ![Alternativtext](URL)
Vergessen Sie den Alternativtext nicht — er ist wichtig für
barrierefreie Lehrmaterialien.
------------------------------------------------------------
--->


<!---
------------------------------------------------------------
AUFGABE 9 — Video einbetten
Cheatsheet-Abschnitt: Video

LiaScript bettet YouTube-Videos automatisch ein, wenn Sie die
URL einfach in einer eigenen Zeile schreiben:

  !?[Kurze Beschreibung](https://www.youtube.com/watch?v=...)

Suchen Sie ein passendes Erklärvideo zur kinetischen oder
potentiellen Energie (z.B. von "musstewissen Physik") und
betten Sie es hier ein. Achten Sie auf die Lizenz.
------------------------------------------------------------
--->


<!---
------------------------------------------------------------
AUFGABE 10 — PhET-Simulation einbetten
Cheatsheet-Abschnitt: Eingebettete Ressource

Betten Sie die PhET-Simulation zum Energie-Skatepark direkt
in die Seite ein. LiaScript hat dafür eine eigene Syntax —
**kein iframe** nötig:

  ??[Kurztitel](URL "Titel mit Untertitel")

Das doppelte Fragezeichen ?? sagt LiaScript: "diese Ressource
einbetten" (statt nur zu verlinken). Format wird automatisch
erkannt — PhET, GeoGebra, PDF, oEmbed …

Die deutsche Variante finden Sie unter:
  https://phet.colorado.edu/sims/html/energy-skate-park/latest/energy-skate-park_de.html

------------------------------------------------------------
--->


<!---
============================================================
TEIL 3 — QUIZ UND LERNSTANDSERFASSUNG
============================================================

------------------------------------------------------------
AUFGABE 11 — Einfachauswahl-Quiz
Cheatsheet-Abschnitt: Quizformate / Einfachauswahl

Bauen Sie ein Einfachauswahl-Quiz. Die Syntax lautet:

  Frage hier?

  - [( )] falsche Antwort
  - [(X)] richtige Antwort
  - [( )] noch eine falsche Antwort

Aufgabe für die Klasse: "Welche Einheit hat die Energie?"
Optionen: Newton, Joule, Watt, Pascal.
------------------------------------------------------------
--->


<!---
------------------------------------------------------------
AUFGABE 12 — Zahleneingabe-Quiz
Cheatsheet-Abschnitt: Quizformate / Zahleneingabe

Bauen Sie ein Zahleneingabe-Quiz. Die Syntax lautet:

  Frage hier?

  [[Erwartete Zahl]]

Beispielaufgabe (aus dem OPAL-Original):

  Ein Ball mit Masse m = 4 kg rollt mit v = 27 m/s.
  Berechnen Sie E_kin in Joule.

Die Lösung ist 1458 J.
------------------------------------------------------------
--->


<!---
------------------------------------------------------------
AUFGABE 13 — Mehrfachauswahl-Quiz
Cheatsheet-Abschnitt: Quizformate / Mehrfachauswahl

Bauen Sie ein Mehrfachauswahl-Quiz. Die Syntax lautet:

  Frage?

  - [[X]] richtig
  - [[ ]] falsch
  - [[X]] richtig

Aufgabe: "Wovon hängt die potentielle Energie E_pot ab?"
Optionen: Masse m (richtig), Höhe h (richtig),
Geschwindigkeit v (falsch), Gravitation g (richtig).
------------------------------------------------------------
--->


<!---
------------------------------------------------------------
AUFGABE 14 — Hinweis und ausklappbare Lösung
Cheatsheet-Abschnitt: Hinweise & Spoiler

Ergänzen Sie das Zahleneingabe-Quiz aus Aufgabe 12 um:
  • einen Hinweis  - [[?]] Hinweis-Text hier
  • einen ausklappbaren Lösungsblock direkt unter dem Quiz:

    ***********************************************
    Lösungsweg:

    E_kin = 1/2 · 4 kg · (27 m/s)² = 1458 J
    ***********************************************

LiaScript erkennt zwei Zeilen mit vielen Sternchen als
Begrenzung eines ausklappbaren Blocks und koppelt ihn
automatisch an das direkt darüber stehende Quiz.

So bekommen die Lernenden Unterstützung in zwei Stufen:
erst ein Tipp, dann der volle Lösungsweg.
------------------------------------------------------------
--->


<!---
============================================================
TEIL 4 — AUSFÜHRBARER CODE (OPTIONAL, FORTGESCHRITTEN)
============================================================

------------------------------------------------------------
AUFGABE 15 — Python-Code-Block
Cheatsheet-Abschnitt: Code-Blöcke

LiaScript kann Python-Code direkt im Browser ausführen
(über Pyodide). Voraussetzung: Im YAML-Header oben muss
`import: https://github.com/LiaTemplates/Pyodide` stehen.

Bauen Sie einen Code-Block, der die kinetische Energie für
verschiedene Werte berechnet:

  ```python  e_kin.py
  m = 4      # Masse in kg
  v = 27     # Geschwindigkeit in m/s
  E_kin = 0.5 * m * v**2
  print(f"Kinetische Energie: {E_kin} J")
  ```
  @Pyodide.eval

Achten Sie auf das `@Pyodide.eval` direkt unterhalb des Code-Blocks
— ohne diese Zeile wird der Code nicht ausführbar.
------------------------------------------------------------
--->


<!---
============================================================
TEIL 5 — FREIE GESTALTUNG
============================================================

Hier ist Platz für Ihre eigenen Ergänzungen:
  • Eine Lernfortschritts-Checkliste mit `- [ ] Punkt`
  • Eine ASCII-Skizze einer Energieumwandlung
  • Ein Verweis auf ein weiterführendes Material
  • Eine Differenzierungsaufgabe für leistungsstärkere SuS
  • ...

Tauschen Sie sich am Ende mit Ihren Nachbar:innen aus —
welche Idee aus Ihrem eigenen Unterricht würden Sie hier
ergänzen?

============================================================
--->
