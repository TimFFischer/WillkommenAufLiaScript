<!--
author:   Sebastian Zug

email:    Sebastian.Zug@informatik.tu-freiberg.de

version:  0.0.2

language: de

narrator: Deutsch Male

mode:     Presentation

comment:  Dieser Kurs für in das Projekt LiaScript ein und diskutiert die
          Vorteile im Kontext der OER Idee.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

import: https://raw.githubusercontent.com/LiaTemplates/Rextester/master/README.md

translation: Deutsch  translations/German.md

-->

# Willkommen bei LiaScript

    --{{0}}--
Hallo, wenn Sie sich für *Open Educational Ressources* interessieren, sind Sie
hier genau richtig. Wir wollen Ihnen ein neues Konzept für das "O" in O E R
vorstellen, dass deutlich weitergeht als Dokumente, die auf einem Server online
gestellt werden. Unser Projekt heißt "LiaScript" und erlaubt es Lehrinhalte wie
ein Open Source Projekt zu realisieren. Interessiert? Dann klicken Sie auf den
Pfeil nach rechts.

Wie Sie sich sicher schon denken können, entstand dieser Kurs auch auf der Basis
von *LiaScript*.  Um Ihnen die Konzept vorzustellen verwenden wir die Features,
die zugehörige Browserbasierte Ausführungsumgebung bereitstellt.

Sie haben die Möglichkeit diesen Kurs entweder in Buchform, als Vorlesung oder
ähnlich eines Vorlesungsskriptes auszuführen. Klicken Sie dazu auf das Symbol
oben rechts. Das

+ **Auge** bezeichnet die Darstellung das Vorlesungsmitschrift. Die eigentlichen
  Lehrinhalte werden durch zusätzliche Informationen angereichert. Den Text, den
  Sie gerade gehört haben, sehen Sie jetzt im unteren Bereich des Bildschirmes.

+ **Buch** definiert die Darstellung aller Inhalte in Textform. Alle Animationen
  und Übergänge sind in diesem Fall deaktiviert.

+ **Ohr** die zusätzlichen Informationen werden als Text-to-Speech vorgetragen.
  Dies vermittelt das Gefühl einer Lehrveranstaltung.

Für den Fortschritt im Kurs nutzen Sie bitte die Pfeiltasten oben. Die
Darstellung links bietet einen Überblick zur Struktur des Kurses.

<<<<<<< HEAD
--------------------------------------------------------------------------

Die interaktive Version zu diesem Kurs können Sie unter [LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/SebastianZug/WillkommenAufLiaScript/master/README.md#1) starten.
=======
Die interaktive Version zu diesem Kurs können Sie unter
[LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/SebastianZug/WillkommenAufLiaScript/master/README.md#1)
starten.
>>>>>>> f679bbdb2b2a260f5107aa91edd87d00902bc0ad

Der vollständige "Code" ist unter
[GitHub](https://github.com/SebastianZug/WillkommenAufLiaScript/blob/master/README.md)
zu finden.

![Logo](./images/logo.png)<!-- width="20%" -->


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
                                      | Reise ...                 |
```
*Versionen der Lehrinhalte eines Kurses und deren Wiederverwendung in anderen Veranstaltungen*

    --{{0}}--
Wie sollten Lehrmaterialien entstehen, die den Stempel O E R wirklich verdienen?
Zum einen sollten sie frei verfügbar sein. Lehrveranstaltungen zu einem Thema
sind aber sehr unterschiedlich, die Lehrenden setzen variierende Schwerpunkte
oder einen anderen Kontext. Die bloße Übernahme reicht nicht aus, vielmehr muss
der Inhalt überarbeitbar sein und neu zusammengestellt werden können. Die
Abbildung illustriert dies. Eine Zahl von Autoren korrigiert Fehler und
entwickelt die Inhalte weiter. Dabei entstehen auch komplett neue
Kurskonfigurationen beziehungsweise Übersetzungen von Inhalten.

********************************************************************************


     {{1-2}}
********************************************************************************

Warum gelingt es Wikipedia dieses Konzept mit Millionen aktiver Freiwilliger
erfolgreich umzusetzen.

    --{{1}}--
Der Eintrag "Bundesrepublik Deutschland" blickte im Mai 2019 auf 15850
Änderungen zurück. Dazu haben 3928 Nutzer beigetragen. Wikipedia sichert so die
Aktualität und Qualität des Bestandes an Daten. Wo aber liegt der Schlüssel zum
Erfolg?

| Gründe für den Erfolg von Wikipedia | Erläuterung                                                                                                                                                                                                                                                      |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Versionierungsmethode               | Wikipdia speichert die gesamte Entwicklungshistoriedes Dokumentes ab. Damit lassen sich Änderungsverläufe rekonstruieren, Versionen fusionieren und Fehler einfacher beseitigen.                                                                                 |
| Einfache Beschreibungssprache       | Die Inhalte in Wikipedia werden in einer einfachen Beschreibungssprache [wikitext](https://de.wikipedia.org/wiki/Wikitext) editiert. Anders als Word oder pdf-Dokumente sind diese einfache Textdateien, die im Browser von jedermann manipuliert werden können. |
| Integrierter Editor                 | Nutzer können die Änderungen in der Beschreibungssprache direkt im Browser vornehmen. Es ist kein separates Tool notwendig.                                                                                                                                      |

********************************************************************************

     {{2-3}}
********************************************************************************

Kann man also einfach ein Wikipedia für Lehrveranstaltungsinhalte ableiten?

    --{{2}}--
Kann man also einfach ein Wikipedia für Lehrveranstaltungsinhalte ableiten?
Diese Frage muss eindeutig mit nein beantwortet werden. Dafür sprechen im
wesentlichen drei Gründe: erstens, die zentral aufgebaute Architektur von
Wikipedia, zweitens die fehlende Möglichkeit interaktive Inhalte zu integrieren.
Und drittens die eingeschränkten Möglichkeiten individuelle Zustände zu
speichern.

Aus der Sicht der Anforderungen an eine Plattform für dem Wissenstransfer
unterliegt das Wikipedia-Konzept zwei zentralen Einschränkungen:

1. Die zentral ausgerichtete Konzept konzentriert alle Inhalte an einer Stelle.
   Es gibt also nur einen Eintrag für ein bestimmtes Thema. Das Aufsplitten und
   die Neukombination für individuelle Zwecke ist der Idee folgend nicht
   vorgesehen. Gleichzeitig erwächst aus dem zentralistischen Konzept die
   Notwendigkeit einer leistungsfähigen IT-Infrastruktur.

2. Wikitext definiert eine Beschreibungssprache
   [Markdown](https://de.wikipedia.org/wiki/Markdown), die für die
   Strukturierung von Texten insbesondere bei der Dokumentation von
   Softwareprojekten verwendet wird. Dabei entsteht aus den Zeilen:

<table border="1" width="100%" >
<tr>
  <th>Markdown Dokument</th>
  <th>Ergebnis nach dem Rendering</th>
</tr>
  <tr>
    <td width="50%"><pre><code>
 # Überschrift 1
 Das ist der Text

 ## Unterüberschrift 1.A
 Das auch nur wird diese Wort __fett__ geschrieben</code></pre> </td>
    <td width="50%"><h2> Überschrift 1 </h2>
    Das ist der Text

    <h1> Unterüberschrift 1.A </h1>
    Das auch nur wird diese Wort __fett__ geschrieben
    </td>
  </tr>
</table>

Die einfache Semantik ist für statische Dokumente von Vorteil aber in Bezug auf
Lerninhalte gleichzeitig die größte Einschränkung. Interaktiven Elementen wie
Quizze, Simulationen oder ausführbare Codefragmente sind damit nicht umsetzbar.

Etablierte Lernumgebungen Moodle oder Ilias realisieren den letztgenannten Punkt
über entsprechende Plugins. Allerdings fehlt in diesem Kontext die Flexibilität
bzw. die Versionierung über Systemgrenzen hinweg völlig. Ein Austausch von
Inhalten erfolgt über Kopieroperationen einzelner Textfragmente. Sobald
aufwändigere interaktive Elemente einbezogen werden ist dies nicht möglich.

********************************************************************************

## LiaScript Konzepte

*LiaScript* zielt entsprechend darauf eine Brücke Lehr-Lern-Umgebungen,
Wikipedia und den Methoden der verteilten Softwareentwicklung zu schlagen und
kombiniert dafür deren Ansätze neu:

| Element                                                        | Bedeutung                                                                                                                                                                                                                                  |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Gestaltung der Inhalte mittels abstrakter Beschreibungssprache | garantiert die unmittelbare Bearbeitbarkeit ohne spezifische Software. Die Strukturelemente unterstützen den logischen Aufbau des Kurses                                                                                                   |
| Versionierung der Kurse                                        | die Speicherung  aller Änderungen erlaubt es in der Historie des Dokumentes nachzuvollziehen und beliebig zu kombinieren. Einfache Textdokumente sind hierbei wesentlich einfacher zu handhaben als binäreformate wie docx, pptx oder pdf. |
| Verteilte Entwicklung der Inhalte                              | anders als in Wikipedia sollten die Lehrenden in der Lage sein, Kurse zu kombinieren und auf eigene Anforderungen hin anzupassen. Entsprechend exisitieren verschiedene Versionen ein und des selben Kurses nebeneinander.                 |

> Damit zielt *LiaScript* auf die Realisierung einer browserbasierten Lehr-Lern-Umgebung, deren Inhalte mit einer Beschreibungssprache spezifiziert werden können.  Damit sind interaktive Inhalte ohne explizite Programmierkenntnisse möglich, wobei die konkreten Elemente oder aber ganze Kurse als offene Materialien weiterverarbeitet und modifiziert werden können.

     {{1}}
********************************************************************************

Die Beiträge von *LiaScript* auf diesem Weg lassen sich wie folgt
zusammenfassen:

1. erweiterte Markdownsyntax, die ein breites Spektrum an interaktiven Elementen
   umfasst,
2. Interpreter für die Darstellung der Inhalte im Browser,
3. Bereitstellung unterschiedlicher Präsentationsformate, die den Kurs
   Nutzergetrieben aufbereiten,
4. verteiltes Versionmanagment auf der Basis der Tools, die für Open-Source
   Projekte zum Einsatz kommen und
5. ein Editor-Tool, das als Open-Source Werkzeug frei zur Verfügung steht.

Der gesamte Umfang eines LiaScript-Dokumentes wird vom Browser geladen. Danach
erfolgt die Darstellung durch den Interpreter. Die dafür bereitstehenden
Präsentationsformate Vorlesung, Mitschriften und Buch kennen Sie ja bereits.

********************************************************************************

## Markdown Erweiterung

    --{{0}}--
LiaScript erweitert den Sprachumfang von Markdown in vielerlei Hinsicht. Dies
sind insbesondere die interaktiven Elemente wie ausführbarer Code oder Quizze.
Dazu kommen statische Elemente wie Diagramme. Auf den folgenden Seiten finden
Sie dazu eine Auswahl von Beispielen. Werfen wir aber zunächst einen Blick auf
die generelle Idee von Markdown. Im oberen Teil der aktuellen Seite sehen Sie
die Inhaltsbeschreibung, im unteren das Ergebnis nach dem Rendering.

Einen guten Überblick zum "traditionellen" Sprachumfang von Markdown bietet die
Zusammenstellung auf der Webseite
[Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
Beispielhaft soll hier ein Ausschnitt aus einem Markdown Dokument gezeigt
werden, dass die Einbindung von Listen, Tabellen und Bildern zeigt.

```markdown                 MeinMarkdownDokument.md
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

Die Sprachausgabe, die *LiaScript* der Ausdrucksmächtigkeit von Markdown
hinzufügt, haben Sie ja bereits genutzt. Diese kann mit 32 Sprachen umgesetzt
werden. Klicken Sie nach rechts ...

     {{1}}
********************************************************************************

... um eine englische Textausgabe zu hören. Deren Ausgaben basieren wiederum nur
auf dem im Dokument festgehaltenen Text. Für den gerade gehörten englischen Text
steht im Kursdokument einfach nur der Eintrag:

```
    --{{1 US English Female}}--
But you can also include other languages in spoken text.
English, French, Russian, etc. are no problem.
```

    --{{1 US English Female}}--
But you can also include other languages in spoken text. English, French,
Russian, etc. are no problem.

Die perspektivische Multilingualität von *LiaScript* betrifft verschiedene
Elemente. Ganze Kurse, einzelne Erläuterungen können übersetzt und international
verwendet werden. Die Sprache der Ausführungsumgebung lässt sich übrigens im
Header eines Dokumentes konfigurieren. Dann erscheinen auch die Elemente in der
Hilfe und den Verweisen in der jeweiligen Sprache.

********************************************************************************

     {{2}}
********************************************************************************

Darüber hinaus können mit

``` markdown
 ?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)
!?[video](https://www.youtube.com/watch?v=bICfKRyKTwE)
```

Videos und Tonsample integriert werden. Für diese existieren eigene
Konfigurationsschnittstellen, die den Startzeitpunkt und die Darstellungsgröße
festlegen. Starten Sie die Einträge über die Bedieninterfaces.

?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)

!?[video](https://www.youtube.com/watch?v=bICfKRyKTwE)

********************************************************************************


### Diagramme

Das in der Kursbeschreibung enthalten Diagramm wird durch den Interpreter in
eine anschauliche Form überführt. Damit sind für einfache Darstellungen keine
weiteren Werkzeuge notwendig, deren Inhalt mit jeder Iteration angepasst werden
müsste.

``` markdown
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

*LiaScript* integriert 12 verschiedene Formen von Quizzen, die in die
Lehrinhalte integriert werden können.

    --{{0}}--
Die Beispiele für Quizze zeigen jeweils im oberen Bereich den LiaScript Code, im
unteren die Darstellung im Browser. Die übergreifende Syntax erlaubt sowohl die
Spezifikation des Formates, der Lösungen, aber auch Hilfen für den Lernenden.

     {{0-1}}
********************************************************************************

**a) Text Quiz**

``` markdown
What did the **fish** say when he hit a **concrete wall**?

    [[dam]]
```

What did the **fish** say when he hit a **concrete wall**?

    [[dam]]

********************************************************************************


     {{1-2}}
********************************************************************************

**b) Multiple Choice**

``` markdown
Just add as many points as you wish:

    [[X]] Only the **X** marks the correct point.
    [[ ]] Empty ones are wrong.
    [[X]] ...
```

Just add as many points as you wish:

    [[X]] Only the **X** marks the correct point.
    [[ ]] Empty ones are wrong.
    [[X]] ...

********************************************************************************

    {{2-3}}
********************************************************************************

**c) Single Choice**

``` markdown
Just add as many points as you wish:

    [( )] ...
    [(X)] <-- Only the **X** is allowed.
    [( )] ...
```

Just add as many points as you wish:

    [( )] ...
    [(X)] <-- Only the **X** is allowed.
    [( )] ...

Weitere Beispiele für Quizze finden Sie unter dem [Link](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md)

********************************************************************************

### Ausführbarer Code

Ein Beispiel für ausführbaren Code ist dieses JavaScript Fragment. Dieser Code
wird nativ im Browser ausgeführt und generiert eine entsprechende AUsgabe

```javascript
// Initialize a Line chart in the container with the ID chart1
new Chartist.Line('#chart1', {
  labels: [1, 2, 3, 4],
  series: [[100, 120, 180, 200]]
});
```
<script>@input</script>

<div class="ct-chart ct-golden-section" id="chart1"></div>

Alternativ können Sie aber eine von 32 Programmiersprachen integrieren, die über
einen Webservice eingebunden werden. Der Vorteil liegt hier darin, dass Sie ohne
aufwändige Installationen von Compilern und Editoren praktisch am Code arbeiten
können. Das nachfolgende Fragment zeigt ein Beispiel aus einer
[Informatik-Vorlesung](https://liascript.github.io/course/?https://raw.githubusercontent.com/SebastianZug/SoftwareprojektRobotik/master/00_Einfuehrung.md#1),
die in LiaScript erstellt wurde.

```cpp                     structExample.cpp
#include <iostream>

struct Student{
  std::string name;
  int matrikel;
  void printCertificate(std::string topic);
};

void Student::printCertificate(std::string topic){
  std::cout << name << " passed " << topic;
}

int main()
{
  Student Humboldt {"Alexander Humboldt", 1798};
  Humboldt.printCertificate("Softwareentwicklung");
  return 0;
}
```
@Rextester.CPP

## Verteiltes Versionmanagment

    --{{0}}--
Wie ist nun aber die verteilte Entwicklung dieses Kurses realisiert? Der Kurs
selbst wird auf einer Plattform für Open-Source Projekte gehostet. Github
umfasst Millionen von Implementierungen und stellt unter anderem die Werkzeuge
für die Versionierung bereit.


![Logo](./images/logo.png)<!-- width="20%" -->


## Editor

There are currently 2 Plugins for the [Atom Editor](https://atom.io/) available,
which are intended to ease and simplify the development of online course with
LiaScript.

[liascript-preview](https://atom.io/packages/liascript-preview): Is a tiny
previewer that, if it was toggled, updates the view on your course each time you
save your document.


![previewer](https://raw.githubusercontent.com/andre-dietrich/liascript-preview/master/preview.gif)<!-- style="width: 100%" -->

[liascript-snippets](https://atom.io/packages/liascript-snippets): If you start
typing "lia" in your document you switch on a fuzzy search, that contains a lot
of LiaScript help, examples, and snippets.

![snippets](https://raw.githubusercontent.com/andre-dietrich/liascript-snippets/master/preview.gif)<!-- style="width: 100%" -->




## Ausblick

Die Integration

![Logo](./images/Screenshot.png)<!-- width="80%" -->

Haben wir Sie neugierig gemacht? Weitere Informationen finden Sie unter der Projektwebseite

https://liascript.github.io/

![Logo](./images/logo.png)<!-- width="20%" -->
