# Paradigmen

## Objektoriertiert

Bei der Objektoriertierung verwendet man Klassen, um etwas möglichst nah an der realen Welt abzubilden.

### Vorteile

Man muss weniger umdenken, da man das bereits bestehende Gedankenkonstrukt als Code abbildet.

### Nachteile

Die Side Effects von Methoden können dazu führen, dass der Zustand von Membern nicht gewährleistet werden kann.

## Funktional

Anstelle von Klassen verwendet man oft (nicht ausschließen) Module. In einem Modul befinden sich Variablen und Funktionen. Funktionen dürfen keine Side Effects haben. Variablen sind immer `immutable` (es gibt wenige Ausnahmen).

### Vorteile

Der state von allen Speichern ist immer sichergestellt.

### Nachteile

Nicht jeder Algorithmus und nicht jedes Projekt kann vollständig Funktional implementiert werden.
