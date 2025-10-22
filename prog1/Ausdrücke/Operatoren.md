## Operatoren
Operatoren haben eine sog. Stelligkeit, also wie viele Operanten sie als Eingabe haben.
### Arithmetische Operatoren

| Operator | Stelligkeit | Beduetung        |
| -------- | ----------- | ---------------- |
| +        | 1           | pos. Vorzeuicehn |
| -        | 1           | neg. Vorzeichen  |
| +        | 2           | Summe            |
| -        | 2           | Differenz        |
| *        | 2           | Produkt          |
| /        | 2           | Quotient         |
| %        | 2           | mod              |
| ++       | 1           | Präinkrement     |
| --       | 1           | Prödekrement     |
| ++       | 1           | Postinkrement    |
| --       | 1           | Postdekrement    |
**Wichtig:** Bei Intengern ist das Ergebnis des Quotienten ganzzahlig.

**Wichtig:** Ob das Inkrement vor oder nach dem Operanten kommt, ist relevant, wenn der Wert des Operanten im selben Ausdruck einer anderen variable zugewiesen wird. Handelt es sich um ein Präinkrement, geschieht das Inkrementieren vor der Zuweisung ansonsten danach. Beim Dekrement ist dies ebenfals der Fall.

### Logische Operatoren
#### Vergleichsoperatoren

| Operator | Stelligkeit | Bedeutung      |
| -------- | ----------- | -------------- |
| ==       | 2           | Gleich         |
| !=       | 2           | Ungleich       |
| <        | 2           | Kleiner        |
| <=       | 2           | Kleiner-Gleich |
| >        | 2           | Größer         |
| <=       | 2           | Größer-Gleich  |
#### Andere

| Operator | Stelligkeit | Bedeutung |                       |
| -------- | ----------- | --------- | --------------------- |
| !        | 1           | NOT       | Hat höchste Priorität |
| &        | 2           | AND       |                       |
| \|       | 2           | OR        |                       |
| &&       | 2           | AND (SCE) |                       |
| \|\|     | 2           | OR  (SCE) |                       |
| ^        | 2           | XOR       |                       |
Eine **Short-Circuit-Evaluation** (SCE) bedeutet, dass der 2. Wert nur überprüft wird, wenn er das Ergebnis verändern kann. Entstehen bei der Überprüfung Nebeneffekte ist es möglicherweise notwendig beide Seiten zu überprüfen, ansonsten ist, SCE ist jedoch schneller.

##### Beispiele

| x     | y     | x&y   | x\|y  | x^y   | !x    | !x&y  |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| true  | true  | true  | true  | false | false | false |
| true  | false | false | true  | true  | false | false |
| false | true  | false | true  | true  | true  | true  |
| false | false | false | false | false | true  | false |

### Zuweisungsoperatoren

| Operator | Stelligkeit | Bedeutung               | Effekt                                 |
| -------- | ----------- | ----------------------- | -------------------------------------- |
| =        | 2           | Zuweisung               | "a = b" weist a den Wert von b zu      |
| +=       | 2           | Additionszuweisung      | "a += b" ist equivalent zu "a = a + b" |
| -=       | 2           | Subtraktionszuweisung   | s.o.                                   |
| *=       | 2           | Multplikationszuweisung | s.o.                                   |
| &=       | 2           | AND-ZUweisung           | "a &= b" bedeutet "a = a == b"         |
| ...      |             |                         |                                        |
Zuweisungsoperatoren geben den zugewiesenen Wert zurück.

### Bitwise Operatoren

| Operator | Stelligkeit | Bedeutung      | Effekt                                                        |
| -------- | ----------- | -------------- | ------------------------------------------------------------- |
| \|       | 2           | Bitwise OR     |                                                               |
| &        | 2           | Bitwise AND    |                                                               |
| >>       | 2           | Bitshift right | "a>>b" Bitshiftet a um b nach rechts vorzeichen wird erhalten |
| >>>      | 2           | Bitshift right | s.o. das Vorzeichen wird nicht erhalten.                      |
| <<       | 2           | Bitshift left  | s.o. nach links                                               |
| ^        | 2           | Bitwise XOR    |                                                               |
| ~        | 1           | Bitwise NOT    |                                                               |

### Weitere Operatoren

| Operator | Stelligkeit | Bedeutung          | Effekt                                                                                           |
| -------- | ----------- | ------------------ | ------------------------------------------------------------------------------------------------ |
| ?        | 3           | Bedingter Operator | "a = b ? c : d" weist a den Wert von c zu wenn b true ist, und denn Wert von d wenn b false ist. |
Der "?" Operator sollte meist nicht genutzt werden.