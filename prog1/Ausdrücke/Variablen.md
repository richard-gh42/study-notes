## Was
Variablen speichern Werte, auf die später im Programm zugegriffen werden soll. Das können primitive Typen wie int oder Pointer zu Objekten wie Strings sein.
## Warum
Werte müssen zwischengespeichert werden und anschließend wieder Aufrufbar sein diese Funktion übernehmen Variablen.
## Erklärung
Eine Variable wird wie folgt erklärt:
\[access\] \[static\] \[final\] \[type\] \[name\];
```java
private String exampleVar; 
```

|                          | Auswirkung                                       | Werte                              |
| ------------------------ | ------------------------------------------------ | ---------------------------------- |
| [[Access Level\|access]] | Von wo kann mit der Variable interagiert werden? | public, protectet, private, [None] |
| [[Static\|static]]       | Handelt es sich um eine Klassen variable?        | static, [None]                     |
| final                    | Handelt es sich um eine Konstante?               | final, [None]                      |
| type                     | Bestimmt den type der Variable                   | Alle Typen                         |
## Zuweisung
Einer Variable kann ein Wert zugewiesen werden. Dies geschieht wie folgt:
```java
exampleVar = "Hello World";
```
### Initialisierung
Die Initialisierung ist die erste Zuweisung einer Variable. Vor dieser Zuweisung kann der Wert einer Variable nicht aufgerufen werden, da es keinen Wert gibt.
Die Initialisierung kann gleichzeitig mit der Erklärung geschehen, was wie folgt aussieht:
```java
public double anotherExample = 20.0;
```
## Konstanten
Der Wert einer Konstante kann nach der Initialisierung nicht mehr geändert werden.

## Global v Lokal
Eine globale Variable ist eine Variable, die in einer Klasse erklärt wird, während eine lokale Variable in einem Codeblock erklärt wird. Globale Variablen sind von überall in der Methode aufrufbar, lokale nur innerhalb ihres Codeblocks (wobei sie auch in inneren Codeblocks aufrufbar sind).
Eine lokale Variable kann eine globale Variable überlagern, das heißt sie kann denselben Namen haben, wodurch die globale Variable nicht mehr direkt unter ihrem Nahmen aufrufbar ist. Eine lokale Variable kann jedoch keine höher gelegene lokalen Variablen überlagern.

Globale Variablen sollten vermieden werden.