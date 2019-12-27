<!--
author:   Sebastian Zug

email:    Sebastian.Zug@informatik.tu-freiberg.de

version:  1.0.2

language: de

narrator: UK English Female

mode:     Presentation

comment:  This course introduces LiaScript and explains the benefits of the new, open-source concept.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

logo:     ./images/logo.png

import: https://raw.githubusercontent.com/LiaTemplates/Rextester/master/README.md
        https://raw.githubusercontent.com/liaTemplates/processingjs/master/README.md

translation: Deutsch  translations/German.md
-->

# Welcom to LiaScript

    --{{0}}--
Hello, if you are interested in *Open Educational Resources*, you are you have come to the right place. We want to present you a new concept for the "O" in O E R
that goes much further than providing documents on a server. Our project is called "LiaScript" and supports the design of teaching material similar to Open Source project development. Interested? Then click on the arrow to the right.

As you can probably already imagine, this course was also developed on the basis
of *LiaScript*.  For introducing the concept we use the features,
provided by browser-based execution environment.

You can run the course either in book form, as a lecture or
similar to a lecture script. To switch the presentation style, click on the symbol
top right. The

+ **eye** means the presentation of the material with addtional lecture notes. The actual teaching content is enriched by additional information. The text you have just heard is now displayed in the lower part of the screen.

+ **book** integrates all contents in a common text document. All animations and transitions are disabled in this case.

+ **ear** the additional information is presented as text-to-speech.  This gives the feeling of an actual course.

To progress through the course, please use the arrow keys on top. The
Display on the left provides an overview of the structure of the course.

--------------------------------------------------------------------------------

If you currently view the text on the code base, you can switch to the interactive version by clicking here:
[LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/SebastianZug/WillkommenAufLiaScript/master/Welcome.md#1).

In the other direction you can take a view on the "Code" by following this link
[GitHub](https://github.com/SebastianZug/WillkommenAufLiaScript/blob/master/Welcome.md).

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
+---------------------------+          +---------------------------+
| Course German Literatur   |          | Course German Literature  |
| Autors John Muster        | "Error"  | Autors John Muster        |
|                           |------->  |        Angelika Maier     |----->
|~~~~~~~~~~~~~~~~~~~~~~~~~~~|          |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
| In 1756 Goethe visited    |---.      | In 1786 Goethe visited    |--.
| Italy ...                 |   |      | Italy ...                 |  |
                                |                                     |
                                |                                     |    +----------------------------+
                                |                                     |    | Course  Deutsche Literatur |
                                |                                     |    | Autoren John Muster        |
                                |                                     .--> |         Angelika Maier     |
                                |                                          |         Steve Gray         |
                                |                                          |~~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                                |                                          | 1786 reiste Goethe nach    |
                                |                                          | Italien ...                |
                                |       Version 1.0
                                |      +---------------------------+
                                |      | Course  Goethe & Schiller |
                                |      | Autoren John Muster       |
                                .-->   |         Angelika Maier    |----->
                                       |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                                       | The correspondence during |
                                       | the Italian journey ...   |
```
*Versions of the contents of a course and their reuse in other contexts*

    --{{0}}--
How should teaching materials be created that really deserve the O E R idea? They should be freely available AND manipulable. Some protagonists
of the community emphazise the first aspect and annotate a pdf document as
open. But courses on a topic are very different, the teachers set varying priorities
or chose another contexts. Hence, a complete adoption is not enough. Furthermore
it is necessary to provide materials that can be revised and newly compiled. The
Figure illustrates this. A number of authors corrected errors and
develops the contents further. This also results in completely new
course configurations or translations of content. Which other platform for a successful multi-editor knowledge collections could be used as inspiring example?

********************************************************************************


     {{1-2}}
********************************************************************************

Wikipedia as a web-based system has brought together millions of authors and users. Why does this project succeeds?

    --{{1}}--
The German entry for "Federal Republic of Germany" looked back on 15850 changes in May 2019. 3928 users have contributed to this. Wikipedia thus ensures the timeliness and quality of the data stock. But where is the key to success?

| Reasons for success                 | Comments                                                                                                                                                                                                                              |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Versioning method                   | Wikipdia stores the entire history of a  document. This makes it possible to reconstruct changes, to merge versions and eliminate errors very easy.                                                                                   |
| Simple context description language | The contents in Wikipedia are edited in a simple description language [wikitext](https://de.wikipedia.org/wiki/Wikitext). Unlike Word or pdf documents, these are simple text files that can be manipulated in the browser by anyone. |
| Integrated editor                   | Users can make the changes in the description language directly in the browser. No separate tool and installation is necessary.                                                                                                       |

********************************************************************************

     {{2-3}}
********************************************************************************

So can one simply transfer the concepts of Wikipedia to course content management?

    --{{2}}--
So can you simply derive a Wikipedia for course content? The answer to this question is clearly no. This statement is supported by the three main reasons: firstly, the central architecture of Wikipedia, secondly the missing possibility to integrate interactive content.
And thirdly, the limited possibilities to create individual states save.

From the perspective of the requirements for a platform for knowledge transfer
the Wikipedia concept includes two central limitations:

1. The centrally oriented concept concentrates all content in one place.
   So there is only one entry for a specific topic. Splitting, reuseage or a new
   combination for individual purposes is not in accordance with the basic idea.
   At the same time the centralistic concept gives rise to the
   need for an efficient IT infrastructure.

2. Wikitext defines a description language
   [Markdown](https://de.wikipedia.org/wiki/Markdown), which was developed for enhancing
   text documents by structural infomration (headline, normal text, code, etc.)
   Differnt dialects are especially used for the documentation of
   software projects. Markdown documents can be transformend into html representations automatically. Hence, the author do not need explicit knowledge in html or website description. The following table shows
   the side by side display of the

   The simple semantics is advantageous for static documents but in terms of
   learning content is also the biggest limitation. Interactive elements like
   Quizzes, simulations or executable code fragments cannot be implemented with it.

<table class="lia-inline lia-table">
    <thead class="lia-inline lia-table-head">
        <tr>
          <th>Markdown Content</th>
          <th>HTML Output</th>
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

Additionally, Wikipedia is not a learning environment. Many aspects of established
platforms, like Moodle or Ilias, are missed here.
However, these teaching-learning environments lack the flexibility
or versioning across system boundaries completely. An exchange of
content is done by copying operations of single text fragments. As soon as
more complex interactive elements are included, which are specific to the system, this is not possible.

********************************************************************************

## LiaScript Concepts

--{{0}}--
Consequently, *LiaScript* wants a bridge between the teaching-learning environments, the Wikipedia approach and methods of distributed software development. To achieve this, the project redefines and combines the approaches in the following points:

| Element                            | Significance                                                                                                                                                                                                                                                                                |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Abstract description language      | ... guarantees immediate workability without specific software. The combination of content and explicite structure commands provides easy to understand but well organized materials.                                                                                                       |
| Versioning of the courses          | ... saving all changes of a course document allows to trace its history and to combine it contents in various ways. Simple text documents are much easier to handle in this context than binary formats like docx, pptx or pdf.                                                             |
| Distributed development of content | ... unlike in Wikipedia, teachers should host and organize their course material independtently. The infrastructure free approach guarantees a free access and publications on the materials without mastering individual server applications before.                                                                                                                                                                                                              |

> Thus, *LiaScript* aims at the realization of a browser-based  courses, whose contents can be specified with a abstract description language. Thus, interactive course elements are possible without explicit programming knowledge, whereby the concrete elements or entire courses can be further processed and modified as open materials.

     {{1}}
********************************************************************************

The conceptional contributions of *LiaScript* can be summarize as follows:

1. advanced markdown syntax, which includes a wide range of interactive elements,
2. infra-strucuture indepenendend interpretation of the content directly in the browser,
3. provision of different presentation formats, which provide the course contents driven by user demands,
4. distributed version management based on the tools that are commonly used in open source
   projects and
5. an editor tool, which is freely available.

The entire content of a LiaScript document is loaded by the browser. Afterwards the interpreter displays the document. You already know the presentation formats lecture, notes and book.

********************************************************************************

## Markdown extentions

    --{{0}}--
LiaScript extends the language scope of Markdown in many ways. These are especially the interactive elements like executable code or quizzes. In addition, there are static elements such as diagrams or movies. On the following pages you will find a selection of examples. But first let's take a look at the general idea of Markdown. In the upper part of the current page you see the content description within the box, in the lower part the result after rendering.

The website [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) provides an overview of the "traditional" Markdown feature set.  
As an example for the transformation process we included a code block in the following box.

```markdown                 MeinMarkdownDokument.md
Markdown is the basis of *Liascript*. However, the features integrated in this description language do not meet the requirements of interactive learning content. For example, Markdown supports by default:

**Lists**

1. in
2. orded,

   * unordered or
   * embedded structure

**Tables**

| Header 1   | Header 2   |
| :--------- | :--------- |
| Item 1     | Item 2     |


**Images**

![images](https://farm2.static.flickr.com/1618/26701766821_7bea494826.jpg)<!-- width="30%" -->
```

Daraus entsteht folgende Darstellung:

--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
Markdown is the basis of *Liascript*. However, the features integrated in this description language do not meet the requirements of interactive learning content. For example, Markdown supports by default:

**Lists**

1. in
2. orded,

   * unordered or
   * embedded structure

**Tables**

| Header 1   | Header 2   |
| :--------- | :--------- |
| Item 1     | Item 2     |

**Images**

![images](https://farm2.static.flickr.com/1618/26701766821_7bea494826.jpg)<!-- width="30%" -->

-------------------------------------------------------------------------------

### Integration of media content

     {{0-3}}
********************************************************************************

**Text-to-Speech Output**

The variable speech output of *LiaScript* you've already used. The integration
of notes, actual content and voices can be implemented with 32 languages.
Click right...

********************************************************************************

     {{1-3}}
********************************************************************************

... ...to hear a German text output. The sentences are not recorded but defined
by writen paragraphs. The German text you just heard, based on the following
code fragment:

```
    --{{1 Deutsch Male}}--
Hallo, dies ist eine deutsche Textausgabe, die die Flexibilität von LiaScript bezüglich der
Sprache deutlich machen soll.
```

    --{{1 Deutsch Male}}--
Hallo, dies ist eine deutsche Textausgabe, die die Flexibilität von LiaScript bezüglich der
Sprache deutlich machen soll.

The multilingualism of *LiaScript* affects various elements. Entire courses, individual explanations can be translated and used internationally. By the way, the language of the execution environment can be configured in the header of a document. Supporting elements  and references will also appear in the respective language.

********************************************************************************

     {{2-3}}
********************************************************************************

**Embedding movies**

Furthermore LiaScript supports the integration of movies and sound samples by

``` markdown
 ?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)
!?[video](https://www.youtube.com/watch?v=bICfKRyKTwE)
```

There are separate configuration interfaces for both media types, which allow to define the start time and the display size. Try it out !

?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)

!?[video](https://www.youtube.com/watch?v=bICfKRyKTwE)

********************************************************************************


                                       {{3-5}}
********************************************************************************

**And now all together**

In LiaScript, you can dub the videos by adding text-to-speech voices. That's much more flexible than adapting the audio track directly. Let's first take a look at the original video of the Youtube user Björn Seidler, which can be found at the following [link](https://www.youtube.com/watch?v=qAh6P1MaYtU). At the start of the video you will hear audio track spoken in German. We switch the language and "reuse" the movie content.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qAh6P1MaYtU?start=15&controls=0&showinfo=0&rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

********************************************************************************

--{{4}}--
In this video we focus on the concepts of the analog-to-digital converters. We will start with a look at the Atmel 8 bit controller manual. You see the basic features that I mark with the mouse.

                                       {{4-5}}
********************************************************************************

This is now the dubbed version using the LiaScript speech output. The audio is available as written text and can be adapted as desired.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qAh6P1MaYtU?start=15&controls=0&mute=1&showinfo=0&rel=0&autoplay=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

********************************************************************************


### Diagrams

Diagrams are an essential element when dealing with technical topics. The diagram contained in the course description is converted into a descriptive form by the interpreter. This means that no further tools are required for simple representations, whose content would have to be adapted with each iteration.


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

JavaScript based diagrams can also be embedded directly in the LiaScript document. This code fragment generates an xy diagram. The parameters can be adjusted at presentation time.


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

*LiaScript* integrates 12 different variants of quizzes that can be
intensifiy the learning process by a self-testing.

    --{{0}}--
The examples for quizzes show the LiaScript code in the upper area, in below the display in the browser. The overall syntax allows to specify the format, solutions, but also aids for the learner.

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

The crosses mark very intuitively the correct solutions for the multiple choice test.
This example illustrates how additional help for the learner
can be integrated. A question mark now appears next to the "i" for the solution.

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

### Executable code

--{{0}}--
Executable code is particularly important for programming training in computer science. These can be program snippets that generate a graphical feedback
or provide an output to the console. With the browser internal
interpreter, all kinds of tools that offer a JavaScript interface can be integrated. Click on the button below the code block to execute them. Change the code, for example to redefine the color or to adapt the size of the circle.

In this example, the Processing Toolchain, which is a JavaScript implementation, has been integrated into LiaScript. You can embed this using an 'include' above the associated macro.

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


Alternatively, you can integrate one of 32 programming languages, which can be accessed via
a web service can be integrated. The advantage of this is that you can use it without
complex installation processes. Your browser becomes your development environment. The following fragment shows an example from a
[Computer Science class](https://liascript.github.io/course/?https://raw.githubusercontent.com/SebastianZug/SoftwareprojektRobotik/master/00_Einfuehrung.md#1),
that was used in a lecture created in LiaScript.

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

## Distributed version management

    --{{0}}--
But how is the distributed development of a LiaScript course realized?
The present "lecture" itself is hosted on Github, a platform for
hosted the software development. There you will find millions of open source projects, now also the code for this document.

You can download the *LiaScript* document behind this course at
[Link](https://github.com/SebastianZug/WillkommenAufLiaScript). Unfortunately, GitHub supports only the conventional markdown, so that some elements are not displayed correctly in the preview.

The following screenshot shows the overview of the versions since December 1st. With this overview the contributors and their changes can be tracked individually.

![GitHub](./images/ScreenshotGitHub.png)<!-- width="80%" -->
*Overview of the status of the versions on 3.12.2019*

## Editor

    --{{0}}--
LiaScript documents can be edited with any text editor. In order to support LiaScript users, we developed plugins for an open source editor adapted. Atom is a free editing tool for text and code, that is available for Windows, Linux and Mac OS.

Currently there are two extentions of the [Atom Editor](https://atom.io/), which
support the development of learning content with a preview and code snippets

[liascript-preview](https://atom.io/packages/liascript-preview): The Previewer
gives the user immediate feedback for his work. While in the left
window LiaScript code is entered, the output appears immediately on the
right side.

![previewer](https://raw.githubusercontent.com/andre-dietrich/liascript-preview/master/preview.gif)<!-- style="width: 100%" -->

[liascript-snippets](https://atom.io/packages/liascript-snippets): To have certain LiaScript constructs quickly at hand, this plugin integrates small fragments and examples. The user simply enters a shortcut of the intended content, for example 'liaQuiz' and a selection menu appears, displaying all possible variants of quizzes.

![snippets](https://raw.githubusercontent.com/andre-dietrich/liascript-snippets/master/preview.gif)<!-- style="width: 100%" -->

## Integration

Since the winter semester 2017/18, LiaScript is used to design lectures in computer science at the Otto-von-Guericke University and the TU Bergakademie Freiberg. The seamless integration of respective materials in the teaching-learning environments of both  universities ensures a high level of acceptance.

![Logo](./images/Screenshot.png)<!-- width="80%" -->
*Integration of the LiaScript-based Lecture "Softwareprojekt" in the learning management system of the TU Bergakademie Freiberg (OPAL)*

## Kontakt

Have we made you curious? You can find further information on the project website

https://liascript.github.io/

![Logo](./images/logo.png)<!-- width="20%" -->


| Dr. Andrè Dietrich | andre.dietrich@ovgu.de |
| Prof. Dr. Sebastian Zug | sebastian.zug@informatik.tu-freiberg.de |
