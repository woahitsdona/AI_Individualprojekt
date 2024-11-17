# AI_Individualprojekt - Effiziente Bildverarbeitung und Speicheroptimierung für semantische Segmentierung

## Projektübersicht
### Beschreibung 
Die Verarbeitung von Bildern in neuronalen Netzen ist oft herausfordernd, da hohe Auflösungen zu Memory-Errors führen können. In der Vorstudie der Bachelorarbeit wurde deutlich, dass es schwierig ist, Originalbildgrössen beizubehalten, ohne Speicherprobleme zu verursachen. Gleichzeitig beeinflussen Anpassungsschritte wie Resizing oder die Zerlegung in Batches die Qualität der Segmentierungsergebnisse.

Das Ziel dieses Projekts ist es, ein tieferes Verständnis für diese Problematik zu entwickeln. Es soll analysiert werden, wie sich gewisse Vorverarbeitungsmethoden auf die Segmentierungsqualität auswirken um ausreichend aussagekräftige Ergebnisse für die Berechnung der IoU-Statistik zwischen den Ground-Truth-Masken und den Modellvorhersagen zu liefern. Durch diese Analyse soll ein besseres Verständnis für die Balance zwischen Speicherbedarf, Bildgrösse und Modellgenauigkeit geschaffen werden.

### Projektziele
- Analyse des Speicherbedarfs von Deep-Learning-Modellen.
- Untersuchung von Bildvorverarbeitungsschritten in Python, wie Resizing und Normalisierung.
- Validierung der semantischen Segmentierung bei kleinen vs. grösseren Datensätzen.
 
### Modell und Daten
Da im Rahmen dieses Projekts nicht dasselbe Modell und derselbe Datensatz wie in der Bachelorarbeit  verwendet werden dürfen, erfolgt die Analyse der Fragestellungen mit dem klassischen U-Net-Modell und dem Cityscapes-Datensatz. Die Labels und die Thematik der Segmentierung sind thematisch passend zur Bachelorarbeit, jedoch ohne direkte Überschneidung, um die Eigenständigkeit des Projekts zu gewährleisten.


## Verzeichnisstruktur

### Individualprojekt_AI_HS24_Liridona_C.py

## Bibliotheken und Tools









