## Normalformen
### Disjunktive Normalform
Ist die Darstellung von Logischensätzen in der Form:
$$
(a \land b \land c) \lor (\lnot a \land \lnot b \land c) \lor (a \land \lnot b \land c)
$$
Das hier angegebene Beispiel hätte folgende Werte

| a   | b   | c   |     | y   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   |     | 0   |
| 0   | 0   | 1   |     | 0   |
| 0   | 1   | 0   |     | 0   |
| 0   | 1   | 1   |     | 0   |
| 1   | 0   | 0   |     | 0   |
| 1   | 0   | 1   |     | 1   |
| 1   | 1   | 0   |     | 1   |
| 1   | 1   | 1   |     | 1   |

### Konjunktive Normalform
Ist die Darstellung von logischen Sätzen in der Form:
$$
(a \lor b \lor c ) \land (\lnot a \lor \lnot b \lor c) \land (a \lor \lnot b \lor c)
$$
Was z.B. in dieser werte Tabelle darstellbar ist:

| a   | b   | c   |     | y   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   |     | 0   |
| 0   | 0   | 1   |     | 1   |
| 0   | 1   | 0   |     | 0   |
| 0   | 1   | 1   |     | 1   |
| 1   | 0   | 0   |     | 1   |
| 1   | 0   | 1   |     | 1   |
| 1   | 1   | 0   |     | 0   |
| 1   | 1   | 1   |     | 1   |
### Disjunktive Minimalform

### Konjunktive Minimalform

## Karnough-Vietch-Diagramme
Diese Helfen die DMF zu finden.

|     |     | A   | A   |     |     |
| --- | --- | --- | --- | --- | --- |
|     | 1   | 0   | 0   | 1   |     |
| B   | 0   | 1   | 1   | 0   |     |
| B   | 0   | 1   | 1   | 1   | D   |
|     | 1   | 0   | 1   | 1   | D   |
|     |     |     | C   | C   |     |
Dieses diagram kann stellt folgenden Satz dar:
$$
\lnot(A \lor B) \lor (A \land B) \lor (C \land B)
$$
Bzw.:
$$
(A \leftrightarrow B) \lor (C \land B)
$$
Das ist jedoch keine 
## Begriffe
### Don't Cares
Ergebniss dessen Wert irrelevent ist.
wird meist ddurch "x" oder "-" markiert