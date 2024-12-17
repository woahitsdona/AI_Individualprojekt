# AI_Individualprojekt - Effiziente Bildverarbeitung und Speicheroptimierung für semantische Segmentierung

## Projektübersicht
### Beschreibung 
Die Verarbeitung von Bildern in neuronalen Netzen ist oft herausfordernd, da hohe Auflösungen zu Memory-Errors führen können. In der Vorstudie der Bachelorarbeit wurde deutlich, dass es schwierig ist, Originalbildgrössen beizubehalten, ohne Speicherprobleme zu verursachen. Gleichzeitig beeinflussen Anpassungsschritte wie Resizing oder die Zerlegung in Batches die Qualität der Segmentierungsergebnisse.

Das Ziel dieses Projekts ist es, ein tieferes Verständnis für diese Problematik zu entwickeln. Es soll analysiert werden, wie sich gewisse Vorverarbeitungsmethoden auf die Segmentierungsqualität auswirken um ausreichend aussagekräftige Ergebnisse für die Berechnung der IoU-Statistik zwischen den Ground-Truth-Masken und den Modellvorhersagen zu liefern. Durch diese Analyse soll ein besseres Verständnis für die Balance zwischen Speicherbedarf, Bildgrösse und Modellgenauigkeit geschaffen werden.

### Projektziele
- Analyse Auswirkungen Kompression/Auflösungsreduktion auf Modellgenauigkeit (IoU)
- Validierung einfache vs. komplexere Task
 
### Daten
- 122 Bilder aus dem Cityscape-Datensatz
- Einfache Task: segmentiert mit Deeplabv3
- Komplexere Task: segmentiert mit OneFormer (Thesis Bezug)

### Vorgehen
- Speicheranalyse: Vergleich Speicherbedarfs Modelle
- Bildkompression: Vergleich Kompressionsmethoden
- Streaming: Test von Stream-Reading-Ansätzen für grosse Datasets (Thesis Bezug)
- Qualität: Bewertung IoU für komprimierte vs. unkomprimierte Bilder & einfache vs. komplexere Task (ausgewählte Klassen)

### Verwendete Datensätze
- Cordts u. a., „The Cityscapes Dataset for Semantic Urban Scene Understanding“. (Quelle: http://arxiv.org/abs/1604.01685)
- 
### Weitere Quellen


## Verzeichnisstruktur
#### Individualprojekt_AI_HS24_Liridona_C.ipynb


## Bibliotheken und Tools









