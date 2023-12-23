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

## Software

![](bilder/disks_dithered.png "[Original Foto](https://www.flickr.com/photos/57519914@N00/9120429846) von [jepoirrier](https://www.flickr.com/photos/jepoirrier/), lizensiert unter [CC BY-SA 2.0](https://creativecommons.org/licenses/by-sa/2.0/).")

In disem Kapitel geht es ganz allgemein um verscheiden Aspekte von Software, die nicht unmittelbar einen konkreten Anwendunsgfall betreffen, aber troztdem bei der Auswahl und Anwendung Software berücksichtigt werden sollten.

### Hallo Welt

![](bilder/hello-bob_dithered.png "[Original Bild](https://www.deviantart.com/dagadele/art/His-name-was-Robert-Paulson-575768567) von [dagadele](https://www.deviantart.com/dagadele/gallery)")

Software ist eine Ansammlung von Anweisungen, die in einer **Programmiersprachen** geschrieben werden.  Diese Anweisungen bilden Programme, die Computer ausführen, um bestimmte Aufgaben zu erledigen. Software reicht von Betriebssystemen bis zu Anwendungsprogrammen und ermöglicht die **Interaktion von Benutzern mit Computern**. Oftmals erfolgt die Interaktion über eine Grafische Benutzeroberfläche (GUI).

> The first program to write is the same for all languages:<br>
> *Print the words*<br>
> `hello, world`
>
> -- Brian Kernighan, Dennis Ritchie; The C Programming Language, 1st Edition (1978); Prentice Hall

Nahezu jedes Lehrbuch zu einer beliebigen Programmierspache und jedes Tutorial da draußen fängt mit einem ”hello, world“ Beispiel an. (Eine Ausnahme Bilden JavaScript Frameworks, dort sind es [“ToDo” Apps](https://todomvc.com). 😅) Das war schon in den 70ern so und hat sich bis heute nicht geändert. In der [Hello World Collection](http://helloworldcollection.de) sind 603 Beispiele gesammelt, in [diesem GitHub repository](https://github.com/leachim6/hello-world) sind es sogar 1000.

### I/O Beispiel

In diesem Beispiel wird ein Text ausgegeben, der eine Variable enthält. Dieser Variable wird von dir (dem Benuzter) ein Wert zugewiesen. Das nennt man eine **Benutzereingabe**. Eingaben (Input) werden verarbeitet um eine **Ausgabe** (Output) zu erzeugen. Dieser Prozess ist als **I/O** bekannt und ist fundamental für Software Anwendungen. In unserem Beispiel erfolgt die Eingabe direkt im Code, sie könnte aber genauso gut durch das Ausfüllen eines Textfeldes oder das Auslesen einer Datei erfolgen.

``` javascript
const myName = '<NAME>';

const greeting = `Hello, world!\nMy name is ${myName}.`;
const promptForName = 'Bitte gib deinen Namen in dem Script ein.';
const message = myName === '<NAME>' ? promptForName : greeting;

message;
```
<script>@input</script>

{{1}} Führe das Script aus, indem du auf den runden Button links unter dem Code klickst.

{{2}} Ersetze in der 1. Code-Zeile den Wert `<NAME>` mit deinem Namen.

{{3}} Führe das Script erneut aus vergleiche die Ausgabe.

{{4}} Versuche den Code so zu verändern, dass du eine Fehlermeldung als Ausgabe erhältst.

<!-- class = "callout info with-title" -->
> Des Pudels Kern
> 
> Eingaben beeinflussen das Verhalten von Software und können u.U. auch zu Fehlern führen.

### Bugs

![](bilder/guru3-00c06560_dithered.png "Fehlermeldung eines Amiga 500 von Commodore, [Original Foto](https://www.techtravels.org/2013/11/amiga-guru-meditation-number-00000003-00c06560/) von [keith](https://www.techtravels.org/author/keith/)")

Ein **Bug** (Englisch für Käfer) in der Software ist ein **Fehler oder eine unerwünschte Fehlfunktion**, die dazu führt, dass das Programm nicht wie beabsichtigt arbeitet. Bugs können verschiedene Ursachen haben, darunter Programmierfehler, unerwartete Eingaben (wie in userem I/O Beispiel) oder Inkompatibilitäten zwischen verschiedenen Softwarekomponenten.

<!-- class = "callout info with-title" -->
> Fun Fact
>
> 1947 wurde [der erste *echte* Bug in einem Computer](https://education.nationalgeographic.org/resource/worlds-first-computer-bug/) identifizert. Eine Motte verursachte Fehler in einem Computer and der Harvard Universiät.

Früher oder später wird dir bei der Verwednung von Software eine Fehlermeldung begegnen oder irgendetwas funktioniert einfach nicht. Wenn du Glück hast waren die Programmierer so nett in der Meldung zu beschreiben was du tun kannst um den Fehler zu beheben. Wenn du Pech hast bekommst du einfach nur kryptischen Informationsmüll und ggf. eine Nummer.

Welche der folgenden Maßnahmen erscheinen dir sinnvoll wenn dir ein Fehler in einer Software begegnet?

- [[x]] Den Fehler an die Entwickler melden
- [[ ]] Mich im Netzwerk meiner Wahl laut beschweren
- [[ ]] An etwas anderem arbeiten und hoffen, dass der Fehler nächste Woche vershwunden ist
- [[x]] In der Hilfe oder Dokumentation der Software nach einer Lösung suchen
- [[x]] Die Version der Software überprüfen und ggf. eine aktuelle installieren

### Datenschutz & Datensicherheit

In einer Welt, die von digitaler Vernetzung geprägt ist, und in der Software allgegenwärtig ist, wird der Schutz von Daten und Systemen zunehmend zu einer Priorität. Je komplexer ein System ist, umso mehr Angriffsvektoren ergeben sich. Gleichfalls steigt die Wahrscheinlichkeit, dass Fehler ([siehe Bugs](#bugs)) bei der Programmierung von Software und der Wartung von Systemen gemacht werden.

Neben technischen Aspekten spielt Vertrauen eine entscheidende Rolle im Bezug auf Sicherheit im digitalen Raum. Wir teilen alle möglichen Arten von Infomationen miteinander aus, aber auch mit Systemen wie z.B. Online-Platformen. Unternehmen und Organisationen müssen Vertrauen durch transparente Datenschutzrichtlinien ([Datenschutz-Grundverordnung (DS-GVO)](https://www.bmj.de/DE/themen/digitales/DSGVO/DSGVO_node.html)), sichere Übertragungen ([Ende-zu-Ende-Verschlüsselung](https://de.wikipedia.org/wiki/Ende-zu-Ende-Verschlüsselung)) und robuste Sicherheitsmaßnahmen aufbauen.

<!-- class = "callout danger" -->
> Vertauen ist gut, Misstrauen ist besser.

Es ist wichtig, dass Nutzer eine gesunde Skepsis und kritische Haltung bewahren. Blindes Vertrauen in Online-Dienste oder  Software kann zu Sicherheitsrisiken oder Datenverlust führen. Es ist ratsam, sich über die Sicherheitspraktiken der genutzten Plattformen zu informieren, regelmäßig Passwörter zu aktualisieren, Backups anzulegen und auch mal zu überprüfen, ob eigene Daten in einem der zahlreichen Datenlecks enthalten sind.

<!-- class = "callout tip" -->
> Auf der Seite [';--have i been pwned?](https://haveibeenpwned.com) kannst du überprüfen, ob deine E-Mail-Adresse in einem Datenleck enthalten war.

### Software für offene Beziehung gesucht

![](bilder/connect_dithered.png "[Original Bild](https://www.flickr.com/photos/rocksrain/4961264599) von [Gulia](https://www.flickr.com/photos/rocksrain/) lizensiert unter [CC BY 2.0](https://creativecommons.org/licenses/by/2.0/)")

Der Begriff **"offen"** im Kontext von Software kann verschiedene Bedeutungen haben. Einerseits bezieht es sich auf **Open Source-Software**, bei der der Quellcode für die Öffentlichkeit zugänglich ist, was es interessierten ermöglicht, sie zu überprüfen, zu modifizieren und zu teilen. Andererseits kann "offen" bedeuten, dass eine Software **interoperabel** und mit anderen Systemen **kompatibel** ist. "Offen" kan auch bedeuten, dass eine Software **erweiterbar** ist oder schlicht und einfach, dass deine Daten jederzeit für dich **zugänglich** sind.

#### Walled Gardens

Der Begriff "Walled Garden" bezieht sich auf eine geschlossene und kontrollierte Umgebung, insbesondere im Bereich der Software oder Online-Dienste. In einem "Walled Garden" kontrolliert ein Unternehmen oder eine Plattform den Zugang zu Inhalten, Anwendungen oder Diensten, indem es restriktive Maßnahmen implementiert. Dies kann dazu führen, dass Benutzer innerhalb der Plattform eingeschränkt sind und nur auf vordefinierte Inhalte oder Anwendungen zugreifen können. Typische Beispiele für "Walled Gardens" sind **geschlossene App Stores** oder Plattformen, die ihre eigenen Inhalte und Anwendungen bevorzugen und den **Zugang zu externen Quellen beschränken**.

Eine solche Umgebung hat Vorteile genauso wie Nachteile. Wie schätzt du die Apsekte in der folgenden Tabelle ein? 

- [[Vorteil] [Nachteil] [Beides]]
- [    [x]           [ ]             [ ]     ]  Sicherheit und Zuverlässigkeit
- [    [ ]           [x]             [ ]     ]  Zensurpotential
- [    [x]           [ ]             [ ]     ]  Konsistenz und Kompatibilität
- [    [ ]           [ ]             [x]     ]  Strenge Richtilinen und Kontrolle

#### Vendor lock-in

![](bilder/safe_dithered.png "[Original Bild](https://www.flickr.com/photos/15131913@N00/288491653) von [Rob Pongsajapan](https://www.flickr.com/photos/pong/) lizensiert unter [CC BY 2.0](https://creativecommons.org/licenses/by/2.0/)")

"Vendor lock-in" bezieht sich auf die Situation, in der ein Anwender so stark von einem bestimmten Anbieter (Vendor) abhängig ist, dass es schwierig oder kostspielig wird, zu einem anderen Anbieter zu wechseln.

Die Abhängigkeit kann verschiedene Formen annehmen, einschließlich

- proprietäre Datenformate
- spezifischer Schnittstellen
- individueller Softwarelösungen

Es macht also Sinn, sich ein wenig mit der Software auseinander zu setzten, bevor du sie intensiv nutzt. 

<!-- class = "callout tip" -->
> Wenn eine Software den Import und Export von Daten zulässt ist das schon mal ein gutes Zeichen.

#### Open-Source Software

![](bilder/6731974561_158e4f17b8_o_dithered.png "[Original Bild](https://www.flickr.com/photos/opensourceway/6731974561/) von [opensourceway](https://www.flickr.com/photos/opensourceway/) lizensiert unter [CC BY-SA 2.0](https://creativecommons.org/licenses/by-sa/2.0/)")

Es muss nicht immer die vorinstallierte App von Microsoft oder Apple sein. Open-Source Software (OSS) bietet eine Reihe von Vorteilen:

1. **Kosten:**
   - Die Nutzung von Open-Source Software ist oft kostenfrei.

2. **Anpassbarkeit und Flexibilität:**
   - Der Quellcode von Open-Source Software ist offen und kann von Entwicklern angepasst werden. Dies ermöglicht eine hohe Flexibilität und die Anpassung an individuelle Anforderungen.

3. **Transparenz:**
   - Die Offenlegung des Quellcodes fördert Transparenz und ermöglicht eine Überprüfung auf Sicherheitslücken oder unerwünschte Funktionen durch die Gemeinschaft.

4. **Gemeinschaftsgetriebene Entwicklung:**
   - Open-Source-Projekte werden oft von einer breiten Gemeinschaft von Entwicklern unterstützt. Dies fördert eine kollaborative Entwicklungsumgebung und den Austausch von Wissen.

5. **Sicherheit:**
   - Durch die Beteiligung der Gemeinschaft an der Überprüfung und Verbesserung des Codes kann die Sicherheit von Open-Source Software oft schneller und effektiver gewährleistet werden.

6. **Unabhängigkeit von einem Anbieter (Vendor):**
   - Open-Source Software reduziert das Risiko von "Vendor lock-in", da Nutzer nicht an einen bestimmten Anbieter gebunden sind und den Quellcode selbst kontrollieren können.

7. **Langfristige Verfügbarkeit:**
   - Die Offenheit des Quellcodes trägt dazu bei, dass Softwareprojekte auch dann fortgesetzt werden können, wenn der ursprüngliche Entwickler oder Anbieter das Projekt nicht mehr unterstützt.

8. **Globale Zusammenarbeit:**
   - Open-Source-Projekte ermöglichen es Entwicklern weltweit, zusammenzuarbeiten und innovative Lösungen zu schaffen, was zu einer breiten Vielfalt von Ideen und Perspektiven führt.

<!-- class = "callout success" -->
> Open-Source Software ist toll!

**ABER**

<!-- class = "callout warning" -->
> Achte darauf, aus welcher Quelle du Software installierst.
