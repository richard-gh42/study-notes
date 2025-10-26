# Aufwärmübungen
### Kap3
1. Gemeinsamkeiten in den Gruppen
    1. Der Wert der Ausgabe ist unabhängig von den Eingaben
    2. Es werden immer Negationen gegenübergestellt, ist immer Falsch
2. $E \leftrightarrow N$ 
### Kap4
#### 1
a)

| $A$ | $B$ | $C$ | $A \land (B \land C)$ | $(A \land B) \land C$ | $y_{1} \leftrightarrow y_{2}$ |
| --- | --- | --- | --------------------- | --------------------- | ----------------------------- |
| 0   | 0   | 0   | 0                     | 0                     | 1                             |
| 0   | 0   | 1   | 0                     | 0                     | 1                             |
| 0   | 1   | 0   | 0                     | 0                     | 1                             |
| 0   | 1   | 1   | 0                     | 0                     | 1                             |
| 1   | 0   | 0   | 0                     | 0                     | 1                             |
| 1   | 0   | 1   | 0                     | 0                     | 1                             |
| 1   | 1   | 0   | 0                     | 0                     | 1                             |
| 1   | 1   | 1   | 1                     | 1                     | 1                             |
b)

| $A$ | $B$ | $C$ | $A \lor (B \land C)$ | $(A \lor B) \land (A \lor C)$ | $y_{1} \leftrightarrow y_{2}$ |
| --- | --- | --- | -------------------- | ----------------------------- | ----------------------------- |
| 0   | 0   | 0   | 0                    | 0                             | 1                             |
| 0   | 0   | 1   | 0                    | 0                             | 1                             |
| 0   | 1   | 0   | 0                    | 0                             | 1                             |
| 0   | 1   | 1   | 1                    | 1                             | 1                             |
| 1   | 0   | 0   | 1                    | 1                             | 1                             |
| 1   | 0   | 1   | 1                    | 1                             | 1                             |
| 1   | 1   | 0   | 1                    | 1                             | 1                             |
| 1   | 1   | 1   | 1                    | 1                             | 1                             |

#### 2
1. Da $P_{1} = \mathbb{1}$ bedeutet, dass $P_{2} = \mathbb{1}$ und dass wiederum, dass $P_{3} = \mathbb{1}$ was $P_{4} = \mathbb{1}$ bedeutet. Daher gilt $P_{1} \to P_{4}$.
2. Ja
3. Da $P_{0} \to P_{1} \to P_{2} \implies P_{0} \to P_{2}$ gilt $P_{0} \to P_{1} \to \dots \to P_{n} \implies P_{0} \to P_{n}$ 
## Leitfragen
### Kap3
1. Warum sind manche Sätze immer wahr?
    1. Weil die Satzteile so in Abhängigkeit voneinander stehen, dass der gesammte Satz immer wahr ist.
2. Warum bedeutet wenn-dann in den Sätzen unterschiedliches?
    1. $\lnot O \land \lnot M \rightarrow S$ vs $T \rightarrow M$ 
3. $=$ Kann entweder Äquivalenz anzeigen oder auf Gleichheit prüfen. $\Leftrightarrow$ zeigt Äquivalenz an.
### Kap4
1. Wieso kann man mit $\land$ und $\lor$ fast genauso rechnen wie mit $\cdot$ und $+$?
    1. All sind Kommutativ und Assoziativ
2. Wie kann man Faulheit in der Logik vorteilhaft nutzen?
    1. Um Logische Abkürzungrn zuvfinden
3. Warum müssen Komptuer nicht mehr als eine einzige logische operatieon kennen?
    1. Alle logischen Opreratoren sind aus NAND aufbaubar.
# Tautologie und Kontradiktion
### Kontradiktion
Kontradiktionen sind Sätze oder Aussageformen, die unabhängig von den Werten der Variablen immer falsch sind.
### Tautologie
Tautologien sind Sätze oder Aussageformen, die unabhängig von den Werten der Variablen immer wahr sind.
Das Symbohl mit dem eine Tautologie markiert wird ist: 
$$
\mathcal{T}
$$
$$
\begin{matrix}
\mathcal{T} & A \to A \lor B
\end{matrix}
$$
#### Äquivalenzen
Tautologische Bijunktionen werden Äquivalenzen genannt.
$$
\begin{matrix}
\mathcal{T} & A \lor B \leftrightarrow \lnot (\lnot A \land \lnot B)
\end{matrix}
$$
wird zu
$$
A \Leftrightarrow A \lor B
$$
#### Implikationen
Tautologische Subjunktionen werden Implikationen gennant.
$$
\begin{matrix}
\mathcal{T} & A \to A \lor B
\end{matrix}
$$
wird zu
$$
A \implies A \lor B
$$
kann auch Schlussfolgerung markieren
$$
A \implies B
$$
$A$ ist hier die *hinreichende Bedingung*, $B$ die "notwendige Bedingung".
#### Definition
Eine Definition bestimmt einen Begriff für einen Zustand. Ist der Zustand gegeben, wird der Begriff verwendet, ist er nicht gegeben nicht. Es handelt sich also um eine Äquivalenz.
#### Theorem
Ein Theorem ist eine beweisbare Aussage. Sie werden teils auch Sätze oder Gesetze genannt. 
## Äquivalenzumformungen
Wird eine Gleichung verändert, ohne dass sich der Wahrheitswert dieser ändert, dann handelt es sich bei der Umformung um eine Äquivalenzumformung. Hierfür sollte dass Äuivalenzzeichen verwendet werden.
## Hinreichende und notwendige Bedingungen
$$
A \to B
$$
Hier ist A die *hinreichende* Bedingung. Hinreichend in dem Sinn, dass A reicht, dass B wahr sein muss.

B wiederum ist die *notwendige* Bedingung. Notwendig in dem Sinn, dass B wahr sein muss, damit A wahr sein kann.
# Aussagenlogisches Rechnen
## Algebraische Eigenschaften logischer Operatoren
1. 
# Übungsaufgaben
## Kap3
1. $x = \pm 1 \equiv x = 1 \lor x = -1$
2. Moddelle
    1. $t = 0 \to t+1 = 2$
    2. $x_{0}<0 \equiv x_{1}=-x_{0}$
    3. $W \leftarrow F$
    4. $\lnot S \equiv B$
    5. $Q \implies R$
    6. $U \equiv (n = 1 \space (mod \space 2))$
    7. $E \implies T$
    8. $A_{E,D} \implies A_{\lnot D}$
3. Definitionen oder Theorem?
    1. D
    2. D
    3. D
    4. D
    5. T
    6. D
    7. D
    8. D
    9. T
## Kap4
# Notizen Lesung
### Duales Studium
$$
D \to V
$$
### Kommutativität von Subjunktionen
1. $A \land B \equiv B \land A$
2. $A \lor B \equiv B \lor A$
3. $(A \to B \equiv \lnot A \lor B) \land (B \to A \equiv \lnot B \lor A) \implies$

### Summe zu Produkt
$$
a + a \cdot b = a(1+b)
$$
$$
A \lor (A \land B) \equiv (A \lor A) \land (A \lor B) \equiv (A \land \mathbb{1}) \lor (A \land B) \equiv A
$$
### Vereinfachen
$$
\begin{align}
& (\lnot A \lor B) \land (\lnot B \lor C) \land (\lnot C \lor D) \\
\equiv & ()
\end{align}
$$