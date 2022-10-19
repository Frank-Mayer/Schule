# Klasse

Eine Klasse ist ein Bauplan für ein Objekt.

Um eine Klasse zu definieren, wird das `class` Keyword verwendet.

```java
class KlasseA {

}
```

Alles, was in dieser Klasse definiert wird, besteht auch in dem Objekt, welches aus dieser Klasse erstellt wird.

## Constructor

Mit dem `new` Keyword, wird ein neues Objekt aus einer Klasse erstellt. Dabei wird die sogenannte Constructor-Methode aufgerufen.

Ein Constructor bestellt **immer**. Wenn er nicht explizit angegeben wird, ist er `public`, besitzt keine Parameter und führt keinen eigenen Code aus.

```java
class KlasseA {
	String text = "text Inhalt";

	String updateText() {
		this.text = "neuer Inhalt";
	}
}

KlasseA objectA = new KlasseA();
```

Um auf die eigenen Inhalte zuzugreifen, wird `this` verwendet.

Um auf den Inhalt eines Objektes zuzugreifen, verwendet man den `.` Operator mit dem Objekt.

```java
System.out.println(objectA.text); // text Inhalt
objectA.updateText();
System.out.println(objectA.text); // neuer Inhalt
```

## Vererbung / Ableitung

Um Inhalte einer Klasse an eine andere weiterzugeben, kann man von dieser Klasse ableiten.

```java
class KlasseA { }
class KlasseB extends KlasseA { } // KlasseB erbt alles von KlasseA
```

## Zugriffsmodifikator

Der Zugriff auf Klassen in einem Paket sowie Inhalte von Klassen können über Zugriffsmodifikatoren gesteuert werden.

### Public

Jeder hat Zugriff

### Private

Nur die eigene Klasse kann auf ihren Inhalt zugreifen.

### Protected

Die eigene und davon abgeleitete Klassen könne auf die Inhalte zugreifen.

### Internal

Es kann nur innerhalb derselben Assembly auf die Inhalte zugegriffen werden.
