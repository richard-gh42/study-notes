Siehe [[../geogebra/Frösche.ggb|Frösche]]
Sowie "../programme/amphibianSort/"

## Das Problem
### Schritte
Legende: 
F = Frosch
K = Kröte
v = Vor
ü = Überspringen

| **move**   | 1.     | 2.     | 3.     | 4.     | 5.     |
| ---------- | ------ | ------ | ------ | ------ | ------ |
| **01**     | Fv     | Fv     | Fv     | Fv     | Fv     |
| **02**     | Kü     | Kü     | Kü     | Kü     | Kü     |
| ==**03**== | ==Fv== | Kv     | Kv     | Kv     | Kv     |
| **04**     |        | Fü     | Fü     | Fü     | Fü     |
| **05**     |        | Fü     | Fü     | Fü     | Fü     |
| **06**     |        | Kv     | Fv     | Fv     | Fv     |
| **07**     |        | Kü     | Kü     | Kü     | Kü     |
| ==**08**== |        | ==Fv== | Kü     | Kü     | Kü     |
| **09**     |        |        | Kü     | Kü     | Kü     |
| **10**     |        |        | Fv     | Kv     | kv     |
|            |        |        |        |        |        |
| **11**     |        |        | Fü     | Fü     | Fü     |
| **12**     |        |        | Fü     | Fü     | Fü     |
| **13**     |        |        | Kv     | Fü     | Fü     |
| **14**     |        |        | Kü     | Fü     | Fü     |
| ==**15**== |        |        | ==Fv== | Kv     | Fv     |
| **16**     |        |        |        | Kü     | Kü     |
| **17**     |        |        |        | Kü     | Kü     |
| **18**     |        |        |        | Kü     | Kü     |
| **19**     |        |        |        | Fv     | Kü     |
| **20**     |        |        |        | Fü     | Kü     |
|            |        |        |        |        |        |
| **21**     |        |        |        | Fü     | Fv     |
| **22**     |        |        |        | Kv     | Fü     |
| **23**     |        |        |        | Kü     | Fü     |
| ==**24**== |        |        |        | ==Fv== | Fü     |
| **25**     |        |        |        |        | Fü     |
| **26**     |        |        |        |        | Kv     |
| **27**     |        |        |        |        | Kü     |
| **28**     |        |        |        |        | Kü     |
| **29**     |        |        |        |        | Kü     |
| **30**     |        |        |        |        | Fv     |
|            |        |        |        |        |        |
| **31**     |        |        |        |        | Fü     |
| **32**     |        |        |        |        | Fü     |
| **33**     |        |        |        |        | Kv     |
| **34**     |        |        |        |        | Kü     |
| ==**35**== |        |        |        |        | ==Fv== |

### Algorithmus

**Regeln**:

1. Wenn möglich, überspringt eine Amphibie eine Amphibie anderer Art. 
2. Ist 1. nicht möglich, springt, wenn möglich, eine Amphibie die sich bisher nicht bewegt hat nach vorne.
3. Sind weder 1. noch 2. möglich springt eine Amphibie, die hierzu in der Lage ist, ein Feld nach vorn.

