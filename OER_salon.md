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

# HDS.Salon

<p style="font-size:60px">OER im Kleinen wie im Großen</p>

5.11.2020

Sebastian Zug, TU Bergakademie Freiberg


_Auch dieser Vortrag ist ein Open Source Dokument und unter  zu finden._


## Motivation

           {{0-2}}
********************************************************************************
> Open Courseware / Open Educational Resources _ ... teaching, learning and research materials in any medium, digital or otherwise,that reside in the **public domain** or have been released under an open license that permits no-cost access, use, **adaptation** and **redistribution** by others with no or limited restrictions. Open licensing is built within the existing framework of intellectual property rights as defined by relevant international conventions and respects the authorship of the work_
[UNESCO 2002 Forum on the Impact of Open Courseware for Higher Education in Developing Countries]
********************************************************************************

           {{1-2}}
********************************************************************************

**Wie stellen wir uns das Ganze praktisch vor?**

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

********************************************************************************


   {{2-3}}
********************************************************************************

**Was sind die Herausforderungen auf diesem Weg?**

| Aspekt       | Bedeutung                                                     |
| ------------ | ------------------------------------------------------------- |
| Suche        | Wie finde ich die für mich passenden Materialien?             |
| Tools        | Wie kann ich diese auf meine spezifischen Lernziele anpassen? |
| Qualität     | Wer stellt sich, dass die Inhalte korrekt aufbereitet sind?   |
| Sichtbarkeit | Wie lässt sich meine Autorenschaft darstellen?                |

********************************************************************************


## Alternative Ansätze mit ähnlichen Problemen

**1. Wikipedia**

Der Eintrag "Bundesrepublik Deutschland" blickte im Mai 2019 auf 15850
Änderungen zurück. Dazu haben 3928 Nutzer beigetragen. Wikipedia sichert so die
Aktualität und Qualität des Bestandes an Daten. Wo aber liegt der Schlüssel zum
Erfolg?

| Aspekt       | Wikipedia - Lösung                                          | Nachteil                                                     |
| ------------ | ----------------------------------------------------------- | ------------------------------------------------------------ |
| Suche        | eine Instanz eines Artikels unmittelbar abrufbar      | keine unterschiedlichen Ausprägungen zu einem Thema möglich. |
| Tools        | integrierter Editor auf der Basis eines Markdown-Dialekts   | starke Beschränkung der Möglichkeiten auf strukturierte Texte, Formeln, Bilder                                                             |
| Qualität     | ausgefeilte Reviewsystem mit Experten, Versionsdatenerfassung und -vergleich |                                                              |
| Sichtbarkeit | Autorenschaft in der Versionshistorie sichtbar              |                                                              |

                  {{1-2}}
********************************************************************************

**2. (Open-Source-) Softwareprojekte**

Die Softwareentwicklung wird heute über webbasierte Projekttools (GitLab, GitHub) koordiniert.

| Aspekt       | Wikipedia - Lösung                                          | Nachteil                                                     |
| ------------ | ----------------------------------------------------------- | ------------------------------------------------------------ |
| Suche        | Volltextsuche und Dokumentationen      | Suche zumeist aufwändig und nicht selten frustrierend |
| Tools        |    |  Keine Vorgaben                                                            |
| Qualität     | technische Unterstützung von Reviews, aufwändige Versionsdatenerfassung und -vergleich, automatisierte Tests |                                                                |
| Sichtbarkeit | Aufwändige Analysen zu den Beiträgen der Einzelnen             |                                                              |

********************************************************************************

## Lösungsansatz

*LiaScript* möchte eine Brücke zwischen den Lehr-Lern-Umgebungen,
dem Wikipedia Ansatz und den Methoden der verteilten Softwareentwicklung schlagen.
Dafür definiert das Projekt deren Ansätze in folgenden Punkten neu und kombiniert
sie:

<!--
style="width: 100%; max-width: 860px; display: block; margin-left: auto; margin-right: auto;"
-->
```ascii
Wikipedia --> [Bescheibungssprache     ]
          --> [Versionsmanagement      ] <-- Softwareentwicklung
              [Verteilte Entwicklung   ] <--
              [Serverlose Infrastruktur]
              [Dynamische Inhalte      ]
                                                                               .
```

       {{1}}
********************************************************************************

**Tabellen**

```markdown
| Animal          | weight in kg | Lifespan years |
| --------------- | ------------:| --------------:|
| Mouse           |        0.028 |              2 |
| Flying squirrel |        0.085 |             15 |
| Brown bat       |        0.020 |             30 |
| Sheep           |           90 |             12 |
| Human           |           68 |             70 |
```

| Animal          | weight in kg | Lifespan years |
| --------------- | ------------:| --------------:|
| Mouse           |        0.028 |              2 |
| Flying squirrel |        0.085 |             15 |
| Brown bat       |        0.020 |             30 |
| Sheep           |           90 |             12 |
| Human           |           68 |             70 |

********************************************************************************

      {{2}}
********************************************************************************

**Ausführbarer Code**

```
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

********************************************************************************

      {{3}}
********************************************************************************

**Quizze**

```markdown
Markieren Sie die ungeraden Zahlen!

    [[X]] 1
    [[ ]] 2
    [[X]] 3
    [[?]] Nur zur Erinnerung, wie definiert sich eine ungerade Zahl?
```

Markieren Sie die ungeraden Zahlen!

    [[X]] 1
    [[ ]] 2
    [[X]] 3
    [[?]] Nur zur Erinnerung, wie definiert sich eine ungerade Zahl?

Weitere Informationen finden Sie unter der Projektwebseite

https://liascript.github.io/

in der [Dokumentation](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md#1) oder dem [Youtube-Channel](https://www.youtube.com/channel/UCyiTe2GkW_u05HSdvUblGYg)

********************************************************************************

## Erfahrungen beim Einsatz von OER

-> Kursüberblick anhand von [GitHub](https://github.com/SebastianZug/VL_Softwareentwicklung)

Ergebnisse:

1. Aus der Zusammenarbeit an den Materialien entsteht zu mindest im Kontext eines Kernteams ein "wir" Gedanke.
2. Fehler werden deutlich schneller ausgemerzt als in vergangenen Jahren. Die "kurzfristige" Qualität steigt an.
3. Die Interaktion zwischen Lehrenden und Studierenden steigert sich - *"Sollte man das nicht besser so erklären ..."*
4. Das Verständis über verteilte Entwicklung von Inhalten entwickelt sich sehr positiv, selbst die Nicht-Informatiker beschäftigen sich mit den Methoden.

## Kontakt

Neugierig geworden auf OER?

| Prof. Dr. Sebastian Zug | sebastian.zug@informatik.tu-freiberg.de |
