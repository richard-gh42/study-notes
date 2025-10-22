## Schaltnetz 
* Ohne Rückkopplung
* Werte an den Ausgängen sind nur von Eingängen abhängig.
* Ohne Speicher
* "Kombinatorisch"
## Schaltwerk
* Mit Rückkopplung 
* Ausgabe ist abhängig von Eingängen sowie Systemstatus.
* Mit Speicher
## Synchronität
Ein getakteter Schaltkreis ist Sysnchron, ein ungetakteter Schaltkreis ist Asynchron.
## Flip-Flops
Speichern Daten synchron
### RS-Flipflop
* Set-Reset-Flip-Flop
* Set setzt Ausgabe auf 1
* Reset setzt die Ausgabe auf 0
* R und S dürfen nicht gleichzeitig 1 sein
* *Ändern sich spezifisch zu Beginn des Taktes*. 
### D-Flipflop
* Ausgang wird zum Takt an Eingang angepasst.
### T-Flipflop
* Toggled wenn der Eingang zum Takt 1 ist.
* Immer Flanken gesteuert.
### JK-Flipflop
* Jump-kill-flip-flop
* Funktioniert wie ein RS-FlipFlop solange die Eingaben einzeln wahr sind.
* Funktioniert wie ein T-FlipFlop wenn beide 

### Steuerung
* Pegelgesteuert
    * Ein Flipflop kann so lange schalten, wie der Takt wahr ist.
* Flankengestuert
    * Positive Flanke
        * Ein Flipflop schaltet wenn der Takt positiv wird.
    * Negative Flanke
        * Ein Flipflop schaltet wenn der Takt negativ wird.

## Latches
Englisch sprachiger nahme für ein Asynchrones FlipFlop 
## Register
Register bestehen klassisch aus D-Flipflops
Heute häufig aus Kondensatoren

## Beispiel Aufgaben
### 1

| x   | q'  | q        |
| --- | --- | -------- |
| 0   | 0   | 0        |
| 1   | 1   | instabil |



## Zeiten umrechnen
0. $1s \cdot 10^{0} = 1s$
1. $1s \cdot 10^{-3} = 1ms$
2. $1s \cdot 10^{-6} = 1\mu s$
3. $1s \cdot 10^{-9} = 1ns$
4. $1s \cdot 10^{-12} = 1ps$