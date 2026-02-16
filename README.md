Hier ist der Text, transformiert in ein professionelles, GitHub-optimiertes Markdown-Format.

---

# Detektion und Klassifikation von Mundschutz-Maskentypen mit neuronalen Netzen

Dieses Repository enthält die Dokumentation und theoretische Grundlage der Bachelorarbeit zum Thema **„Detektion und Klassifikation verschiedener Mundschutz-Maskentypen unter Verwendung neuronaler Netze“**. Die Arbeit wurde an der Technischen Hochschule Deggendorf im Studiengang Internet of Things erstellt.

<p align="center">
<img src="./1iwkldoq.png" alt="THD Logo" width="400"/>
</p>

## Table des matières

* [Überblick](https://www.google.com/search?q=%23%C3%BCberblick)
* [Abstract](https://www.google.com/search?q=%23abstract)
* [Einleitung](https://www.google.com/search?q=%23einleitung)
* [Theoretische Grundlagen](https://www.google.com/search?q=%23theoretische-grundlagen)
* [Computer Vision](https://www.google.com/search?q=%23computer-vision)
* [Deep Learning & Neuronale Netze](https://www.google.com/search?q=%23deep-learning--neuronale-netze)
* [Objekterkennung (DNN)](https://www.google.com/search?q=%23objekterkennung-dnn)


* [Methodik & Architektur](https://www.google.com/search?q=%23methodik--architektur)
* [YOLO (You Only Look Once)](https://www.google.com/search?q=%23yolo-you-only-look-once)
* [Vergleich: Single-Shot vs. Two-Stage](https://www.google.com/search?q=%23vergleich-single-shot-vs-two-stage)


* [Technische Stack](https://www.google.com/search?q=%23technische-stack)
* [Projektstruktur](https://www.google.com/search?q=%23projektstruktur)

---

## Überblick

* **Autor:** Aboudou Koffitse
* **Hochschule:** Technische Hochschule Deggendorf (Fakultät Angewandte Informatik)
* **Studiengang:** Internet of Things (B.Eng.)
* **Prüfer/Betreuer:** Prof. Dr. Marcus Barkowsky, Prof. Dr. Peter Faber
* **Datum:** 01.08.2021 (Abgabe) / 31.01.2022 (Erklärung)

---

## Abstract

Die COVID-19-Krise hat weltweit Maßnahmen wie die Maskenpflicht hervorgebracht. Die manuelle Kontrolle der Maskentypen und der korrekten Trageweise ist im öffentlichen Raum jedoch schwierig. Diese Arbeit untersucht den Einsatz von **Deep Learning** und **Convolutional Neural Networks (CNN)** zur automatisierten Erkennung.

Das Ziel ist nicht nur die bloße Feststellung, ob eine Maske getragen wird, sondern die Differenzierung zwischen verschiedenen Typen (OP-Maske, FFP2, Gesichtsschutz) sowie die Analyse der Trageweise (Mund- und Nasenschutz). Hierzu wird ein modifizierter **YOLOv3-Ansatz** verwendet und eine spezifisch annotierte Bild-Datenbank erstellt.

---

## Einleitung

### Zielsetzung

Untersuchung von Bildverarbeitungsarchitekturen zur Klassifikation von Menschen mit und ohne Maske. Fokus liegt auf der Ermittlung der Leistungsfähigkeit und Genauigkeit der Netzwerke unter realen Bedingungen.

### Aufbau der Arbeit

1. **Einleitung & Zielsetzung**
2. **Theorie Computer Vision**
3. **Deep Learning Grundlagen**
4. **Objekterkennung mit DNN (CNN & YOLO)**
5. **Gesichtserkennung vs. Maskenerkennung**
6. **Modifizierter YOLO-Ansatz & Experimente**
7. **Fazit & Ausblick**

---

## Theoretische Grundlagen

### Computer Vision

Computer Vision ermöglicht die Analyse von Kameradaten mittels KI. Der Prozess umfasst:

* Datenerfassung
* Vorverarbeitung
* Analyse/Erkennung
* Prädiktion basierend auf extrahierten Informationen.

### Deep Learning & Neuronale Netze

Inspiriert vom menschlichen Gehirn nutzen diese Systeme **Perzeptrone** (künstliche Neuronen), um Merkmale in Daten iterativ zu erlernen.

* **Einschichtige Perzeptrone:** Für linear separierbare Probleme.
* **Mehrschichtige Perzeptrone (MLP):** Höhere Rechenleistung für komplexe Muster.

---

## Methodik & Architektur

### Objekterkennung (DNN)

In der Arbeit werden insbesondere **Convolutional Neural Networks (CNN)** behandelt, die durch Faltungsschichten (Filters), Pooling Layer und Fully-connected Layers Merkmale aus Bildern extrahieren.

### YOLO (You Only Look Once)

YOLO ist ein zentraler Bestandteil dieser Forschung. Im Gegensatz zu klassischen Methoden betrachtet YOLO die Objekterkennung als ein einziges Regressionsproblem.

* **YOLOv3:** Nutzt eine Residual-Block-Struktur und Anchor-Boxen zur präzisen Lokalisierung.
* **Metriken:** Bewertung erfolgt über IOU (Intersection over Union) und Non-maximum Suppression.

### Vergleich: Single-Shot vs. Two-Stage

| Merkmal | Single-Shot (SSD/YOLO) | Two-Stage (R-CNN/Faster R-CNN) |
| --- | --- | --- |
| **Geschwindigkeit** | Sehr hoch (Echtzeit) | Langsamer |
| **Genauigkeit** | Tendenziell niedriger | Sehr hoch |
| **Vorgehensweise** | Ein einziger Durchgang | Region Proposals + Klassifikation |

<p align="center">
<img src="./ujv1oblv.png" alt="Comparison SSD vs Two-Shot" width="600"/>





<em>Abbildung 1: Vergleich der Meta-Architekturen (Quelle: Clear.ml)</em>
</p>

---

## Technische Stack

Die Implementierung basiert auf modernen Computer Vision Bibliotheken:

* **Sprache:** Python
* **Bibliotheken:** OpenCV, TensorFlow/Keras (MobileNetV2), Darknet (YOLO)
* **Hardware:** GPU-beschleunigtes Training für tiefe neuronale Netze

---

## Projektstruktur

Das Inhaltsverzeichnis der Arbeit gliedert sich wie folgt:

* `1. Einleitung`
* `2. Computer Vision Grundlagen`
* `3. Deep Learning & KNN`
* `4. Objekterkennung mit DNN`
* `5. Gesichtserkennung zu Maskenerkennung`
* `6. Modifizierter YOLO-Ansatz`
* `7. Fazit`

---

> **Hinweis:** Dies ist eine strukturierte Zusammenfassung der Bachelorarbeit von Aboudou Koffitse. Alle Rechte liegen beim Autor und der THD.
