## Was
Eine Methode ist ein Stück Code, welches von anderen Stellen des Codes aufgerufen werden kann.
Ihr können Parameter übergeben werden und sie kann Werte zurückgeben.
## Warum?
* *Wiederverwendung von Code*
* Strukturierung in Sinnabschnitte
## Erklärung
Eine Methodenerklärung ist nach dem Schema:
\[access\] \[static\] \[return type\] \[name\](\[Parameter\]) {\[Code der Methode\]}
```java
public static int exapleMethod(int Foo, Boolean Bar) {
    //Some Code
}
```

|                          | Auswirkung                                              | Werte                                      |
| ------------------------ | ------------------------------------------------------- | ------------------------------------------ |
| [[Access Level\|access]] | Bestimmt von wo auf die Methode zugegriffen werden kann | public, protectet, private, [None]         |
| [[Static\|static]]       | Ist die Methode eine Klassenmethode?                    | static, [None]                             |
| return type              | Bestimmt welche typen die Funktion zurück gibt.         | Alle Typen, void für keinen Rückgabe Wert. |

### Prameter
Parameter sind Variablen, die ihren Wert beim Aufrufen der Methode zugewiesen bekommen. Ihre Lebensdauer endet mit dem Ende der Funktion. 
## Überladen
Eine Klasse kann mehrere Methoden mit demselben Namen, aber unterschiedlichen Parameter haben. Dies nennt sich überladen. Java schließt hier aus dem Kontext, welche der Methoden aufgerufen wird.
## Rekursion
Eine Methode kann sich selbst aufrufen. Dieses Verhalten nennt sich Rekursion. Rekursion muss nicht zwingend innerhalb einer einzelnen Methode stattfinden. Rekursion kann zu Endlosschleifen führen oder auch als Lösungsansatz fungieren. Zu tiefe Rekursion führt zu einem StackOverflowError, wenn das Programm zu viel Arbeitsspeicher verbraucht.
## Rückgabe
Methoden können Werte zurückgeben, dies geschieht mit dem keyword "return". Der Rückgabe Wert muss nicht verwendet werden. Dies ist der Fall, wenn eine Methode als Anweisung aufgerufen wird:
```java
exampleFunc(Foo, Bar);
```
Wird eine Funktion an einer Stelle eingesetzt an der sonst eine Variable oder eine, Wert stehen würde, so wird der zurückgegebene Wert hier verwendet.
```java
int foo = exampleFunc(exampleFunc(Bar));
```
## Nebeneffekte
Nebeneffekte sind Dinge die Variablen tun, die den Zustand des Programms oder des Systems ändern, ohne ein Rückgabewert zu sein. z.B. hat die Methode println den Nebeneffekt einer Ausgabe in die Konsole. Nebeneffekte sollten vermieden und sonst gut Dokumentiert werden.
## Verhalten
0. Speicher für return value wird reserviert
1. Parameter werden l2r ausgewertet und Kopien ([[call by value]]) werden im Stack gespeichert.