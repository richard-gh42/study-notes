# Aussagenlogik
S.15 - 42
## Aufwärmübungen
1. negieren
    1. voll -> nicht voll
    2. schwarz -> nicht schwarz
    3. Hans mag keinen Wein aber Bier.
    4. Denise engagiert sich werder im im Terschutz noch boxt sie.
2. 
    1. Wenn-dann-Sätze sind dann falsch, wenn B nicht aus A folgt.
    2. Nein, aber B muss wahr sein wenn A wahr ist und falsch wenn A falsch ist.
## Leitfragen
1. Es werden Grundannahmen (sog. Axiome) gebraucht, auf denen die Logik fust.
2. Wenn immer Mitwoch ist, ist nie Sonntag, somit nie Montag.
3. Es handelt sich um eine Aufzählung.
## Gegenstand der Logik
* "logisch" im Sprachgebrauch meist eher ein Ersatz für offensichtlich.
* Intuition häufig ist hilfreich, basierend gerne aber auch auf falschen annahmen.
* **Logik befasst sich mit Wahren und Falschen aussagen und deren Verknüpfung.**
* Zwei Kategorien: *wahr* und *falsch*
    * *true* und *false*
    * *1* und *0*
    * Sog. Boolsche Werte
* Analog zu Binären zahlen
* Hier $\mathbb{0}$ und $\mathbb{1}$
* Die Menge der boolschen werte ist also: $\mathbb{B} = \{ \mathbb{0}, \mathbb{1} \}$

## Aussagen und Aussageformen
* Kann etwas nur wahr oder falsch sein, dann ist es eine *Aussage*
* Eine Aussage muss nicht entscheidbar sein
* Es nicht Aufgabe der Logik den Wahrheitswerrt von Aussgaen herrauszu finde, dies ist anderen Wissenschaften überlassen

### Beispiel 2.1
Aussage oder Keine Aussage?
1. Aussage
2. Aussage
3. keine Aussage
4. keine Aussage
5. Aussage
6. Aussage
7. keine Aussage
### Beispiel 2.2
Aussage oder keine Aussage?
1. ~~Aussage~~ Aussagenform
2. ~~Aussage~~ Aussagenform
3. ~~Aussage~~ Aussagenform

* Aussagenformen sind Sätze, welche einer Aussage ähneln, jedoch Variablen enthalten und erst zu einer Aussage werden, wenn diese eingefüllt wurden.

### Beispiel 2.3
1. Aussagenform
2. Aussage 
3. Aussage
4. keins
5. Aussagenform
6. Aussagenform

### Beispiel 2.5
?????

Müsste der Satz nicht äquivalent sein zu "A bedeutet, dass B oder C gilt." und damit eine Aussage sein, da A entweder bedeuten kann das B oder C wahr sind oder eben nicht?

Müsste es sich hier nicht um eine Subjunktion handeln?
$$
A \rightarrow B \lor C
$$

## Logische Operatoren

"Konjuntion" = Oder $\lor$
"Disjunktion" = Und $\land$ 
"Negation" = nicht $\lnot$

**Wichtig:** Klammern sind für klarheit notwendig

### Beispiel 2.15
Mir fält auf, dass $(A \lor \lnot B) \equiv (A \lor \lnot B \lor (A \land \lnot C))$

$\implies$ Ausdrücke können gekürtzt werden

Es gilt:
$\lnot (\lnot A) = A$
$\lnot (A \land B) = (\lnot A \lor \lnot B)$
$\lnot (A \lor B) = (\lnot A \land \lnot B)$

"Alternation" || "ausschließliche Disjunktion" = XOR $\not\leftrightarrow$

"Bijunktion" = NOT XOR $\leftrightarrow$

### Definition 2.17
Die Subjuntion bedeutet, dass B wahr sein muss, wenn A wahr ist. "Wenn A, dann B" 

$A \rightarrow B$ 

| $A$ | $B$ | $A \rightarrow B$ | $\lnot A \lor B$ |
| --- | --- | ----------------- | ---------------- |
| 0   | 0   | 1                 | 1                |
| 1   | 0   | 0                 | 0                |
| 0   | 1   | 1                 | 1                |
| 1   | 1   | 1                 | 1                |
Es gilt:
$$
(\lnot B \rightarrow \lnot A) = (A \rightarrow B)
$$
sowie:
$$
(A \leftrightarrow B) = ((A \rightarrow B) \land (B \rightarrow A))
$$

### Führerschein
Ja?

### Die 16 Binären logischen Operatoren
Für unbekannte Operatoren $\Diamond$ verwenden

0. $0$
1. $A \land B$
2. $A \land \lnot B$
3. $A$
4. $\lnot A \land B$
5. $B$
6. $A \not\leftrightarrow B$
7. $A \lor B$
8. $\lnot (A \lor B)$
9. $A \leftrightarrow B$
10. $A \land \lnot B$
11. $\lnot A \land B$
12. $\lnot A$
13. $A \rightarrow B$
14. $\lnot (A \land B)$ 
15. $\mathbb{1}$ 


### Beispiel 2.22
Es handelt sich um eine Aussage

## Präzedenz 
Auch Bindungsstärke:
$$
\overrightarrow{
\Leftrightarrow,
\rightarrow, 
\leftrightarrow,
\lor, 
\not\leftrightarrow,
\land,
\lnot,
=,
+,
\cdot,
n^{p}}
$$
$\Leftrightarrow$ Bedeutet Äquivalenz.

## Sprachliche Negierung
Die sprachliche Negierung von "Wenn A, dann muss B" ist "A und nicht B"
$$
\lnot (A \rightarrow B) \Leftrightarrow A \land \lnot B
$$
Gennerel solte eine Aussage in ihre Formale Form umgewandelt werden, dann negiert und anschließend wieder in Sprache umgewandelt werden.

### Gegenteil und Gegensatz
Das gegenteil von der Farbe Weiß ist nicht Weiß, der Gegensatz ist Schwarz.

### Gleichheitszeichen
Drei bedeutungen
0. Zuweisung
1. Vereinfachung (Ergibt)
2. Äqivalenzüberprüfung

