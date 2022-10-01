# Big O Notation

Die Big O Notation beschreibt die Komplexität eines Algorithmus, in Relation zur Eingabegröße $n$.

Hierbei wird beschrieben, wie viele Schritte ein Algorithmus benötigt, diese Angabe ist unabhängig vom Gerät, auf welchem der Algorithmus implementiert wurde.

Man kann den worst-case, best-case und average-case beschreiben. Gängigerweise schaut man sich den worst-case an.

## Suche einen bestimmten Eintrag in einer Liste von Namen

Die Anzahl an Einträgen der Liste ist die Eingabegröße $n$.

Man könnte alle Einträge nacheinander durchsuchen. Der Worst-case wäre dann $O(n)$, das bedeutet, dass man im schlechtesten Fall die komplette Liste durchsuchen muss.

### Divide and conquer

Mit der Annahme, dass die Liste sortiert ist, kann man schneller suchen.
Beginnend mit dem Eintrag an der Position $\frac{n}{2}$ (in der Mitte) wird dieser Eintrag mit dem gesuchten Wert verglichen, da die Liste sortiert ist, weiß man, ob sich der gesuchte Eintrag in der ersten oder der letzten Hälfte zu finden ist.
Damit hat man mit nur einer Überprüfung die Hälfte der Einträge ausgeschlossen.

**Beispiel:**

| 0         | 1     | 2      | 3    | 4      | 5    | 6     | 7     | 8      | 9     | 10  | 11   | 12    | 13   | 14    | 15     |
| --------- | ----- | ------ | ---- | ------ | ---- | ----- | ----- | ------ | ----- | --- | ---- | ----- | ---- | ----- | ------ |
| Alexander | Alina | Daniel | Emil | Emilia | Emma | Jakob | Jonas | Julian | Laura | Lea | Lena | Likas | Lina | Linus | Sophie |

Wir suchen nach `Lea`

1. An Stelle 7: `Jonas` < `Lea` (0 bis 7 können ausgeschlossen werden)
1. An Stelle 11: `Lena` > `Lea` (11 bis 15 können ausgeschlossen werden)
1. An Stelle 9: `Laura` < `Lea` (8 bis 9 können ausgeschlossen werden)
1. Bleibt nur noch 10 übrig: `Lea`

Divide and conquer ist ein Prinzip, auf dem mehrere gute Algorithmen basieren. Der Suchalgorithmus heißt binäre Suche.

Die Komplexität der binären Suche beträgt $O(log(n))$

### Hash Map / Dictionary

Eine Hash Funktion wird verwendet, um jedem möglichen Eintrag der Liste einen Schlüssel zuzuweisen.
Für dieselbe Eingabe wird eine Hash Funktion immer denselben Wert zurückgeben.

Für solche Zwecke werden besonders schnelle Hash Funktionen wie [xxhash](https://www.wikidata.org/wiki/Q28456680) verwendet.

**Beispiel:**

| 9545BF92  | F1950CB6 | 6B2BB6D5 | 4526A235 | 6D75217A | 3BEADBA7 | 9BBFBC6B | C8ED183F | 3FA07580 | 52607046 | 2914FFAC | 077C499E | 1D1C8AC4 | 2106B14C | BF9EFDF4 | DEF37243 |
| --------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- | -------- |
| Alexander | Alina    | Daniel   | Emil     | Emilia   | Emma     | Jakob    | Jonas    | Julian   | Laura    | Lea      | Lena     | Likas    | Lina     | Linus    | Sophie   |

Wir suchen nach `Lea`

```js
xxhash("Lea") = "2914FFAC"
```

Wir wissen also, dass der gesuchte Eintrag an der Position mit dem Schlüssel 2914FFAC ist.

Die Laufzeit ist hierbei konstant $O(1)$, egal wie viele Einträge, wir finden den gesuchten Eintrag direkt.
Hierbei muss man aber bedenken, dass eine Hash Funktion eine eigene Komplexität hat, die ist bei xxhash sehr gering, aber man sollte das im Hinterkopf behalten.

## Komplexitätsdiagramm

![](https://frank-mayer.github.io/Schule/Interaktive-Programme/big-o-complexity-chart.svg)
