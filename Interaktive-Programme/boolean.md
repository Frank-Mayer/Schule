# Boolean

Der Datentyp `boolean` wird für Wahrheitswerte verwendet, er kann die Zustände `true` und `false` annehmen.

## Logische Operatoren

Logische Operatoren können nur auf boolesche Werte angewendet werden. Sie geben ebenfalls einen booleschen Wert zurück.

Der `&&` Operator ist ein logischer Operator, der die Wahrheitstabelle für die Konjunktion (und) implementiert.

```Java
true && true // true
false && true // false
true && false // false
false && false // false
```

Der `||` Operator ist ein logischer Operator, der die Wahrheitstabelle für die Disjunktion (oder) implementiert.

```Java
true || true // true
false || true // true
true || false // true
false || false // false
```

Der `!` Operator ist ein logischer Operator, der die Wahrheitstabelle für die Negation (nicht) implementiert.

```Java
!true // false
!false // true
```

## Bitweise Operationen

Bitweise Operationen können auf boolesche oder numerische Werte angewendet werden. Sie geben ebenfalls einen booleschen oder numerischen Wert zurück.

Der `&` Operator ist ein bitweiser Operator, der die Wahrheitstabelle für die Konjunktion (und) implementiert.

```Java
true & true // true
false & true // false
true & false // false
false & false // false

3 & 5 // 1 => 0011 & 0101 = 0001
1 & 2 // 0 => 0001 & 0010 = 0000
```

Der `|` Operator ist ein bitweiser Operator, der die Wahrheitstabelle für die Disjunktion (oder) implementiert.

```Java
true | true // true
false | true // true
true | false // true
false | false // false

3 | 5 // 7 => 0011 | 0101 = 0111
1 | 2 // 3 => 0001 | 0010 = 0011
```

Der `^` Operator ist ein bitweiser Operator, der die Wahrheitstabelle für die Kontravalenz (exklusives oder) implementiert.

```Java
true ^ true // false
false ^ true // true
true ^ false // true
false ^ false // false

3 ^ 5 // 6 => 0011 ^ 0101 = 0110
1 ^ 2 // 3 => 0001 ^ 0010 = 0011
```

### Bitshifts

Der `<<` Operator ist ein bitweiser Operator, der die Wahrheitstabelle für die Verschiebung nach links implementiert.

```Java
true << true // 2 => 0001 << 0001 = 0010
false << true // 0 => 0000 << 0001 = 0000
true << false // 1 => 0001 << 0000 = 0001
false << false // 0 => 0000 << 0000 = 0000

3 << 5 // 96 => 0011 << 0101 = 0110 0000
1 << 2 // 4 => 0001 << 0010 = 0100
```

Der `>>` Operator ist ein bitweiser Operator, der die Wahrheitstabelle für die Verschiebung nach rechts implementiert.

```Java
true >> true // 0 => 0001 >> 0001 = 0000
false >> true // 0 => 0000 >> 0001 = 0000
true >> false // 1 => 0001 >> 0000 = 0001
false >> false // 0 => 0000 >> 0000 = 0000

3 >> 5 // 0 => 0011 >> 0101 = 0000
1 >> 2 // 0 => 0001 >> 0010 = 0000
```
