# Modifikatoren

## final

Von einer Klasse mit dem `final` Keyword kann nicht vererbt werden.

## static

Eine Methode oder ein Feld mit dem `static` Keyword gehört zur Klasse, nicht zu einer Instanz.

```java
public class ClassA {
  public int x = 0;
}

ClassA a = new ClassA();
a.x = 1;
```

```java
public class ClassA {
  public static int x = 0;
}

ClassA.x = 1;
```
