<!--
author:   Sebastian Zug

email:    Sebastian.Zug@informatik.tu-freiberg.de

version:  1.0.2

language: de

narrator: Deutsch Male

mode:     Presentation

comment:  Dieser Kurs für in das Projekt LiaScript ein und diskutiert die
          Vorteile im Kontext der OER Idee.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

logo:     ./images/logo.png

import: https://raw.githubusercontent.com/LiaTemplates/Rextester/master/README.md
        https://raw.githubusercontent.com/liaTemplates/processingjs/master/README.md

translation: Deutsch  translations/German.md

-->

# Willkommen bei LiaScript

    --{{0}}--
Hallo, wenn Sie sich für *Open Educational Ressources* interessieren, sind Sie
hier genau richtig. Wir wollen Ihnen ein neues Konzept für das "O" in O E R
vorstellen, dass deutlich weitergeht als Dokumente, die auf einem Server online
gestellt werden. Unser Projekt heißt "LiaScript" und erlaubt es Lehrinhalte wie
ein Open Source Projekt umzusetzen. Interessiert? Dann klicken Sie auf den
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

--------------------------------------------------------------------------------

Die interaktive Version zu diesem Kurs können Sie unter
[LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/SebastianZug/WillkommenAufLiaScript/master/Willkommen.md#1)
starten.

Der vollständige "Code" ist unter
[GitHub](https://github.com/SebastianZug/WillkommenAufLiaScript/blob/master/Willkommen.md)
zu finden.

![Logo](./images/logo.png)<!-- width="20%" -->

--------------------------------------------------------------------------------

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
   Softwareprojekten verwendet wird. Die Markdown-Dokumente werden dabei durch
   Interpreter in html Darstellungen überführt, ohne das der Anwender deren
   deutlich abstraktere Semantik kennen muss. Die nachfolgende Tabelle zeigt
   das nebeneinander der Darstellung

   Die einfache Semantik ist für statische Dokumente von Vorteil aber in Bezug auf
   Lerninhalte gleichzeitig die größte Einschränkung. Interaktiven Elementen wie
   Quizze, Simulationen oder ausführbare Codefragmente sind damit nicht umsetzbar.

<table class="lia-inline lia-table">
    <thead class="lia-inline lia-table-head">
        <tr>
          <th>Markdown Inhalt</th>
          <th>Ausgabe</th>
        </tr>
    </thead>
        <tr class="lia-inline lia-table-row">
          <td>
          <code><pre 	style = "Lucida Console; font-size: 14px;font-style: normal; ">
 # Überschrift 1
 Das ist der Text

 ## Unterüberschrift 1.A
 Das auch, nur wird dieses Wort __fett__ geschrieben
          </pre></code></td>
          <td>
          <h2> Überschrift 1 </h2>
          Das ist der Text

          <h1> Unterüberschrift 1.A </h1>
          Das auch nur, wird dieses Wort <b>fett</b>  geschrieben
          </td>
        </tr>
</table>

Im Unterschied dazu definieren etablierte Lernumgebungen Moodle oder Ilias
die notwendige Infrastruktur, um den notwendigen Lernfortschritt individuell
zu begleiteten. Allerdings fehlt diesen Lehr-Lern-Umgebungen die Flexibilität
bzw. die Versionierung über Systemgrenzen hinweg völlig. Ein Austausch von
Inhalten erfolgt über Kopieroperationen einzelner Textfragmente. Sobald
aufwändigere interaktive Elemente einbezogen werden, die system-spezifisch
implementiert sind, ist dies nicht möglich.

********************************************************************************

## LiaScript Konzepte

--{{0}}--
Folglich möchte *LiaScript* eine Brücke zwischen den Lehr-Lern-Umgebungen,
dem Wikipedia Ansatz und den Methoden der verteilten Softwareentwicklung schlagen.
Dafür definiert das Projekt deren Ansätze in folgenden Punkten neu und kombiniert
sie:

| Element                                                        | Bedeutung                                                                                                                                                                                                                                  |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Gestaltung der Inhalte mittels abstrakter Beschreibungssprache | garantiert die unmittelbare Bearbeitbarkeit ohne spezifische Software. Die Strukturelemente unterstützen den logischen Aufbau des Kurses                                                                                                   |
| Versionierung der Kurse                                        | die Speicherung  aller Änderungen erlaubt es in der Historie des Dokumentes nachzuvollziehen und beliebig zu kombinieren. Einfache Textdokumente sind hierbei wesentlich einfacher zu handhaben als binäreformate wie docx, pptx oder pdf. |
| Verteilte Entwicklung der Inhalte                              | anders als in Wikipedia sollten die Lehrenden in der Lage sein, Kurse zu kombinieren und auf eigene Anforderungen hin anzupassen. Entsprechend existieren verschiedene Versionen ein und des selben Kurses nebeneinander.                 |

> Damit zielt *LiaScript* auf die Realisierung einer browserbasierten Kursdarstellung, deren Inhalte mit einer Beschreibungssprache spezifiziert werden können. Damit sind interaktive Inhalte ohne explizite Programmierkenntnisse möglich, wobei die konkreten Elemente oder aber ganze Kurse als offene Materialien weiterverarbeitet und modifiziert werden können.

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
Markdown ist die Basis von *Liascript*. Allerdings genügen die in dieser
Beschreibungssprache integrierten Features den Anforderungen eines interaktiven
Lerninhaltes nicht. Von Haus aus unterstützt Markdown zum Beispiel:

**Listen**

1. in
2. geordnet oder

   * ungeordnet
   * auch in geschachtelter Struktur

**Tabellen**

| Header 1   | Header 2   |
| :--------- | :--------- |
| Item 1     | Item 2     |


**Images**

![images](https://farm2.static.flickr.com/1618/26701766821_7bea494826.jpg)<!-- width="30%" -->
```

Daraus entsteht folgende Darstellung:

-------------------------------------------------------------------------------
Markdown ist die Basis von *Liascript*. Allerdings genügen die in dieser
Beschreibungssprache integrierten Features den Anforderungen eines interaktiven
Lerninhaltes nicht. Von Haus aus unterstützt Markdown zum Beispiel:

**Listen**

1. in
2. geordnet oder

   * ungeordnet
   * auch in geschachtelter Struktur

**Tabellen**

| Header 1   | Header 2   |
| :--------- | :--------- |
| Item 1     | Item 2     |


**Images**

![images](https://farm2.static.flickr.com/1618/26701766821_7bea494826.jpg)<!-- width="30%" -->

-------------------------------------------------------------------------------

### Medieneinbindung/ Sprachausgabe

     {{0-3}}
********************************************************************************

**Text-to-Speech Ausgabe**

Die Sprachausgabe, die *LiaScript* der Ausdrucksmächtigkeit von Markdown
hinzufügt, haben Sie ja bereits genutzt. Diese kann mit 32 Sprachen umgesetzt
werden. Klicken Sie nach rechts ...

********************************************************************************

     {{1-3}}
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

     {{2-3}}
********************************************************************************

**Einbettung von Medien**

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


                                       {{3-6}}
********************************************************************************

**Und nun alles zusammen**

In LiaScript können Sie die Videos nachvertonen, in dem Sie Texte zu den Videos abspielen. Schauen wir zunächst auf das Originalvideo des Youtube-Nutzers Björn Seidler, das unter folgendem [Link](https://www.youtube.com/watch?v=qAh6P1MaYtU) zu finden ist. Beim Start des Videos hören Sie den gesprochenen Originalton.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qAh6P1MaYtU?start=15&controls=0&showinfo=0&rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

********************************************************************************

--{{4}}--
In diesem Video werden wir uns mit den Konzepten des Analog-Digital-Wandlers beschäftigen. Dazu beginnen wir zunächst mit einem Blick ins Handbuch der Atmel 8 Bit-Controller. Sie sehen die Basis Features die ich mit der Maus markiere.

                                       {{4-6}}
********************************************************************************

Dies ist nun die nachvertonte Version mit Hilfe der LiaScript Sprachausgabe. Der Text liegt als geschriebener Inhalt vor und kann beliebig angepasst werden.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qAh6P1MaYtU?start=15&controls=0&mute=1&showinfo=0&rel=0&autoplay=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

********************************************************************************

--{{5 US English Female}}--
In this video we focus on the concepts of the analog-to-digital converters. We will start with a look at the Atmel 8 bit controller manual. You see the basic features that I mark with the mouse.

                                       {{5-6}}
********************************************************************************

So sind auch (maschinelle) Übersetzungen möglich, während das Ursprungsvideomaterial erhalten bleibt.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qAh6P1MaYtU?start=15&controls=0&mute=1&showinfo=0&rel=0&autoplay=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

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


{{1}}
********************************************************************************

Daneben können aber auch JavaScript basierte Diagramme unmittelbar im LiaScript-Dokument eingebettet werden. Dieses Codefragment generiert ein xy Diagramm. Die Parameter können zur Präsentationszeit angepasst werden.

```javascript
// Initialize a Line chart in the container with the ID chart1
new Chartist.Line('#chart1', {
  labels: [1, 2, 3, 4],
  series: [[100, 120, 180, 200]]
});
```
<script>@input</script>

<div class="ct-chart ct-golden-section" id="chart1"></div>

********************************************************************************

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

Die Kreuze markieren sehr intuitiv die korrekten Lösungen beim Mulitple Choice Test.
In diesem Beispiel wird illustriert, wie zusätzliche Hilfen für den Lernenden
Integriert werden können. Neben dem "i" für die Lösung taucht nun auch ein Fragezeichen auf.

``` markdown
Please mark even numbers!

    [[X]] 1
    [[ ]] 2
    [[X]] 3
```

Just add as many points as you wish:

    [[X]] 1
    [[ ]] 2
    [[X]] 3
    [[?]] What is the characteristic of an even number?

Weitere Beispiele für Quizze finden Sie unter dem [Link](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md)

********************************************************************************

### Ausführbarer Code

--{{0}}--
Ausführbarer Code ist insbesondere für die Ausbildung in der Informatik von
zentraler Bedeutung. Dies können Programme sein, die eine grafische Ausgabe generieren
oder aber einen Output auf der Konsole liefern. Mit dem browserinternen
Interpreter können alle Arten von Tools, die ein JavaScript Interface bieten, integriert werden. Klicken Sie auf den Button unter den Codefragmenten, um diese auszuführen. Ändern Sie den Code, um zum Beispiel die Farbwahl neu zu definieren oder Ausgaben anzupassen.

In diesem Beispiel wurde eine die Processing Toolchain, die als JavaScript-Implementierung vorliegt, in LiaScript integriert. Über ein `include` über dem zugehörigen Makro kann dies eingebettet werden.

```cpp                         Processing.js
void setup() {
  size(480, 220);
}

void draw() {
  if (mousePressed) {
    fill(0);
  } else {
    fill(255);
  }
  ellipse(mouseX, mouseY, 80, 80);
}
```
@Processing.eval


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
Wie ist nun aber die verteilte Entwicklung eines LiaScript-Kurses realisiert?
Die vorliegende "Vorlesung" selbst wird auf Github, einer Plattform für
die Softwareentwicklung gehostet. Dort finden sich Millionen von Open-Source Projekten, nun auch der Code für dieses Dokument.

Sie können das *LiaScript* Dokument, dass hinter diesem Kurs steht unter folgendem
[Link](https://github.com/SebastianZug/WillkommenAufLiaScript) finden. GitHub unterstützt
aber nur das konventionelle Markdown, so dass einige Elemente in der Vorschau nicht korrekt angezeigt werden.

Der folgende Screenshot zeigt die Übersicht über die Versionen seit dem 1. Dezember. Anhand dieser Übersicht können die Beitragenden und deren Änderungen individuell nachvollzogen werden.

![GitHub](./images/ScreenshotGitHub.png)<!-- width="80%" -->
*Übersicht über den Stand der Versionen am 3.12.2019*

Ein öffentliches Git-Projekt kann sehr einfach kopiert und weiterentwickelt werden. Dabei unterstützen entsprechende Tools das Verschmelzen von unterschiedlichen Versionen und Entwicklungssträngen.

## Editor

    --{{0}}--
LiaScript Dokumente könnnen mit jedem Texteditor bearbeitet werden. Um den
LiaScript-Nutzer aber bei der effektiven Arbeit zu unterstützen, wurde ein
Open-Source Editor angepasst. Atom ist ein freies Editierwerkzeug für Texte und Code,
dass für Windows, Linux und Mac OS bereitsteht.

Gegenwärtig bestehen zwei Plugins für den [Atom Editor](https://atom.io/), die
die Entwicklung von Lerninhalten mit einer Vorschau und Codesnippets unterstützen.

[liascript-preview](https://atom.io/packages/liascript-preview): Der Previewer
gibt dem Nutzer ein sofortiges Feedback für seine Arbeit. Während im linken
Fenster LiaScript Code eingegeben wird erscheint die Ausgabe sofort auf der
rechten Seite.

![previewer](https://raw.githubusercontent.com/andre-dietrich/liascript-preview/master/preview.gif)<!-- style="width: 100%" -->

[liascript-snippets](https://atom.io/packages/liascript-snippets): Um bestimmte
LiaScript-Konstrukte rasch bei der Hand zu haben, integriert dieses Plugin
kleine Fragmente und Beispiele. Der Nutzer gibt lediglich ein Kürzel des
intendierten Inhaltes ein, also zum Beispiel `liaQuiz` und bekommt ein
Auswahlmenü aller möglichen Formate angezeigt.

![snippets](https://raw.githubusercontent.com/andre-dietrich/liascript-snippets/master/preview.gif)<!-- style="width: 100%" -->

## Integration

Seit dem Wintersemester 2017/18 wird LiaScript Vorlesungen der Informatik an der Otto-von-Guericke Universität und der TU Bergakademie Freiberg eingesetzt. Für die nahtlose Integration in den Lehrbetrieb sorgt dabei die Einbettung der jeweiligen Materialien in die Lehr-Lern-Umgebungen, die an den Hochschulen eingesetzt werden.

![Logo](./images/Screenshot.png)<!-- width="80%" -->
*Integration der LiaScript-basierten Vorlesung "Softwareprojekt" in das OPAL System*

## Kontakt

Haben wir Sie neugierig gemacht? Weitere Informationen finden Sie unter der Projektwebseite

https://liascript.github.io/

![Logo](./images/logo.png)<!-- width="20%" -->


| Dr. Andrè Dietrich | andre.dietrich@ovgu.de |
| Prof. Dr. Sebastian Zug | sebastian.zug@informatik.tu-freiberg.de |
