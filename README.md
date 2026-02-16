
# Technische Hochschule Deggendorf

---

<p align="center">
  <b>Bachelorarbeit (B.Eng.)</b> <br>
  Studiengang Internet of Things | Technische Hochschule Deggendorf
</p>


<p align="center">
  <b>Bachelorarbeit zur Erlangung des akademischen Grades:</b><br>
  Bachelor of Engineering 
</p>


## Thema:

# Detektion und Klassifikation von Mundschutz-Maskentypen mit neuronalen Netzen

Dieses Repository enthält die Dokumentation und theoretische Grundlage der Bachelorarbeit zum Thema **„Detektion und Klassifikation verschiedener Mundschutz-Maskentypen unter Verwendung neuronaler Netze“**. Die Arbeit wurde an der Technischen Hochschule Deggendorf im Studiengang [Internet of Things](https://www.th-deg.de/ai-b) erstellt.


<p align="center">
<img width="446" height="102" alt="image" src="https://github.com/user-attachments/assets/5ce5746e-41d6-4b18-9eef-7527cda8d8f2" />

</p>

## Inhaltsverzeichnis

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


---

## Motivation

Nach derzeitigem Stand kann die Ausbreitung des SARS-CoV-2 Virus durch das Tragen einer Maske über Mund und Nase gehemmt werden. Insbesondere beim Betreten von Gebäuden ist das Anlegen von Masken relevant, gleichzeitig ist aber eine individuelle, manuelle Überprüfung nur schwer umzusetzen. Daher soll im Rahmen dieser Bachelorarbeit eine erweiterte Maskendetektion durch Kamerabilder untersucht werden.

## Kurzbeschreibung

Die Verwendung tiefer neuronaler Netze (Deep Neural Networks, DNN) in der Bildverarbeitung hat insbesondere in der Objektdetektion signifikante Fortschritte ermöglicht. Ausgehend von den aktuellen DNN Architekturen soll zunächst durch Transfer-Learning die Verlässlichkeit der Detektion von Masken in Gesichtern im Allgemeinen untersucht werden.

Hierzu soll auch eine annotierte Bilddatenbank mit unterschiedlichen Kameratypen (z.B. Infrarot-, Wärmebildkamera) und Kameraauflösungen für den Einsatz in der Forschung erstellt werden. Im weiteren Verlauf der Bachelorarbeit wird die Detektion schrittweise erweitert und verfeinert, insbesondere sollen Klassen für verschiedene Maskentypen (Alltagsmaske, FFP2-Schutzmaske, Schal, Gesichtsschild, etc.) untersucht werden und die Art des Tragens (Mundschutz, Mund- und Nasenschutz) detektiert werden.

## Stichworte

*Neuronale Netzwerke

*Deep Convolutional Neuronal Networks

*Bilderkennung Objektdetektion



## Abstract

Die COVID-19-Pandemie hat weltweit vielfältige Maßnahmen zur Eindämmung der Virusausbreitung, darunter die verpflichtende Maskennutzung, hervorgerufen. Im öffentlichen Raum erweist sich die manuelle Überprüfung sowohl der verwendeten Maskentypen als auch der korrekten Trageweise als Herausforderung. Diese Arbeit befasst sich mit der Implementierung von Deep Learning und Convolutional Neural Networks (CNN) zur automatisierten Erkennung von Gesichtsmasken.

Ziel dieser Forschung ist es, über die bloße Feststellung des Maskentragens hinauszugehen und eine differenzierte Klassifizierung der Maskentypen (z. B. OP-Masken, FFP2-Masken, Gesichtsschutz) sowie die Analyse der Trageweise (insbesondere den ordnungsgemäßen Schutz von Mund und Nase) zu ermöglichen. Hierzu wird ein modifizierter YOLOv3-Ansatz entwickelt und eine eigens annotierte Bilddatenbank erstellt. Diese Methodik soll dazu beitragen, die Effizienz der Maskenkontrolle im öffentlichen Raum zu erhöhen und zugleich wertvolle Erkenntnisse für die öffentliche Gesundheit zu liefern.




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
7. **Implementierung Face Mask detektion mit python**
8. **Fazit & Ausblick**

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

<img width="799" height="1017" alt="image" src="https://github.com/user-attachments/assets/03e80947-cb24-4388-8e51-777c46cf41ca" />


<img width="758" height="949" alt="image" src="https://github.com/user-attachments/assets/d8d7ca6e-3d05-4592-acd1-d2420dcbf62f" />



<img width="792" height="898" alt="image" src="https://github.com/user-attachments/assets/913d88d2-2546-4416-ae7a-36fcf94ab4f4" />



<img width="744" height="1001" alt="image" src="https://github.com/user-attachments/assets/9398770e-b00e-47c5-a652-3d631da2c78c" />

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
*  7. Implementierung Face Maskt datection mit python`
* `8. Fazit`

---


<img width="1003" height="790" alt="image" src="https://github.com/user-attachments/assets/b882d3d8-5d86-4205-9752-629369200cdd" />

# Klassen für verschiedene Maskentypen

<img width="935" height="880" alt="image" src="https://github.com/user-attachments/assets/48f46ee7-8ef2-44d1-89ef-079d5efbb60c" />

<img width="967" height="845" alt="image" src="https://github.com/user-attachments/assets/2a520d12-6b27-476b-b6fd-029e2b552215" />

# Data Annotation 

<img width="1024" height="837" alt="image" src="https://github.com/user-attachments/assets/471a0c3f-65e2-4cd0-8b2b-c35ba62d3a0b" />

# Resultat

# Die Detektion der verschiedenen Gesichtsmaske in Echtzeit

<img width="972" height="1139" alt="image" src="https://github.com/user-attachments/assets/f7dfa0b9-e06e-4b21-aa7b-adaa87451434" />


## Hinweis: 
Dies ist eine strukturierte Zusammenfassung der Bachelorarbeit von **Aboudou Koffitse**. Alle Rechte liegen beim Autor und der THD.
