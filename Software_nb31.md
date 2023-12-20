<!--

author:   Nicolai Bach

email:    nicolai.bach@fh-potsdam.de

version:  0.0.1

language: de

narrator: Deutsch Female

dark: false

comment:  Teil-Modul zum Bereich “Software” im Kurs “IT-Kompetenzen“
					In diesem Kapitel wird allg. Software behandelt. Naturgemäß
					kommt es dabei zu Überschenidungen mit (fast) allen anderen
					Themen-Gebieten. …

link: css/callouts.css

-->

# Software

## Hello World

> The first program to write is the same for all languages:<br>
> *Print the words*<br>
> `hello, world`
>
> -- Brian Kernighan, Dennis Ritchie; The C Programming Language, 1st Edition (1978); Prentice Hall

Nahezu jedes Lehrbuch zu einer beliebigen Programmierspache und jedes Tutorial da draußen fängt mit einem ”hello, world“ Beispiel an. (Eine Ausnahme Bilden JavaScript Frameworks, dort sind es [“ToDo” Apps](https://todomvc.com). 😅) Das war schon in den 70ern so und hat sich bis heute nicht geändert. In der [Hello World Collection](http://helloworldcollection.de) sind 603 Beispiele gesammelt, in [diesem GitHub reposity](https://github.com/leachim6/hello-world) sind es sogar 1000.

### Fingerübung: Dein eigenes “Hallo Welt“ Programm.

{{1}} Führe das folgende Script aus indem du auf den runden Button links unter dem Code klickst.

{{2}} Ersetze in der 2. Code-Zeile den Wert `<NAME>` mit deinem Namen.

{{3}} Führe das Script erneut aus vergleiche die Ausgabe.

``` javascript
// Ersetze in der nächsten Zeile <NAME> mit deinem Namen:
const myName = '<NAME>';

const greeting = `Hello, world!\nMy name is ${myName}.`;
const promptForName = 'Bitte gib deinen Namen in dem Script ein.';
const message = myName === '<NAME>' ? promptForName : greeting;

message;
```
<script>@input</script>

<!-- class = "callout success" -->
> Herzlichen Glückwunsch, du bist nun eine Programmiererin und kannst deine eigene Software entwickeln!

### … Auswertung … 

Hier Reflexion zum Beispiel einbauen und Überleitiung zu *Datenschutz und Datensicherheit* …

## Datenschutz & Datensicherheit

In einer Welt, die von digitaler Vernetzung geprägt ist, und in der Software allgegenwärtig ist, wird der Schutz von Daten und Systemen zunehmend zu einer Priorität. Je komplexer ein System ist, umso mehr Angriffsvektoren ergeben sich. Gleichfalls steigt die Wahrscheinlichkeit, dass Fehler bei der Programmierung von Software (*Bugs*) und der Wartung von Systemen gemacht werden.

<!-- class = "callout tip with-title" -->
> Fun Fact
>
> Der Begriff *Bug* für Fehler in Software [geht tatsächlich auf ein Insekt zurück](https://education.nationalgeographic.org/resource/worlds-first-computer-bug/), der 1947 in einem Großcomputer einen Fehler verurscht hatte.

Neben technischen Aspekten spielt Vertrauen eine entscheidende Rolle im Bezug auf Sicherheit im digitalen Raum, da es die Grundlage für sichere digitale Interaktionen bildet. Vertrauen ist notwendig, damit Benutzer ihre persönlichen Informationen online teilen und digitale Dienste nutzen können. Unternehmen und Organisationen müssen Vertrauen durch transparente Datenschutzrichtlinien ([Datenschutz-Grundverordnung (DS-GVO)](https://www.bmj.de/DE/themen/digitales/DSGVO/DSGVO_node.html)), sichere Übertragungen ([Ende-zu-Ende-Verschlüsselung](https://de.wikipedia.org/wiki/Ende-zu-Ende-Verschlüsselung)) und robuste Sicherheitsmaßnahmen aufbauen.

Vertauen ist gut, Mistrauen ist besser.

Es ist wichtig, dass Nutzer eine gesunde Skepsis und kritische Haltung bewahren. Blindes Vertrauen in Online-Dienste oder  Software kann zu Sicherheitsrisiken führen. Es ist ratsam, sich über die Sicherheitspraktiken der genutzten Plattformen zu informieren, regelmäßig Passwörter zu aktualisieren und sicherheitsbewusst zu handeln. Durch eine kritische Herangehensweise können Nutzer potenzielle Bedrohungen besser erkennen und proaktiv Maßnahmen ergreifen, um ihre persönlichen Daten zu schützen.
