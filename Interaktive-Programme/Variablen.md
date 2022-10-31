# Variablen und Typen

Eine Variable ist ein Speicher.

In Java muss der Typ eines Speichers festgelegt werden.

```java
int variable = 42;
```

## Typen

| Keyword      | Beschreibung  | Wertebereich                                                                   | Bit Größe |
| ------------ | ------------- | ------------------------------------------------------------------------------ | --------- |
| `String`     | Text          | 0 bis 2147483647 Stellen Text                                                  | 16 Bit    |
| `char`       | Zeichen       | 0 bis 65535                                                                    | 16 Bit    |
| `byte`       | Ganzzahl      | -128 bis 127                                                                   | 8 Bit     |
| `boolean`    | Wahrheitswert | `true` oder `false`                                                            | 1 Bit     |
| `int`        | Ganzzahl      | $-2^{31}$ bis $2^{31}-1$                                                       | 32 Bit    |
| `long`       | Ganzzahl      | $-2^{63}$ bis $2^{63}-1$                                                       | 64 Bit    |
| `BigInteger` | Ganzzahl      | $-2^{Integer.MAX\_VALUE}$ bis $2^{Integer.MAX\_VALUE}-1$                       | 64 Bit    |
| `float`      | Kommazahl     | $3,40282347 \cdot 10^{38}$ bis $1,40239846 \cdot 10^{-45}$                     | 32 Bit    |
| `doable`     | Kommazahl     | $1,79769313486231570 \cdot 10^{308}$ bis $4,94065645841246544 \cdot 10^{-324}$ | 64 Bit    |
| `BigDecimal` | Kommazahl     | $-2^{Integer.MAX\_VALUE}$ bis $2^{Integer.MAX\_VALUE}-1$                       | 16 Bit    |

### Wahl des Datentyps

Bei Desktop Computern ist es sinnlos einen kleineren Datentyp (wie `int`) zu verwenden, um Speicherplatz zu sparen, da ein 64-Bit-Prozessor Zahlen zu 64 Bit umwandelt, um schneller rechnen zu können.

`BigInteger` und `BigDecimal` sind von davon ausgenommen, da hier anders gespeichert wird.

## Generics

Wenn man mit Datenstrukturen wie Listen arbeitet, haben diese einen generischen Typ. Dieser wird in kleiner- und größer Zeichen geschrieben.

In diesem Beispiel wird eine `ArrayList` mit dem Typ `BigInteger` verwendet.

```java
ArrayList<BigInteger> bigInts = new ArrayList<BigInteger>();
```

Es kann eingeschränkt werden, welche Typen erlaubt sind. Das ist sinnvoll, wenn man zum Beispiel ausschließlich Zahlentypen verarbeiten möchte/kann.
