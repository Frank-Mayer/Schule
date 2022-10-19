# Funktion

Eine Funktion ist eine festgelegte Prozedur.

Diese Prozedur kann Parameter entgegennehmen, Statements ausführen und Werte zurückgeben.

## Lambda Expression

Eine Funktion kann in eine Variable gespeichert werden, auch Lambda Expression genannt. So kann eine Funktion an eine andere Funktion als Parameter übergeben werden. Das nennt man dann higher order function.

```java
Consumer<Integer> action = (Integer i) -> {  
  System.out.println(i);  
};
```

## Methode

Wenn eine Funktion Teil einer Klasse ist, nennt man das Methode.

```java
class KlasseA {
	String invert(String text) {
	  if (text.length() <= 1) {
	    return text;
	  }

	  return text.charAt(text.length() - 1) + PalindromGenerator.invert(text.substring(0, text.length() - 1));  
	}
}
```

## Parameter

Um beeinflussen zu können, was eine Funktion macht, wenn sie aufgerufen wird, kann man ihr Parameter hinzufügen.

Hierbei wird wie bei Variablen der Typ und der Name des Parameters angegeben.

## Rückgabewert

Mit dem `return` Keyword, wird ein Wert aus der Funktion an den Aufrufer zurückgegeben.

## Side Effects

Wenn eine Funktion einen fremden Wert verändert, nennt man das Side Effect.

Beispiel:
```java
class KlasseA {
	String text = "text 1";

	void funktion() {
		this.text = "text 2"; // side effect
	}
}
```
