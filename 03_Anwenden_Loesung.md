<!--
author:   Sebastian Zug
email:    sebastian.zug@informatik.tu-freiberg.de
version:  0.1.0
language: de
narrator: Deutsch Male

comment:  Musterlösung zur Mini-Lerneinheit
          "Energie — kinetische und potentielle Energie".
          Entstanden im Rahmen des Workshops
          "OPAL Schule meets LiaScript" am 28.05.2026
          für die Referent:innen der Medienpädagogischen Zentren.

import:   https://github.com/LiaTemplates/Pyodide

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Opal_Schule_meets_LiaScript/main/03_Anwenden_Loesung.md)

# Energie — kinetische und potentielle Energie

<!---
============================================================
TEIL 1 — DEN KURS IN BETRIEB NEHMEN
============================================================

------------------------------------------------------------
AUFGABE 1 — Header personalisieren  ✅ GELÖST
Cheatsheet-Abschnitt: YAML-Header

Im YAML-Header oben sind author, email und comment ausgefüllt.
Zusätzlich wurde der Pyodide-Import ergänzt, damit der Code-Block
in Aufgabe 15 funktioniert.
------------------------------------------------------------
--->


<!---
------------------------------------------------------------
AUFGABE 2 — Einleitungsabsatz formatieren  ✅ GELÖST
Cheatsheet-Abschnitt: Textauszeichnung

Zentrale Fachbegriffe sind **fett**, alltagssprachliche
Wendungen *kursiv*. Der ursprünglich lange Absatz wurde
in zwei Paragraphen aufgeteilt.
------------------------------------------------------------
--->

**Energie** im physikalischen Sinne ist streng vom alltagssprachlichen Gebrauch zu unterscheiden. Im Alltag wird sie eher als Stimmungszustand verstanden, etwa in Sätzen wie *„Ich habe keine Energie"* oder *„Wir verbrauchen zu viel Energie"*.

Im physikalischen Sinne gibt **Energie** die **Fähigkeit an, etwas zu verrichten**. Energie ist eine *Zustandsgröße* und wird in der Einheit **Joule (J)** gemessen — benannt nach James Prescott Joule.


<!---
------------------------------------------------------------
AUFGABE 3 — Überschriften und Subüberschriften  ✅ GELÖST
Cheatsheet-Abschnitt: Überschriften

Die Zeile "Worum geht es?" ist jetzt eine ##-Überschrift.
Weitere Abschnitte unten wurden ebenfalls mit ## ausgezeichnet,
damit die Navigation am rechten Rand übersichtlich wird.
------------------------------------------------------------
--->

## Worum geht es?


<!---
------------------------------------------------------------
AUFGABE 4 — Lernziele als Liste  ✅ GELÖST
Cheatsheet-Abschnitt: Listen

Die vier Lernziele stehen als ungeordnete Liste (mit -).
Eine geordnete Variante (1. 2. 3.) wäre genauso möglich —
inhaltlich kein Unterschied, didaktisch aber: nummerierte
Listen suggerieren eine Reihenfolge, ungeordnete eher
gleichrangige Punkte.
------------------------------------------------------------
--->

Am Ende dieser Lerneinheit können Sie:

- den Begriff **Energie** physikalisch definieren und vom alltagssprachlichen Gebrauch abgrenzen,
- **kinetische** und **potentielle Energie** unterscheiden,
- die zugehörigen Formeln auf konkrete Aufgaben anwenden,
- die **Einheit Joule** benennen und in andere Einheiten umrechnen.


<!---
------------------------------------------------------------
AUFGABE 5 — Tabelle der Energiearten  ✅ GELÖST
Cheatsheet-Abschnitt: Tabellen

Drei Spalten, drei Zeilen. In der zweiten Spalte sind die
Formeln direkt als LaTeX gesetzt (siehe Aufgabe 6) — so
sind beide Aufgaben in einem Schritt erledigt.
------------------------------------------------------------
--->

## Die drei Energiearten im Überblick

| Energieart              | Formel                                  | Anwendung im Alltag                                |
| ----------------------- | --------------------------------------- | -------------------------------------------------- |
| **Kinetische Energie**  | $E_\text{kin} = \tfrac{1}{2}\, m\, v^2$ | fahrendes Auto, fliegender Ball, rotierende Welle |
| **Potentielle Energie** | $E_\text{pot} = m\, g\, h$              | gehobene Werkzeugkiste am Kran, Stausee, Gipfel    |
| **Spannenergie**        | $E_\text{spann} = \tfrac{1}{2}\, D\, s^2$ | gespannte Feder, gedehntes Gummiband, Bogen        |


<!---
------------------------------------------------------------
AUFGABE 6 — Mathematische Formeln  ✅ GELÖST
Cheatsheet-Abschnitt: Mathematische Formeln (LaTeX)

Die zerlegten Unicode-Schnipsel (𝐸𝑘𝑖𝑛=12⋅𝑚⋅𝑣2) wurden durch
saubere LaTeX-Formeln ersetzt. Wir nutzen $...$ inline und
$$...$$ als Block, wenn die Formel zentral hervorgehoben werden
soll. Indizes werden mit _, Brüche mit \tfrac und Quadrate
mit ^2 gesetzt.
------------------------------------------------------------
--->

Kinetische Energie:

$$E_\text{kin} = \tfrac{1}{2}\, m\, v^2$$

Potentielle Energie:

$$E_\text{pot} = m\, g\, h$$


<!---
------------------------------------------------------------
AUFGABE 7 — Hinweis-Boxen (Callouts)  ✅ GELÖST
Cheatsheet-Abschnitt: Hinweise / Callouts

Der Absatz wurde in einen [!TIP]-Block umgewandelt. Damit
wird die didaktisch wichtigste Aussage des Kapitels visuell
hervorgehoben — Lernende erkennen sofort: "Das soll ich
mir merken."
------------------------------------------------------------
--->

> [!TIP]
> Eine **Besonderheit** der kinetischen Energie: Die Geschwindigkeit geht **quadratisch** ein.
>
> Eine **Verdopplung** der Geschwindigkeit führt zu einer **Vervierfachung** der Energie — eine Verdreifachung sogar zu einer Verneunfachung. Genau das erklärt, warum Bremswege im Straßenverkehr so dramatisch von der Geschwindigkeit abhängen.


<!---
============================================================
TEIL 2 — INTERAKTIVE ELEMENTE
============================================================

------------------------------------------------------------
AUFGABE 8 — Bild einbinden  ✅ GELÖST
Cheatsheet-Abschnitt: Bilder

Das Pendel-Bild aus Wikimedia Commons ist eingebunden, mit
sprechendem Alternativtext für barrierefreie Nutzung.
Die Original-Quelle (Wikimedia) ist in der Bildunterschrift
verlinkt — wichtig für die korrekte CC-Attribuierung.
------------------------------------------------------------
--->

## Vom Pendel zum Energiebegriff

![Schematische Darstellung eines schwingenden Pendels mit eingezeichneten Energieformen](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4f/Pendulum.svg/200px-Pendulum.svg.png)

*Schwingendes Pendel — Bildquelle: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Pendulum.svg), Public Domain.*


<!---
------------------------------------------------------------
AUFGABE 9 — Video einbetten  ✅ GELÖST
Cheatsheet-Abschnitt: Video

Mit !?[Beschreibung](URL) bettet LiaScript das YouTube-Video
direkt in die Seite ein — Lernende verlassen den Kurs nicht.
Beachten Sie: Eingebettete Videos sind kein Hosting der Videos
selbst, sondern ein Verweis. Bei Lizenzfragen also weiterhin
prüfen, ob das Video tatsächlich CC-lizenziert ist oder ob es
sich nur um eine erlaubte Einbettung handelt.
------------------------------------------------------------
--->

Ein kurzer Überblick zum Begriff der Energie:

!?[Energieformen — eine Einführung](https://www.youtube.com/watch?v=5MQRsacRJlw)


<!---
------------------------------------------------------------
AUFGABE 10 — PhET-Simulation einbetten  ✅ GELÖST
Cheatsheet-Abschnitt: Eingebettete Ressource

Die PhET-Simulation wird über die LiaScript-eigene Syntax
??[Kurztitel](URL "Titel") eingebettet — kein iframe nötig.
LiaScript erkennt das Format automatisch und bindet die Sim
direkt in die Seite ein. Direkt darunter steht die
Aufgabenstellung, damit Lernende beim Experimentieren nicht
zwischen Sim und Aufgabentext hin- und herscrollen müssen.

------------------------------------------------------------
--->

## Experimentieren mit dem Energie-Skatepark

<!-- style="height: 600px;" -->
??[PhET-Simulation: Energie-Skatepark](https://phet.colorado.edu/sims/html/energy-skate-park/latest/energy-skate-park_de.html "Energie im Skaterpark")

> **Aufgabenstellung:**
>
> 1. Ziehen Sie die Skaterin auf die Halfpipe und lassen Sie sie los.
> 2. Öffnen Sie über das **grüne Plus** oben links die Energie-Übersicht.
> 3. Beobachten Sie die Balken für **kinetische** und **potentielle** Energie — wann ist welcher Balken maximal?
> 4. Was passiert mit der **Gesamtenergie**?


<!---
============================================================
TEIL 3 — QUIZ UND LERNSTANDSERFASSUNG
============================================================

------------------------------------------------------------
AUFGABE 11 — Einfachauswahl-Quiz  ✅ GELÖST
Cheatsheet-Abschnitt: Quizformate / Einfachauswahl

Vier Optionen, eine richtige Antwort (Joule).
Die Distraktoren sind bewusst eng am Thema gewählt:
  • Newton ist die Einheit der Kraft — typische Verwechslung
  • Watt ist die Einheit der Leistung — auch häufig verwechselt
  • Pascal ist die Einheit des Drucks — Distraktor zur Abgrenzung
------------------------------------------------------------
--->

## Selbsttest

**Frage 1:** Welche Einheit hat die Energie?

- [( )] Newton (N)
- [(X)] Joule (J)
- [( )] Watt (W)
- [( )] Pascal (Pa)


<!---
------------------------------------------------------------
AUFGABE 12 — Zahleneingabe-Quiz  ✅ GELÖST
Cheatsheet-Abschnitt: Quizformate / Zahleneingabe

Lösung: E_kin = 1/2 · 4 · 27² = 1458 J
Die erwartete Zahl steht in doppelten eckigen Klammern.
LiaScript akzeptiert verschiedene Eingabeformate
(1458 / 1458.0 / 1.458e3). Mehr Toleranz bei Fließkommazahlen
kann mit der Notation [[1458 ± 1]] erreicht werden.
------------------------------------------------------------
--->

**Frage 2:** Ein Ball mit der Masse $m = 4\,\text{kg}$ rollt mit der Geschwindigkeit $v = 27\,\text{m/s}$. Berechnen Sie $E_\text{kin}$ in Joule.

[[1458]]


<!---
------------------------------------------------------------
AUFGABE 13 — Mehrfachauswahl-Quiz  ✅ GELÖST
Cheatsheet-Abschnitt: Quizformate / Mehrfachauswahl

Mehrere richtige Antworten. Hier ein didaktisch interessanter
Fall: Geschwindigkeit v ist KEINE Größe, von der E_pot abhängt —
sie taucht in der Formel m·g·h schlicht nicht auf. Die anderen
drei Größen (m, h, g) gehen alle direkt ein.
Die Frage prüft also, ob die Lernenden die Formel formal lesen
können — nicht nur "irgendetwas mit Energie".
------------------------------------------------------------
--->

**Frage 3:** Von welchen Größen hängt die **potentielle Energie** $E_\text{pot} = m\,g\,h$ ab? *(Mehrere Antworten sind möglich.)*

- [[X]] Masse $m$
- [[X]] Höhe $h$
- [[ ]] Geschwindigkeit $v$
- [[X]] Gravitationsbeschleunigung $g$


<!---
------------------------------------------------------------
AUFGABE 14 — Hinweis und ausklappbare Lösung  ✅ GELÖST
Cheatsheet-Abschnitt: Hinweise & Spoiler

Wir nutzen ZWEI Stufen der Unterstützung:
  Stufe 1: Hinweis-Pfeil [[?]] - zeigt einen kurzen Tipp
  Stufe 2: Sternchen-Block (********) - klappt den vollen
           Lösungsweg auf, direkt unter dem Quiz angekoppelt
Diese zweistufige Hilfe ist eine sehr wirksame Form der
Binnendifferenzierung: Schnelle SuS klicken gar nicht, mittlere
brauchen den Tipp, schwächere sehen sich den Lösungsweg an.
Im Zahleneingabe-Quiz (Frage 2) eingefügt.
------------------------------------------------------------
--->

**Frage 2 (mit Hilfe):** Ein Ball mit der Masse $m = 4\,\text{kg}$ rollt mit der Geschwindigkeit $v = 27\,\text{m/s}$. Berechnen Sie $E_\text{kin}$ in Joule.

[[1458]]

- [[?]] Hinweis: Die Formel lautet $E_\text{kin} = \tfrac{1}{2}\, m\, v^2$ — achten Sie auf das **Quadrat**.
- [[?]] Stolperstelle: Erst $27^2 = 729$, dann $\cdot 4 = 2916$, dann $\cdot \tfrac{1}{2} = 1458$.

***********************************************

$$E_\text{kin} = \tfrac{1}{2} \cdot 4\,\text{kg} \cdot (27\,\text{m/s})^2 = 2 \cdot 729\,\text{J} = 1458\,\text{J}$$

***********************************************


<!---
============================================================
TEIL 4 — AUSFÜHRBARER CODE
============================================================

------------------------------------------------------------
AUFGABE 15 — Python-Code-Block  ✅ GELÖST
Cheatsheet-Abschnitt: Code-Blöcke

Der Python-Code wird via Pyodide direkt im Browser ausgeführt
— ohne lokales Setup. Voraussetzung ist der Import oben im
YAML-Header. Über `@Pyodide.eval` direkt nach dem Code-Block
wird der Ausführen-Button (▶) eingeblendet.

Wir haben den Code zusätzlich verallgemeinert: Eine Schleife
über mehrere Geschwindigkeiten zeigt eindrücklich den
quadratischen Zusammenhang aus Aufgabe 7.
------------------------------------------------------------
--->

## Energie berechnen — direkt im Browser

```python   e_kin.py
m = 4   # Masse in kg

# Tabelle für verschiedene Geschwindigkeiten
print(f"{'v in m/s':>10} | {'E_kin in J':>12}")
print("-" * 27)
for v in [3, 6, 9, 12, 27]:
    E_kin = 0.5 * m * v**2
    print(f"{v:>10} | {E_kin:>12.1f}")
```
@Pyodide.eval

> [!NOTE]
> Beobachten Sie: Von $v = 3$ auf $v = 6$ (Verdopplung) vervierfacht sich $E_\text{kin}$ — genau das Quadrat aus Aufgabe 7. Probieren Sie auch andere Massen aus, indem Sie `m = 4` ändern.


<!---
============================================================
TEIL 5 — FREIE GESTALTUNG  ✅ BEISPIEL-AUSARBEITUNG
============================================================

Eine mögliche Ergänzung ist hier gezeigt:
  • eine Lernfortschritts-Checkliste,
  • eine ASCII-Skizze einer Energieumwandlung,
  • eine Differenzierungsaufgabe für leistungsstärkere SuS.

Selbstverständlich gibt es viele weitere gute Wege —
diese Ausarbeitung ist ein Anstoß, kein Maßstab.

============================================================
--->

## Lernfortschritt — meine persönliche Bilanz

- [ ] Ich kann **Energie** physikalisch definieren.
- [ ] Ich kenne die **Einheit Joule** und kann sie zuordnen.
- [ ] Ich kann **$E_\text{kin}$** für eine gegebene Masse und Geschwindigkeit berechnen.
- [ ] Ich kann **$E_\text{pot}$** für eine gegebene Masse und Höhe berechnen.
- [ ] Ich verstehe, **warum** die Geschwindigkeit quadratisch eingeht.

## Energieumwandlung — eine Skizze

```ascii
                              höchster Punkt
                                    ●
                                   / \
                                  /   \           E_pot maximal
                                 /     \          E_kin = 0
                                /       \
                               /         \
                              /           \
                             /             \
                            ●               ●
                       Schwung                Schwung
                                ↓
                            tiefster Punkt
                                ●
                              ─────              E_pot minimal
                                                  E_kin maximal
```

> [!NOTE]
> Eine ASCII-Skizze ist nicht das hochwertigste Diagramm — aber sie hat einen unschlagbaren Vorteil: Sie steht **direkt im Markdown**, ist versionierbar, suchbar, und übersteht Copy-Paste in jedes Lehrwerk. Für die schnelle Visualisierung im Unterricht oft genau richtig.

## Differenzierungsaufgabe für Fortgeschrittene

> [!TIP]
> **Knifflige Zusatzfrage:** Eine Skaterin der Masse $m = 60\,\text{kg}$ startet in $h = 4\,\text{m}$ Höhe aus der Ruhe. Welche **Geschwindigkeit** erreicht sie idealisiert (ohne Reibung) am tiefsten Punkt?

[[8.85]]

- [[?]] Hinweis: Im idealisierten Fall gilt $E_\text{pot, oben} = E_\text{kin, unten}$. Also $m\,g\,h = \tfrac{1}{2}\,m\,v^2$ — und $m$ kürzt sich heraus.
- [[?]] Mit $g = 9{,}81\,\text{m/s}^2$ ergibt sich $v = \sqrt{2\,g\,h}$.

***********************************************

Aus dem Energieerhaltungssatz folgt:

$$m\,g\,h = \tfrac{1}{2}\,m\,v^2 \quad\Longleftrightarrow\quad v = \sqrt{2\,g\,h}$$

Einsetzen:

$$v = \sqrt{2 \cdot 9{,}81\,\text{m/s}^2 \cdot 4\,\text{m}} = \sqrt{78{,}48}\,\text{m/s} \approx 8{,}85\,\text{m/s}$$

Bemerkenswert: Die **Masse fällt heraus**. Eine schwere und eine leichte Skaterin erreichen idealisiert dieselbe Endgeschwindigkeit — Galilei lässt grüßen.

***********************************************
