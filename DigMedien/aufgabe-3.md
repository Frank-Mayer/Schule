# Aufgabe 3

## Erläutern Sie, warum ein Mensch auf einem Farbmonitor unzählige Farben sehen kann, obwohl dieser lediglich drei unterschiedliche Farben darstellen kann. Überlegen Sie dabei auch, ob alle Lebewesen auf einem Farbmonitor dasselbe sehen, wie Menschen.

Die drei Farben sprechen die Lichtrezeptoren im Auge an. Da es einen Rezeptor für jede Farbe des Monitors gibt, merkt das Gehirn nicht, dass die Farben einzeln auftreten.

## Erläutern Sie das JPEG-Verfahren in ihren eigenen Worten.

Das Komprimierungsverfahren JPEG ist eine Mischung aus verlustbehafteter und verlustfreier Komprimierung speziell für Fotos. Die Problematik bei Fotos ist der hohe Informationsgehalt. Unregelmäßige Muster, feine Konturen, komplexe Farb- und Helligkeitsverläufe enthalten nur sehr wenige Redundanzen und sind daher ungeeignet für verlustfreie Komprimierungsverfahren.

Die Idee des JPEG Verfahrens ist es, zuerst den Informationsgehalt durch Entfernen unwichtiger Informationen zu verringern, um im Anschluss die übrigen Daten mit verlustfreier Komprimierung optimal zu reduzieren.

Der Komprimierungsvorgang besteht aus vier Schritten:
1. Umwandlung der RGB-Farbwerte in das YUV-Farbmodel
2. Umwandlung der Bilddaten von Punktinformationen in Frequenzinformationen
3. Quantifizierung der Koeffizienten der Ortsfrequenzen
4. Verlustfreie Komprimierung der Daten
