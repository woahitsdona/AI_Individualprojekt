# AI_Individualprojekt - Effiziente Bildverarbeitung und Speicheroptimierung für semantische Segmentierung

## Projektübersicht
### Beschreibung 
Die Verarbeitung von Bildern in neuronalen Netzen ist oft herausfordernd, da hohe Auflösungen zu Memory-Errors führen können. In der Vorstudie der Bachelorarbeit wurde deutlich, dass es schwierig ist, Originalbildgrössen beizubehalten, ohne Speicherprobleme zu verursachen. Gleichzeitig beeinflussen Anpassungsschritte wie Resizing oder die Zerlegung in Batches die Qualität der Segmentierungsergebnisse.

Das Ziel dieses Projekts ist es, ein tieferes Verständnis für diese Problematik zu entwickeln. Es soll analysiert werden, wie sich gewisse Vorverarbeitungsmethoden auf die Segmentierungsqualität auswirken um ausreichend aussagekräftige Ergebnisse für die Berechnung der IoU-Statistik zwischen den Ground-Truth-Masken und den Modellvorhersagen zu liefern. Durch diese Analyse soll ein besseres Verständnis für die Balance zwischen Speicherbedarf, Bildgrösse und Modellgenauigkeit geschaffen werden.

### Projektziele
- Analyse Auswirkungen Kompression/Auflösungsreduktion auf Modellgenauigkeit (IoU)
- Validierung einfache vs. komplexere Task
 
### Daten
- 24 Bilder aus dem Cityscape-Datensatz
- Einfache Task: segmentiert mit Deeplabv3
- Komplexere Task: segmentiert mit OneFormer (Thesis Bezug)

### Vorgehen
- Speicheranalyse: Vergleich Speicherbedarfs Modelle
- Bildkompression: Vergleich Kompressionsmethoden
- Streaming: Test von Stream-Reading-Ansätzen für grosse Datasets (Thesis Bezug)
- Qualität: Bewertung IoU für komprimierte vs. unkomprimierte Bilder & einfache vs. komplexere Task (ausgewählte Klassen)

### Verwendete Datensätze
- Cordts u. a., „The Cityscapes Dataset for Semantic Urban Scene Understanding“. (Quelle: http://arxiv.org/abs/1604.01685)
  
### Weitere Quellen:
- DeeplabV3: https://arxiv.org/pdf/1706.05587
- OneFormer: http://arxiv.org/abs/2211.06220
- HuggingFace: https://huggingface.co/
- DeeplabV3 Benchmark (via Paperswithcode): https://paperswithcode.com/method/deeplabv3
- OneFormer Benchmark (via Paperswithcode): https://paperswithcode.com/paper/oneformer-one-transformer-to-rule-universal

## Verzeichnisstruktur
- Individualprojekt_AI_HS24_Liridona_C.ipynb  # Hauptnotebook des Projekts
- README.md                                   # Projektbeschreibung und Anleitung
- zurich_000002_000019_leftImg8bit.png        # Beispielbild aus dem Cityscapes-Datensatz
  
*Abgabevideo: Das Video, welches die Ergebnisse des Projekts demonstriert, ist auf ILIAS im Abgabeordner zu finden*

## Bibliotheken und Tools
- Hauptframeworks: Pytorch 2.3.1, (torch, torchvision)
- Datenhandling: datasets, Pillow, JSON
- Analyse & Visualisierung: NumPy, Matplotlib, tqdm
- Systemintegration: CUDA 12.1

## Anleitung zur Ausführung des Codes
1. Umgebung starten: Öffnen Sie "GPU Hub" und starten Sie ein Jupyter-Notebook-Server mit "Pytorch 2.3.1 und GPU-Unterstützung".
2. Projekt klonen:
   git clone https://github.com/IhrRepository/AI_Individualprojekt.git
   cd AI_Individualprojekt
3. Notebook auführen: Öffnen Sie das Notebook Individualprojekt_AI_HS24_Liridona_C.ipynb in JupyterLab und führen Sie die Zellen sequenziell aus, um die Daten vorzubereiten, Modelle zu trainieren und Ergebnisse zu analysieren.
