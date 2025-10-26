[Source](https://stackoverflow.com/a/73021)
## Generell
Es gibt zwei Wege denn wert einer Variable auf eine andere zu übertragen:
1. Call by refrence
2. Call by value
### Call By Refrence
Call by refrence übergibt eine Referenz auf die andere Variable. Wird nun der Wert einer dieser Variablen verändert, verändert er sich bei beiden.
### Call By Value
Call by value übergibt eine Kopie des Wertes an die zweite Variable. Diese ist anschließend unabhängig von der ersten.
### Beispiel
```java
int a = 0;
int b = a;
a++;
return b;
```
Diese theoretische Funktion würde unter call by refrence 1 zurückgeben und unter call by value 0.
## Java
In Java sind grundsätzlich alle Zuweisungen call by value. Keine Variable kann den Wert einer anderen Variable ändern.
### Wichtig
Hält eine Variable ein Objekt wie z.B. einen Array, dann ist der Wert der Variable ein Pointer. Das ändern Einer variable ändert dann nicht den Wert einer anderen, jedoch greifen beide auf dasselbe Objekt zu.