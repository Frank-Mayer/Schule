# Aufgabe 5

## Wie viel Speicherplatz benötigt ein digitaler Film von 10 Minuten in Full-HD-Auflösung bei 3 Byte Farbtiefe und 25 Bildern pro Sekunde?

```
Speichergröße = Bildbreite x Bildhöhe x Farbtiefe x Bildrate x Filmdauer
```

```
Speichergröße = 1920px x 1080px x 3B x 25 Bilder/s x 600
```
_(600 Sekunden entsprechen 10 Minuten)_

Speichergröße = 2073600000 Byte = 20 Gigabyte.

## Wie viele Sekunden unkomprimierter Full-HD-Film mit 3 Byte Farbtiefe und 25 Bildern pro Sekunde passen auf eine Single-Layer-DVD (Kapazität 4,7 GB)?

```
Sekunden = (DVD-Kapazität) / (Bildbreite x Bildhöhe x Farbtiefe x Bildrate)
```

```
Sekunden = (4,7GB) / (1920px x 1080px x 3B x 25 Bilder/s)
```

7200 Sekunden

Das entspricht etwa 120 Minuten oder 2 Stunden.

## Erläutern Sie die behandelten Basistechniken zur Videokomprimierung in ihren eigenen Worten.

- Inter-frame-Kodierung: Inter-frame-Kodierung ist eine Technik zur Kompression von Videodaten, bei der die Informationen zwischen den einzelnen Bildern (Frames) eines Videos genutzt werden, um die Datenmenge zu reduzieren. Die Inter-frame-Kodierung vergleicht dazu zwei aufeinanderfolgende Bilder und speichert nur die Unterschiede zwischen ihnen. Diese Unterschiede werden als Bewegungsvektoren bezeichnet und beschreiben, wie sich die Objekte im Bild bewegen.
- Intra-frame-Kodierung: Intra-frame-Kodierung ist eine Technik zur Kompression von Videodaten, bei der jedes Bild einzeln komprimiert wird, ohne dass die Informationen zwischen aufeinanderfolgenden Bildern genutzt werden. Die Intra-frame-Kodierung verwendet dazu verschiedene Techniken, wie zum Beispiel die Verwendung von DCT (Discrete Cosine Transformation) und Huffman-Kodierung, um die Datenmenge zu reduzieren.
- Blockmatching: Blockmatching ist eine Technik, die in der Inter-frame-Kodierung verwendet wird, um Bewegungsvektoren zu berechnen. Bei der Blockmatching-Technik werden kleine Bereiche im Bild, sogenannte Blocks, verglichen, um herauszufinden, wie sich die Objekte im Bild bewegen. Durch den Vergleich von Blocks in aufeinanderfolgenden Bildern können Bewegungsvektoren berechnet werden, die beschreiben, wie sich die Objekte im Bild bewegen. Die Bewegungsvektoren werden dann in der Inter-frame-Kodierung verwendet, um die Datenmenge zu reduzieren.
