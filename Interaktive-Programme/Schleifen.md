# Schleifen / Loops

Nach dem Keyword, welches die Art der Schleife bestimmt, zum Beispiel `for`, steht der Loop-Head in Klammern. Der Head bestimmt, wie oft der Loop-Body in geschweiften Klammern danach ausgeführt wird.

## Keywords

### break

Mit `break` kann man eine Schleife abbrechen.

### continue

Mit `continue` springt man zum nächsten Schleifendurchlauf.

## Labele

Normalerweise spricht ein Keyword die direkt überliegende Schleife an.Normalerweise spricht ein Keyword die direkt überliegende Schleife an. Mit einem Label kann man eine bestimmte Schleife ansprächen.

```java
a:
while(true) {
  while(true) {
    while(true) {
      break a;
    }
  }
}
```

## For

Der Kopf einer For-Schleife besteht aus drei Teilen:

1. Variable
2. Abbruchbedingung
3. Zähler

Eine For-Schleife zählt eine Variable so lange die Abbruchbedingung erfolgreich ist, also `true` ergibt.

Zählt von 0 bis 10:

```java
for(int i = 0; i <= 10; i++) {
  System.out.println(i);
}
```

Zählt von 5 bis 1:

```java
for(int i = 5; i > 0; i--) {
  System.out.println(i);
}
```

Zahlt von 2 bis 6 in zweier Schritten:

```java
for(int i = 2; i <=6; i += 2) {
  System.out.println(i);
}
```

## While

Eine While-Schleife hat nur eine Bedingung, solange diese erfüllt ist, wird der Loop-Body ausgeführt.

```java
int i = 0;

while(i < 10) {
  System.out.println(i);

  i++;
}
```

## Do While

Hier wird zuerst die Loop-Body ausgeführt, danach wird erstmals die Bedingung abgefragt und es geht so weiter wie bei einer regulären While-Schleife.

```java
int i = 0;

do {
  System.out.println(i);

  i++;
}
while(i < 10)
```
