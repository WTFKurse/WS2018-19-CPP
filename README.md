# C++WTF!?

## Willkommen im **(Exzellenz)kurs**

Hey ya! :v: Willkommen in unserem C++ Kurs im Wintersemester 2018/19. Bevor es losgeht, ein paar Details zu unserem Kurs

* Dienstags, 3. DS
* Ort: APB/E046
* Kursseite: www.cplusplus.wtf

Unser Kurs besteht aus drei Komponenten

<div class="panel color-1">
Präsentation
</div>

<div class="panel color-2">
Skript
</div>

<div class="panel color-3">
Praxisaufgabe
</div>

Sämtliche Slides sowie Praxisaufgaben findest du auf der Kursinternetseite der jeweiligen Kurseinheit zum Download bereit. Das Skript ist separat auf der Webseite erreichbar.

!> Für das Sammeln von Credits ist ein Nutzerkonto auf unserer Kursseite erforderlich. Eine Freischaltung erfolgt über https://cplusplus.wtf/enrollment.

### Kurstutoren

<div class="teacher-list">
	<div class="teacher">
		<div class="avatar">
			![Patrik Phan](_images/teacher_patrik.jpg 'Patrik Phan')
		</div>
		<div class="contact">
			<h4>Patrik Phan</h4>
			patrik@wtfkurse.de
		</div>
	</div>
	<div class="teacher">
		<div class="avatar">
			![Kevin Schmid](_images/teacher_kevin.jpg 'Kevin Schmid')
		</div>
		<div class="contact">
			<h4>Kevin Schmid</h4>
			kevin@wtfkurse.de
		</div>
	</div>
</div>

## Grundlagen **Programmierung**

### Grundbegriffe

<div class="column-2">
	<div>
	**Programm**<br>Ein Programm ist eine Vorschrift, nach der Informationen verarbeitet werden. Es besteht aus einer Folge von Vereinbarungen und Anweisungen. Es löst gestellte Aufgaben durch Manipulation von Daten.
	</div>
	<div>
	**Editor**<br>Ein Editor ist eine Software zur Bearbeitung und Eingabe von Programmcode (Quelltext). Er unterscheidet sich von einer komfortablen Textverarbeitung dadurch, dass er keine unsichtbaren Formatierungsanweisungen in den Text einfügt, um ihn Absätze, Listen und Tabellen zu gliedern.
	</div>
	<div>
	**Compiler**<br>Prozessoren des Computers können nur Maschinenbefehle ausführen. Compiler übersetzen den Quellcode bereits vor der Laufzeit des Programms in Maschinenbefehle.
	</div>
	<div>
	**Debugger**<br>helfen dem Programmierer beim Suchen von logischen Fehlern. Man kann Haltepunkte setzen (Breakpoints) um Variablen auf Fehler zu testen.
	</div>
	<div>
	**IDE**<br>Eine IDE ist eine Integrierte Entwicklungsumgebung (Abk. für **I**ntegrated **D**evelopment **E**nvironment) und vereint Editor, Compiler und Debugger unter einer einheitlichen Oberfläche.
	</div>
</div>


### Arten der Programmierung

#### Strukturierte Programmierung

Die strukturierte Programmierung ist die einfachste Art und Weise in der Programmierung. Innerhalb des Programmes geht man von Phasen aus, die abgegrenzt und hierarchisch sequentiell und/oder nebenläufig ausgeführt werden.


Programme werden immer komplexer, Quelltexte füllen hunderte von Seiten (führte zu einer Softwarekrise im Jahr 1970).

?> Wie können Programmerweiterungen, Verbesserungen usw. nachträglich eingebaut werden? Wie werden sie dokumentiert?


#### Objektorientierte Programmierung

**Erwartungen an das objektorientierte Paradigma**

* Wiederverwendbarkeit
* Erweiterbarkeit
* Leichte Wartbarkeit

## Einführung in **C++**

### C++ Werkzeuge

Um deinen C++ Quelltext auszuführen, gibt es zwei verschiedene Wege. Einen einfachen sowie einen etwas komplexeren Weg.

#### mittels einer IDE (einfach)
:one: Der bequemste Weg ist die Ausführung mittels einer IDE. Wir empfehlen für den Einstieg JetBrains CLion. Diese wird im Kurs weiter thematisiert.

#### mittels Compiler/Linker (komplexer)
:two: Alternativ via Compiler/Linker

1.	Quellcode in einem Texteditor eintippen und speichern
2.	Datei mit einem Compiler übersetzen und eine Objektdatei (`*.obj` oder `*.o`) erzeugen lassen
3.	Objektdatei mittels Linker binden, wodurch eine ausführbare Datei generiert wird.


### C++ Boilerplate

```cpp
#include <iostream>

using namespace std;

int main() {


   return 0;
}
```

#### Standart-Bibliotheken

Bibliotheken werden ganz am Anfang mit einer Raute (`#`) definiert. Der Name der Bibliothek steht dabei in spitzen Klammern.

 `iostream`	deklariert die C++ Basisstreamroutinen (Input/Output)

Für weitere spezielle Funktionen gibt es viele weite Bibliotheken, die nach Bedarf eingebunden werden müssen.

#### Hauptprogramm

Der komplette abzulaufende Programmcode findet im Hauptprogramm, innerhalb der `main()`-Funktion statt. Dieses wird als Dateityp int (Ganzzahl) deklariert, da wir einen Rückgabewert von „`0`“, also einer Zahl zurückgeben.

!> :point_up: Der Rückgabewert ist in C++ **essentiell**. C++ verlangt für jegliche Funktion einen Rückgabewert.

?>**WTF!? Konsole wird automatisch geschlossen**<br>Wenn ein Programm in einer Entwicklungsumgebung übersetzt wird und ausgeführt wird, passiert es oft, dass das Programm ausgeführt wird aber direkt wieder geschlossen wird. Um das Problem zu umgehen, wird zusätzlich die Bibliothek `<cstdlib>` sowie die Funktion `system("PAUSE");` im Hauptprogramm definiert.

### C++ Grundlagen

Jede Anweisung in C++ wird mit einem abschließenden Semikolon beendet. Funktionen stehen innerhalb eines Codeblocks zwischen `{ }`.

#### Bezeichner

Bezeichner sind Namen mit einer beliebigen Länge für Klassen, Objekte, Funktionen, Variablen sowie benutzerdefinierte Datentypen.

Dabei werden nur Buchstaben von **a bis z, A bis Z, Unterstriche und Ziffern** berücksichtigt. Umlaute oder sonstige (Sonder-)Zeichen sind nicht gestattet.

<mark>Sonderfall:</mark> Das erste Zeichen muss ein Buchstabe oder ein Unterstrich sein.

!> Groß- und Kleinschreibung beachten!

### Datentypen

|    Art                  	|    Datentyp    	|
|-------------------------	|----------------	|
|    Boolean              	|    bool        	|
|    Charakter            	|    char        	|
|    Ganze Zahl           	|    int         	|
|    Floating-Point       	|    float       	|
|    Doppel Gleitkomma    	|    double      	|
|    Wertlos/Nulltyp      	|    void        	|
|    Breitzeichen         	|    wchar_t     	|


### Konstanten

Eine Konstante wird behandelt wie eine Variable, welche einmalig bei ihrer Deklaration definiert wird. Für die Konstante wird `const` genutzt.

Der Wert lässt sich nicht innerhalb des Programms ändern.

```cpp
const float Pi = 3.14159;
const double Kosten = 1.85;
const char Zeichen = 'a';
```

### Operatoren

| Operatoren        | Bezeichnung                                     |
|-----------------	|------------------------------------------------	|
|    `*`   `/`   `%`    	|    Multiplikation,   Division und Rest         	|
|    `+`  `−`        	|    Addition und Subtraktion                  	  |
|    `<<`   `>>`      	|    bitweise Rechts- und Linksverschiebung    	  |
|    `<`   `<=`       	|    kleiner-als und kleiner-gleich            	  |
|    `>`   `>=`       	|    größer-als und größer-gleich              	  |
|    `==`   `!=`      	|    gleich und ungleich                       	  |
|    `&`            	|    bitweises AND                               	|
|    `^`           	|    bitweises XOR (entweder-oder)             	  |
|    `&&`              	|    logisches AND                                                                   	|
|    `=`               	|    einfache   Zuweisung (automatische Unterstützung ist in C++-Klassen Vorgabe)    	|
|    `+=`   `−=`         	|    Zuweisung   nach Addition/Subtraktion                                           	|
|    `*=`   `/=`   `%=`    	|    Zuweisung   nach Multiplikation, Division, und Rest                             	|


### Eingaben

Für die Eingaben legen wir zunächst eine Variable inklusive des Datentyps fest, unter welcher Variable die Eingabe zwischengespeichert werden soll.

```cpp
int Variable;
```

Wir haben nun eine Variable vom Datentyp `int` (Ganzzahl) deklariert. Dies initiiert, dass unsere Eingabe auch eine Ganzzahl sein soll.

Die eigentliche Eingabe funktioniert mittels dem Befehl `std::cin >>`

```cpp
std::cin >> Variable;
```

Im Gesamtbild mit dem C++ Grundgerüst sieht die Eingabe folgenderweise aus:


```cpp
#include <iostream>

using namespace std;

int main() {
   int Variable;
   std::cin >> Variable;

   return 0;
}
```

### Ausgaben

Für Ausgaben im Programm verwenden wir den Befehl `std::cout <<` mit einer anschließenden Zeichenkette in Anführungszeichen.

```cpp
std::cout<< "C++WTF!? ist cool." << std::endl;
```

Ein Zeilenumbruch wird über `<< std::endl` initiiert.

Im Gesamtbild mit dem C++ Grundgerüst sieht die Eingabe folgenderweise aus:

```cpp
#include <iostream>

using namespace std;

int main() {
   std::cout << "C++WTF!? ist cool." << std::endl;

   return 0;
}
```

### JetBrains CLion als IDE

JetBrains ist ein tschechisches Software-Unternehmen und wurde im Jahr 2000 von den drei Russen gegründet. Das Unternehmen ist seitdem für seine seit 2001 entwickelte Java-Entwicklungsumgebung (IDE) IntelliJ IDEA bekannt.

#### Download

:arrow_down: Für die Programmiersprachen C und C++ entwickelte JetBrains die IDE CLion. Die Software ist Cross-Plattform kompatibel und somit für die Betriebssysteme macOS, Linux und Windows erhältlich.

https://cplusplus.wtf/clion


#### Installation

:arrow_forward: Für die Programmierung von C++ werden einige Tools vorausgesetzt:

* CMake mind. Version 2.8.11, make
* GCC / G ++ oder Clang
* GDB 1 in Version 7.8.x-8.1.x

Die jeweiligen Tools sind abhängig von der Plattform (Windows, Linux, macOS). Alle Hinweise zur Installation findest du in den Installationshinweisen.

https://cplusplus.wtf/clioninstall

#### Lizenzierung

:heart: Studierende können über das JetBrains Education Programm sämtliche Software des Herstellers nutzen. JetBrains bietet auch außerhalb von C++ interessante Software für den Studienalltag an.

Die Anmeldung als Studierender erfolgt über die Webseite von JetBrains. Dafür ist die Verwendung der E-Mail-Adresse der TU Dresden (_@mailbox.tu-dresden.de_) notwendig.

https://cplusplus.wtf/jetbrains


### Kontrollstrukturen

Bis zum aktuellen Stand waren die bisher erstellten Programm in ihrer Ablauffolge sehr simpel. Es handelte sich bei den Programmen ausschließlich um Sequenzen von Anweisungen, die nach und nach ausgeführt wurden. Im Prinzip handelte es sich um das EVA-Prinzip.

In vielen Fällen lässt sich die lineare Programmstruktur nicht anwenden, da Anweisungen in eine Abhängigkeit gesetzt werden müssen. Realisiert wird dieser Programmablauf durch Auswahlstrukturen.


#### Einstufige Auswahl

**Bedingung mit einem positiven Zweig**

```cpp
if (Bedingung) {
    <Anweisung für ja>
}
```

#### Zweistufige Auswahl

**Bedingung mit einem positiven und negativen Zweig**

```cpp
if (Bedingung) {
    Anweisung für ja
}
else {
    <Anweisung für nein>
}
```

#### Zweistufige Auswahl

**Bedingung mit einem positiven und negativen Zweig**

```cpp
if (Bedingung) {
    <Anweisung für ja>
}
else (
    if (Bedingung) {
        <Anweisung für ja>
    }

    else {
        if (Bedingung) {
            <Anweisung für ja>
        }

        else {
            <Anweisung für nein>
        }
    }
}
```

_Alternative Variante_

```cpp
if (Bedingung) {
    <Anweisung für ja>
}
else if (Bedingung) {
        <Anweisung für ja>
}
else if (Bedingung) {
    <Anweisung für ja>
}
else {
    <Anweisung für nein>
}
```

### Zyklische Strukturen (Schleifen)

Wird eine Anweisung **mehrmals nacheinander** ausgeführt, so handelt es sich um eine zyklische Wiederholung.

| Typ                | Definition                                                                                                                |
|--------------------|---------------------------------------------------------------------------------------------------------------------------|
| Feste Schleife     | Besitzen eine festgelegte Anzahl von Schleifendurchläufen.                                                                |
| Bedingte Schleifen | Iterieren so lange, bis eine getestete Bedingung wahr wird. Der Test kann am Anfang und Ende der Schleife sein.           |
| Endlose Schleife   | Iterieren unendlich lang, bis ein bestimmter Mechanismus sie beendet (Warten auf Eingabe) Tastenkombination: Strg + Pause |


#### Merkmale

Bevor eine Schleife ausgelöst wird, muss ein Großteil der Variablen auf einem Anfangswert gesetzt werden.

Diesen **Anfangswert (Vorbedingung)** kann man durch Abfrage von Eingangswerten erhalten oder durch Festlegen von Anfangswerten, die sich später innerhalb der Schleife verändern.

!> Macht man das nicht, nimmt das Programm irgendwelche alte (irre) Werte an.

#### for-Schleife

- Es werden die Anzahl der Wiederholungen in einem Zähler festgehalten und bei Erreichen des Zählerendstandes eingestellt.
- Anweisungen werden mindestens einmal ausgeführt, bis zum Erreichen des Endstartes (So lange, bis die Bedingung wahr geworden ist)
- fehlt eine Bedingung, dann wahr
- Anweisungsblöcke zwischen ```{ }```
- ```var++``` (heißt Schleifendurchlauf +1)
- ```var--``` (heißt Schleifendurchlauf -1)

```cpp
for(A = 1; A <= 10; A = A + 2)
{
    Anweisung1;
    Anweisung2;
    Anweisungn;
}
```

**Was heißt das?**

| Code           | Erklärung                                                                              |
|----------------|----------------------------------------------------------------------------------------|
| Feste Schleife | Schleife beginnt bei A = 1, Anfangswert ist 1                                          |
| A <= 10        | Schleife wird solange ausgeführt, bis A = 10 --> danach abgebrochen „wie wird A = 10?“ |
| A = A + 2      | bei jedem Schleifendurchlauf wird A um 2 erhöht, die Schrittweite um 2 erweitert       |


!> **Besonderheiten der Zählschleife**<br />Der Datentyp der Laufvariable ist nicht auf int beschränkt, jedoch müssen Startwert und Endwert gleichen Typs sein und zur Laufvariable kompatibel.

#### while-Schleife

- Bedingung ist oft ein integer-Ausdruck
-	Separater Schleifenzähler erforderlich
- Anweisungsblöcke zwischen ```{ }```

```cpp
while(A <= 10)
{
    Anweisung1;
    Anweisung2;
    Anweisungn;
}
```

#### do-while-Schleife

-	Bedingung ist ein integer-Ausdruck
-	Wiederholung der Anweisungen solange Bedingung richtig ist
- Anzahl der Schleifendurchläufe unbekannt
-	Auswertung der Bedingung im Schleifenfuß
- Anweisungsblöcke zwischen ```{ }```

```cpp
char Zeichen;
do {
    Anweisung1;
    Anweisung2;
    Anweisungn;
}
while((Zeichen == 'j' ) || Zeichen == 'J'));
```
