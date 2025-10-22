## Hinweise zum Text

* Notizen manchen
* Pausen machen
* Nach Möglichkeit Kapitel nicht am Stück lesen
* Mehrfach lesen
* Kleingedrucktes sind Verknüpfungen zu anderen Themen
* Schwarze Quadrate beenden Beispiele u.ä.
* Wichtige und fremdsprachige Begriffe sind in Kursiv geschrieben
* Stift symbol fordert zu Eintragen von etwas Auf bevor weiter gelesen wird
* Empfohlene Vertiefungen sind Optional
* Lernziele sind nicht Optional
* Übungsaufgaben sind für nach der zugehörigen Lesung

## Aufwärmübungen

1. Etwas ist abstrakt, wenn es sich nicht eine Begebenheit sondern ein Konzept beschrieben ist.
   Die Formel für die Berechnung des freien Falls sind abstrakt, die Begebenheit das ein Apfel vom Baum fällt ist konkret.
2. R = Reihenfolge wichtig, V = Vielfältigkeit wichtig
    1. RV
    2. R
    3. RV

## Leitfragen

1. Wie unterscheidet sich die Bedeutung von abstrakt in der Altagssprache von der in der Informatik?
    1. Altagssprache häufig = unverständlich
    2. Eig. unvesentliches weglassen
2. warum sind Modelle in wissenschaftlicher Arbeit wichtig?
3. Warum ist es sinnvoll, verschiedene Arten vin Kollectionen zu unterscheiden?

## Abstraktion und Modellbildung

* Zahl = Abstraktion
* Abstrakte Klassen könne in Programmen praktisch sein (Inheritance)
* Abstrahieren ist wichtig zu Modellieren
* Modelle sind Beschreibungen die sich auf das (abhängig vom Zweck des Modells) wesentliche beschränken. 
* Es gibt kein richtiges Modell, nur geeignete Modelle und ungeeignete Modelle.

## Kollektionen

* 4 Arten von Kollektionen, 2 Aspekte:
    * Relevanz der Reihenfolge
    * Können sich Elemente wiederholen?

|                                   | Reihenfolge ist relevant | Reihenfolge ist nicht relevant |
| --------------------------------- | ------------------------ | ------------------------------ |
| **Mehrfachvorkommen ist möglich** | Tupel \[\]               |                                |
| **ist nicht möglich**             |                          | Menge {}                       |
* Mengen und Tupel werden, in diesem Kurs sehr häufig gebraucht werden.

## Funktionen

* Zunächst als "Black Box"
* Selbe Eingabe führt immer zur selben Ausgabe.

## Einführung in *setlX*

setlX "deklarativ" also beschreibend was berechnet wird, statt wie berechnet wird.

## Gespräch

* Ausdruck über Kollektionen ist sehr relevant
* **Wichtig:** Beim Problem beschreiben beschreibe was, dass Problem ist, nicht dass es ein Problem gibt.
* Menge Normalisieren: Doppelte Elemente entfernen und Elemente sortieren.

* Tupel
    * Vektoren, Punkte
    * Telefonnummern
    * Wort/String
* Ungeordneter Tupel
    * Einkaufsliste, Bon
* Geordnete Menge
    * Ziffern eines Zahlensystems
    * Sammelalbum
* Menge
    * Natürliche Zahlen

```setlx
z1 := {1,2,3,4};

z2 := [2,3,1,4];

  

a := {n:n in z1 | n**2<5};

b := {n:n in z2 | n**2<5};

c := [n:n in z1 | n**2<5];

d := [n:n in z2 | n**2<5];

  

print(a==b);

print(a==c);

print(a==d);

print(b==c);

print(b==d);

print(c==d);
```

Ausgabe:

```
true
false
false
false
false
false
```

## Übungsaufgaben

1. Vector, Liste, String 
2. 
    1. Ungeordnetes Tupel
    2. Menge
    3. Menge
    4. Tupel
