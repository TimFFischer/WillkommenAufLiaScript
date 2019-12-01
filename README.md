<!--
author:   Sebastian Zug

email:    Sebastian.Zug@informatik.tu-freiberg.de

version:  0.0.1

language: de

narrator: Deutsch Male

comment:  Try to write a short comment about
          your course, multiline is also okay.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css
script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

translation: Deutsch  translations/German.md
-->

# Willkommen bei LiaScript

--{{0}}--
Hallo, wenn Sie sich für *Open Educational Ressources* interessieren, sind Sie hier genau richtig. Wir wollen Ihnen ein neues Konzept für das "O" in O E R vorstellen, dass deutlich weitergeht als Dokumente, die auf einem Server online gestellt werden. Unser Projekt heißt "LiaScript" und erlaubt es Lehrinhalte wie ein Open Source Projekt zu realisieren. Interessiert? Dann klicken Sie auf den Pfeil nach rechts.

Wie Sie sich sicher schon denken können, entstand dieser Kurs auch auf der Basis von *LiaScript*.  Um Ihnen die Konzept vorzustellen verwenden wir die Features, die zugehörige Browserbasierte Ausführungsumgebung bereitstellt.

Sie haben die Möglichkeit diesen Kurs entweder in Buchform, als Vorlesung oder ähnlich eines Vorlesungsskriptes auszuführen. Klicken Sie dazu auf das Symbol oben rechts. Das

+ **Auge** bezeichnet die Darstellung das Vorlesungsmitschrift. Die eigentlichen Lehrinhalte werden durch zusätzliche Informationen angereichert. Den Text, den Sie gerade gehört haben, sehen Sie jetzt im unteren Bereich des Bildschirmes.

+ **Buch** definiert die Darstellung aller Inhalte in Textform. Alle Animationen und Übergänge sind in diesem Fall deaktiviert.

+ **Ohr** die zusätzlichen Informationen werden als Text-to-Speech vorgetragen. Dies vermittelt das Gefühl einer Lehrveranstaltung.

Für den Fortschritt im Kurs nutzen Sie bitte die Pfeiltasten oben. Die Darstellung links bietet einen Überblick zur Struktur des Kurses.


## Motivation


{{0-1}}
********************************************************************************

<!--
style="width: 100%; max-width: 860px; display: block; margin-left: auto; margin-right: auto;"
-->
```ascii

Version 1.0                           Version 1.1
+--------------------------+          +---------------------------+
| Kurs  Deutsche Literatur |          | Kurs  Deutsche Literatur  |
| Autor Peter Muster       | "Fehler" | Autoren Peter Muster      |
|                          |------>   |         Angelika Maier    |----->
|~~~~~~~~~~~~~~~~~~~~~~~~~~|          |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
| Ab 1756 bereiste Goethe  |---.      | Ab 1786 bereiste Goethe   |--.
| Italien ...              |   |      | Italien ...               |  |
                               |                                     |
                               |                                     |    +----------------------------+
                               |                                     |    | Kurs  German Literature    |
                               |                                     |    | Autoren Peter Muster       |
                               |                                     .--> |         Angelika Maier     |
                               |                                          |         Steve Gray         |
                               |                                          |~~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                               |                                          | In 1786 Goethe traveled to |
                               |                                          | Italy ...                  |
                               |       Version 1.0
                               |      +---------------------------+
                               |      | Kurs  Goethes Welt        |
                               |      | Autoren Peter Muster      |
                               .-->   |         Angelika Maier    |----->
                                      |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                                      | Während der italienischen |
                                      |                           |
```
*Versionen der Lehrinhalte eines Kurses und deren Wiederverwendung in anderen Veranstaltungen*

--{{0}}--
Wie sollten Lehrmaterialien entstehen, die den Stempel O E R wirklich verdienen? Zum einen sollten sie frei verfügbar sein. Lehrveranstaltungen zu einem Thema sind aber sehr unterschiedlich, die Lehrenden setzen variierende Schwerpunkte oder einen anderen Kontext. Die bloße Übernahme reicht nicht aus, vielmehr muss der Inhalt überarbeitbar sein und neu zusammengestellt werden können. Die Abbildung illustriert dies. Eine Zahl von Autoren korrigiert Fehler und entwickelt die Inhalte weiter. Dabei entstehen auch komplett neue Kurskonfigurationen beziehungsweise Übersetzungen von Inhalten.

********************************************************************************

{{1-2}}
********************************************************************************
Warum gelingt es Wikipedia dieses Konzept mit Millionen aktiver Freiwilliger erfolgreich umzusetzen.

--{{1}}--
Der Eintrag "Bundesrepublik Deutschland" blickte im Mai 2019 auf 15850 Änderungen von 3928 Nutzern zurück. Wikipedia sichert durch diese Anpassung die Aktualität und Qualität des Bestandes an Daten. Wo aber liegt der Schlüssel zum Erfolg?

| Gründe für den Erfolg von Wikipedia | Erläuterung                                                                                                                                                                                                                                                      |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Versionierungsmethode               | Wikipdia speichert die gesamte Entwicklungshistoriedes Dokumentes ab. Damit lassen sich Änderungsverläufe rekonstruieren, Versionen fusionieren und Fehler einfacher beseitigen.                                                                                 |
| Einfache Beschreibungssprache       | Die Inhalte in Wikipedia werden in einer einfachen Beschreibungssprache [wikitext](https://de.wikipedia.org/wiki/Wikitext) editiert. Anders als Word oder pdf-Dokumente sind diese einfache Textdateien, die im Browser von jedermann manipuliert werden können. |
| Integrierter Editor                                    |  Nutzer können die Änderungen in der Beschreibungssprache direkt im Browser vornehmen. Es ist kein separates Tool notwendig.                                                                                                                                                                                                                                                                |

********************************************************************************

{{2-3}}
********************************************************************************
Kann man also einfach ein Wikipedia für Lehrveranstaltungsinhalte ableiten?

--{{2}}--
Diese Frage muss eindeutig mit nein beantwortet werden. Dafür sprechen im wesentlichen drei Gründe: erstens, die zentral aufgebaute Architektur von Wikipedia, zweitens
die fehlende Möglichkeit interaktive Inhalte zu integrieren und drittens die Notwendigkeit individuelle Zustände zu speichern.

Aus der Sicht der Anforderungen an eine Plattform für dem Wissenstransfer unterliegt das
Wikipedia-Konzept folgenden Einschränkungen:

1. Die zentral ausgerichtete Architektur konzentriert alle Inhalte an einer Stelle. Es gibt also nur einen Eintrag für ein bestimmtes Thema. Das Aufsplitten und die Neukombination für individuelle Zwecke ist der Idee folgend nicht vorgesehen. Gleichzeitig erwächst aus dem zentralistischen Konzept die Notwendigkeit einer leistungsfähigen IT-Infrastruktur.

2. Wikitext erweitert die Beschreibungssprache Markdown, die für die Strukturierung von Texten insbesondere bei der Dokumentation von Softwareprojekten verwendet wird. Dabei entsteht aus den Zeilen:

```
# Überschrift 1
Das ist der Text

## Unterüberschrift 1.A
Das auch nur wird diese Wort __fett__ geschrieben
```

die Ausgabe

-------------------------------------------------------------------------------
<h2> Überschrift 1 </h2>
Das ist der Text

<h1> Unterüberschrift 1.A </h1>
Das auch nur wird diese Wort __fett__ geschrieben

Die Fokussierung auf statische Inhalte genügt aber für die Umsetzung von Lerninhalten,
die in starkem Maße auf interaktiven Elementen wie Quizzen, Simulationen oder ausführbaren Codefragmenten aufbauen, nicht.

3. Eine Lehr-Lern-Umgebung muss neben der Vermittlung von Wissen auch die Möglichkeit bieten den aktuellen Lernfortschritt des einzelnen Nutzers zu speichern.

> Die beiden letztgenannten Punkte werden durch etablierte Tools wie Moodle oder Ilias realisiert. Allerdings fehlt in diesem Kontext die Flexibilität bzw. die Versionierung über Systemgrenzen hinweg völlig.

********************************************************************************

## LiaScript

*LiaScript* zielt entsprechend darauf eine Brücke zwischen diesen beiden Welten zu
schlagen:

1.  die einfache Editierfähigkeit und die Versionierung abgeleitet von Wikipedia.
2.  die Integration relevanter Formate für interaktive Kurse sowie die Begleitung des Lernfortschrittes.

Zudem braucht es einen verteilten Ansatz, um webbasierten Lernmaterialien gemeinsam zu bearbeiten und zu nutzen, ohne dass zunächst ein Server eingerichtet oder ein spezielles Programm für die Editierung beschafft werden muss.

{{1}}
********************************************************************************

Die Beiträge von *LiaScript* dazu lassen sich wie folgt zusammenfassen:

1. erweiterte Markdownsyntax, die ein breites Spektrum an interaktiven Elementen umfasst,
2. Interpreter für die Darstellung der Inhalte im Browser,
3. Bereitstellung unterschiedlicher Präsentationsformate, die den Kurs Nutzergetrieben aufbereiten,
4. verteiltes Versionmanagment auf der Basis der Tools, die für Open Source Projekte zum Einsatz kommen und
5. ein Editor-Tool, das als Open-Source-Werkzeug frei zur Verfügung steht.

--{{1}}--
LiaScript erweitert den Sprachumfang von Markdown in vielerlei Hinsicht. Dies sind insbesondere die interaktiven Elemente wie ausführbarer Code oder Quizze. Dazu kommen statische Elemente wie die Diagramme oder Grafiken. Auf den folgenden Seiten finden Sie dazu eine Auswahl von Beispielen. Der gesamte Umfang eines LiaScript-Dokumentes wird vom Browser geladen und dann lokal durch den Interpreter dargestellt. Die dafür bereitstehenden Präsentationsformate Vorlesung, Mitschriften und Buch kennen Sie ja bereits. Im Folgenden gehen wir nun auf diese Aspekte des Projektes ein.

********************************************************************************

## A) Markdown Erweiterung

Einen guten Überblick zum "traditionellen" Sprachumfang von Markdown bietet
die Zusammenstellung auf der Webseite [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). Dies betrifft Listen, Tabelle und die Einbindung von
Bildern.

```markdown
1. Lists
2. ordered or

   * unordered
   * ones ...


| Header 1   | Header 2   |
| :--------- | :--------- |
| Item 1     | Item 2     |


Images:

![images](https://farm2.static.flickr.com/1618/26701766821_7bea494826.jpg)
```

Daraus entsteht folgende Darstellung:

1. Lists
2. ordered or

   * unordered
   * ones ...


| Header 1   | Header 2   |
| :--------- | :--------- |
| Item 1     | Item 2     |


Images:

![images](https://farm2.static.flickr.com/1618/26701766821_7bea494826.jpg)


### Medieneinbindung/ Sprachausgabe

Die Sprachausgabe haben Sie ja bereits genutzt. Diese kann mit 32 Sprachen
umgesetzt werden. Klicken Sie nach rechts um

{{1}}
********************************************************************************
... eine englische Textausgabe zu hören. Deren Ausgaben basieren wiederum nur auf dem im Dokument festgehaltenen Text. Für den gerade
gehörten englischen Text steht im Kursdokument einfach nur der Eintrag:

```
--{{1 US English Female}}--
But you can also include other features such as spoken text.
```

--{{1 US English Female}}--
But you can also include other features such as spoken text.

********************************************************************************

{{2}}
********************************************************************************

Darüber hinaus können mit

```
?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)
!?[video](https://www.youtube.com/watch?v=bICfKRyKTwE)
```

Videos und Tonsample integriert werden. Für diese existieren eigene Konfigurationsschnittstellen, die den Startzeitpunkt und die Darstellungsgröße festlegen. Starten Sie die Einträge über die Bedieninterfaces.

?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)

!?[video](https://www.youtube.com/watch?v=bICfKRyKTwE)

********************************************************************************


### Diagramme

Das in der Kursbeschreibung enthalten Diagramm wird durch den Interpreter
in eine anschauliche Form überführt. Damit sind für einfache Darstellungen
keine weiteren Werkzeuge notwendig, deren Inhalt mit jeder Iteration angepasst werden müsste.

```
                Multiline
1.9 |    DOTS
    |                 ***
  y |               *     *
  - | r r r r r r r*r r r r*r r r r r r r
  a |             *         *
  x |            *           *
  i | B B B B B * B B B B B B * B B B B B
  s |         *                 *
    | *  * *                       * *  *
 -1 +------------------------------------
      0              x-axis               1
```


                                    Multiline
    1.9 |    DOTS
        |                 ***
      y |               *     *
      - | r r r r r r r*r r r r*r r r r r r r
      a |             *         *
      x |            *           *
      i | B B B B B * B B B B B B * B B B B B
      s |         *                 *
        | *  * *                       * *  *
     -1 +------------------------------------
        0              x-axis               1

### Quizzes

### A Textquiz

What did the **fish** say when he hit a **concrete wall**?

    [[dam]]

### Multiple Choice

Just add as many points as you wish:

    [[X]] Only the **X** marks the correct point.
    [[ ]] Empty ones are wrong.
    [[X]] ...

### Single Choice

Just add as many points as you wish:

    [( )] ...
    [(X)] <-- Only the **X** is allowed.
    [( )] ...

### Ausführbarer Code

A drawing example, for demonstrating that any JavaScript library can be used, also for drawing.

```javascript
// Initialize a Line chart in the container with the ID chart1
new Chartist.Line('#chart1', {
  labels: [1, 2, 3, 4],
  series: [[100, 120, 180, 200]]
});

// Initialize a Line chart in the container with the ID chart2
new Chartist.Bar('#chart2', {
  labels: [1, 2, 3, 4],
  series: [[5, 2, 8, 3]]
});
```
<script>@input</script>

<div class="ct-chart ct-golden-section" id="chart1"></div>
<div class="ct-chart ct-golden-section" id="chart2"></div>

## C) Verteiltes Versionmanagment

Link auf diesen Kurs


## D) Editor
