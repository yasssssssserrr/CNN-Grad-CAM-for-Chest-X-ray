# CNN-Grad-CAM-for-Chest-X-ray
> **Ziel:** Implementierung, Training und Evaluation eines kompakten **CNNs** zur **Binärklassifikation** (gesund vs. Pneumonie) inkl. **Grad-CAM**-Visualisierung und ausgewählten **Fine-Tuning**-Experimenten.
## Data

Datensatz: kursseitig bereitgestellte .pth-Dateien (Bildtensor + Labeltensor).

Laden & Vorverarbeitung erfolgen direkt im Notebook.

Es wird ein fester Seed genutzt, damit die Aufteilung in Train / Val / Test reproduzierbar bleibt (Details siehe Notebookzellen).

> Bitte beachten: Die Nutzung der Daten richtet sich nach der Kurslizenz bzw. den in der Aufgaben-PDF genannten Bedingungen.
## How to run

1. Notebook öffnen: notebooks/abgabe_praktikum3_aufgabe3_Ibourk_Shafieyoun.ipynb
(lokal mit GPU oder in Google Colab; Hardwarebeschleuniger GPU wählen)
2. Zellen der Reihe nach ausführen: Daten laden & Auswahl/Visualisierung -> Modell (ConvBlock, CNN) & torchinfo.summary -> Training (Gewichte, Epochen, Lernrate) -> Evaluation (Kennzahlen + Konfusionsmatrix + Report) -> Grad-CAM (Heatmaps & Overlays) -> Fine-Tuning-Varianten (Dropout, LR, Epochen) mit Vergleichstabelle
3.  (Optional) Artefakte (Plots, Heatmaps, Reports) nach outputs/ speichern.
