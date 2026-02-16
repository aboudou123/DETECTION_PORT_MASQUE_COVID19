<img src="./1iwkldoq.png"
style="width:1.81861in;height:0.30625in" />

> Technische Hochschule Deggendorf
>
> Fakultät Angewandte Informatik
>
> Studiengang Internet of Things
>
> **Thema:**
>
> Deutsch: „Detektion und Klassifikation verschiedener
> Mundschutz-Maskentypen unter Verwendung neuronaler Netze.“
>
> English : " Detection and classification of various types of facemasks
> using neural networks. "
>
> Bachelorarbeit zur Erlangung des akademischen Grades:
>
> Bachelor of Engineering
>
> An der Technischen Hochschule in Deggendorf
>
> Vorgelegt von:
>
> Aboudou Koffitse
>
> Matrikelnummer: 00774763

Prüfer:

> Prof. Dr. Marcus Barkowsky
>
> Betreuer:
>
> am: 01.08.2021 Prof. Dr. Marcus Barkowsky

<img src="./fxawikbu.png"
style="width:1.81861in;height:0.30625in" />

> **Eidesstattliche** **Erklärung**
>
> Name der/des Studierenden: Professor/Betreuer an der Hochschule: 2.
> Betreuer :
>
> Koffitse Aboudou

Prof. Dr.-Ing. Marcus Barkowsky Prof. Dr. rer. nat. Peter

> **Thema** **der** **Bachelorarbeit** **(deutscher** **Titel):**
>
> *Detektion* *und* *Klassifikation* *verschiedener*
> *Mundschutz-Maskentypen* *unter* *Verwendung* *neuronaler* *Netze*.
>
> **Thema** **der** **Bachelorarbeit** **(englischer** **Titel):**
>
> *Detection* *and* *Classification* *of* *Mouth-Nose* *Mask*
> *Protection* *with* *Neu-ral* *Networks*
>
> <img src="./ngpwc50x.png"
> style="width:2.66833in;height:0.57335in" />1. Ich erkläre hiermit,
> dass ich die Bachelorarbeit selbstständig verfasst, noch nicht
> anderweitig für Prüfungszwecke vorgelegt, keine anderen als die
> an-gegebenen Quellen oder Hilfsmittel benutzt sowie wörtliche und
> sinnge-mäße Zitate als solche gekennzeichnet habe.
>
> Deggendorf, 31.01.2022
> \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
> (Unterschrift der/des Studierenden)
>
> 2\. Ich bin damit einverstanden, dass die von mir angefertigte
> Bachelorarbeit über die Bibliothek der Hochschule einer breiteren
> Öffentlichkeit zugänglich gemacht wird.
>
> <img src="./pj3xag32.png"
> style="width:0.21441in;height:0.24479in" />□ Ja □ Nein
>
> **Falls** **Ja:**
>
> <img src="./qfy4tfpk.png"
> style="width:2.66833in;height:0.57335in" /><img src="./0b3rvjzl.png"
> style="width:2.55122in;height:0.45573in" />Ich erkläre und stehe dafür
> ein, dass ich alleiniger Inhaber aller Rechte an der Ba-chelorarbeit,
> einschließlich des Verfügungsrechts über Vorlagen an beigefügten
> Abbil-dungen, Plänen o.ä., bin und durch deren öffentliche
> Zugänglichmachung weder Rechte und Ansprüche Dritter noch gesetzliche
> Bestimmungen verletzt werden.
>
> Deggendorf, 31.01.2022
> \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
> (Unterschrift der/des Studierenden)
>
> \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
> Nur bei Einverständnis des Verfassers mit einer Veröffentlichung der
> Bachelorarbeit vom Prüfer auszufüllen:
>
> Eine Aufnahme eines Exemplars der Bachelorarbeit in den Bestand der
> Bibliothek und die Ausleihe des Exemplars wird
>
> □ befürwortet
>
> <img src="./sbmuqnoa.png"
> style="width:0.23351in;height:0.23698in" />□ nicht befürwortet.
>
> Deggendorf, \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
> (Unterschrift des/der Prüfers/in)
>
> I

<img src="./rlrkv5xt.png"
style="width:1.81861in;height:0.30625in" />

> **Danksagung**
>
> An dieser Stelle möchte ich mich bei allen Personen bedanken, welche
> mich bei der Erstellung dieser Abschlussarbeit unterstützt und
> motiviert haben. Der Dank gilt in erster Linie meinem Erstprüfer Prof.
> Dr. Barkowsky, welcher diese Arbeit betreut und ermöglicht hat. Ich
> bin Prof. Dr. Barkowsky besonders dankbar für seine Unter-stützung,
> seine Verfügbarkeit, seine wertvollen Ratschläge, seine Führung und
> Er-mutigung. Die Zeit in Form von Gesprächen, welche Sie neben Ihrer
> eigentlichen Arbeit für diese Arbeit freiräumte, ist einen besonderen
> Dank wert. Ganz besonders möchte ich auch Prof. Dr. Peter Faber
> bedanken. Seine Anwesenheit während des gesamten Semesters, um uns bei
> dieser Arbeit zu unterstützen, war von größter Bedeutung.
>
> II

<img src="./pta44ig2.png"
style="width:1.81861in;height:0.30625in" />

> Inhaltsverzeichnis
>
> **Eidesstattliche**
> **Erklärung............................................................................................................I**
>
> **Abbildungsverzeichnis..............................................................................................................VI**
>
> **Abstract.....................................................................................................................................VIII**
>
> **1** **Einleitung**
> **............................................................................................................................9**
>
> 1.1Ziel
> ..................................................................................................................9
> 1.2Aufbau der
> Arbeit.............................................................................................9
> 1.3Forschungsstand.............................................................................................9
> 1.4Wissenschaftliche
> Ergebnisse.........................................................................9
> 1.4.1 Single Shot Multi Box
> Detektor...........................................................................10
>
> 1.4.2 Two-stage
> Detektion...........................................................................................10
>
> **2** **Einführung** **in** **die**
> **Computervision..................................................................................11**
>
> 2.1Computer
> Vision............................................................................................11
> 2.2Anwendungen des Computer
> Vision..............................................................11
> 2.3Bildklassifizierung..........................................................................................11
> 2.4Objekterkennung und
> Lokalisierung...............................................................12
>
> **3** **Deep** **Learning** **und** **neural**
> **Networks..............................................................................13**
>
> 3.1Neuronale
> Netzwerke....................................................................................13
> 3.2Perceptrons...................................................................................................13
> 3.3Künstliche neuronale
> Netze(KNN).................................................................14
> 3.4Aufbau neuronaler
> Netze...............................................................................14
> 3.5Aktivierungsfunktionen...................................................................................15
> 3.6Wahl der Aktivierungsfunktion
> .......................................................................15
> 3.7Modell und
> Verlustfunktion.............................................................................16
>
> **4** **Objekterkennung** **mit** **Deep** **Neural** **Networks**
> **(DNN).....................................................17**
>
> 4.1.1 Convolutional Neural Network
> (CNN).................................................................17
>
> 4.1.2
> Filter....................................................................................................................17
>
> 4.1.3
> Faltungsschicht...................................................................................................17
>
> 4.1.4 Pooling
> Layer......................................................................................................18
>
> 4.1.5 Fully-connected Layer
> ........................................................................................18
>
> 4.1.6 CNN Model
> .........................................................................................................19
>
> 4.1.7 Allgemeine Trainingsgrundsätze des
> Convnet...................................................19
>
> III

<img src="./lvzluqvy.png"
style="width:1.81861in;height:0.30625in" />

> 4.2You Only Look Once (YOLO)
> ........................................................................20
> 4.2.1 Das neuronale Netzwerk
> ....................................................................................20
>
> 4.3Yolo
> v3..........................................................................................................21
> 4.3.1
> Netzwerkstruktur.................................................................................................21
>
> 4.3.2
> Training...............................................................................................................22
>
> 4.3.3 Anchor Box
> .........................................................................................................22
>
> 4.3.4 Bounding
> Boxes..................................................................................................23
>
> 4.3.5
> IOU......................................................................................................................24
>
> 4.3.6 Non-maximum Suppression
> ...............................................................................24
>
> 4.3.7 Loss-Funktion
> .....................................................................................................25
>
> 4.3.8 Klassen
> Ermittlung..............................................................................................26
>
> 4.3.9 Klassenermiltlung
> verfahren...............................................................................27
>
> 4.3.10 Residual Block
> ..............................................................................................27
>
> 4.4Objekterkennung mit
> YOLO...........................................................................28
> 4.4.1 Geschwindigkeit / Genauigkeit
> ...........................................................................28
>
> 4.4.2
> Metriken..............................................................................................................29
>
> 4.4.3 Probleme des trainierten Netzes
> ........................................................................31
>
> 4.5Eingesetzte Computer Vision Bibliotheken
> ....................................................31 4.5.1 Hardware
> ............................................................................................................31
>
> 4.5.2 Technologie
> ........................................................................................................32
>
> 4.5.3 Eingesetzte
> Python-Bibliotheken........................................................................32
>
> **5** **Von** **der** **Gesichtserkennung** **zur**
> **Gesichtsmaskenerkennung.....................................34**
>
> 5.1Gesichtserkennung mit Deep
> Learning..........................................................34
> 5.1.1 KI-Methoden und deren Vorbereitung zum Einsatz
> ...........................................34
>
> 5.1.2 Gesicht Erkennung
> Algorithmus.........................................................................35
>
> 5.1.3 Theorie zum Gesichtserkennung mit
> OpenCV...................................................36
>
> 5.1.4
> Datensatz............................................................................................................36
>
> 5.2Die Verfahren kurz beleuchtet
> .......................................................................36
> 5.2.1
> Versuchsaufbau..................................................................................................37
>
> 5.2.2
> Ergebnisse..........................................................................................................38
>
> 5.3Aufbau einer Gesichtsmaskenerkennung mit Deep
> Learning.........................39
>
> IV

<img src="./uj4um300.png"
style="width:1.81861in;height:0.30625in" />

> 5.3.1 Der Einsatz eines vortrainierten
> Modells............................................................39
>
> 5.4MobileNetV2..................................................................................................40
> 5.4.1 Netzwerke
> Struktur.............................................................................................40
>
> 5.4.2 Objekt
> Detektion.................................................................................................41
>
> 5.4.3 Modellaufbau Gesichtsmaskenerkennung mit Python
> .......................................41
>
> 5.4.4 Datensatz
> Gesicht-Maske-Erkennung................................................................41
>
> 5.4.5 Gesichtsmaskenerkennung
> Algorithmus............................................................42
>
> 5.4.6 Aufbau des
> Modells............................................................................................42
>
> 5.4.7
> Evaluation...........................................................................................................43
>
> 5.4.8 Training Ergebnis der verwendeten
> Arbeit.........................................................45
>
> 5.5Gesichtsmasken-Erkennung mit
> YOLOv3......................................................46 5.5.1
> Verwandte
> Arbeiten............................................................................................46
>
> 5.5.2
> Modellbeschreibung............................................................................................46
>
> 5.5.3
> Datensatz............................................................................................................47
>
> 5.5.4
> Training...............................................................................................................47
>
> 5.5.5 Leistung
> ..............................................................................................................47
>
> **6** **Selbst** **modifizierter**
> **YOLO-Ansatz..................................................................................48**
>
> 6.1Bilder Vorbereitung
> Erkennungsraten............................................................48
> 6.2Training
> Yolov3..............................................................................................48
> 6.3Vorbereitung der Daten
> .................................................................................49
> 6.4Klassen für verschiedene
> Maskentypen.........................................................51
> 6.5Annotation
> Data.............................................................................................52
> 6.6Data
> Augmentation........................................................................................52
> 6.7Versuchsaufbau.............................................................................................53
> 6.8Testphase......................................................................................................53
>
> 6.9Training
> .........................................................................................................54
> 6.10 Evaluation und Diskussion der
> Ergebnisse..............................................54 6.10.1
> Evaluation
> .....................................................................................................54
>
> 6.10.2
> Ergebnisse....................................................................................................55
> 6.10.3 Diskussion und
> Ausblick...............................................................................56
> 6.10.4
> Limite.............................................................................................................56
>
> **7**
> **Fazit....................................................................................................................................57**
>
> **8** **References**
> **........................................................................................................................58**
>
> V

<img src="./1hxqm3mu.png"
style="width:1.81861in;height:0.30625in" />

> **Abbildungsverzeichnis**

||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||

> VI

<img src="./p1koafty.png"
style="width:1.81861in;height:0.30625in" />

||
||
||
||
||
||
||
||
||
||
||
||
||
||
||
||

> VII

<img src="./eejgx1ib.png"
style="width:1.81861in;height:0.30625in" />

> **Abstract**
>
> Die COVID 19-Krise stellt eine globale Krise dar. Sie betrifft alle
> Bereiche der Wirt-schaft, aber auch den Bildungssektor. Es werden
> zahlreiche Maßnahmen ergriffen, um die Ausbreitung des Covid-19 Virus
> zu verhindern. Darunter das Tragen von Masken. Dennoch ist die
> individuelle Kontrolle der Verwendung von Masken schwierig und
> problematisch, insbesondere an öffentlichen Orten. Seit der
> Ankün-digung der Maskenpflicht haben viele Experten, Studenten und
> Forscher im Bereich künstlichen Intelligenz Lösungen für die Kontrolle
> des Tragens von Masken vorge-schlagen.
>
> Diese Arbeit befasst sich mit denselben Fragen. Basierend auf den
> bereits ge-leis-teten Arbeiten der Wissenschaftler, insbesondere bei
> der Entwicklung von Techno-logien und Anwendungen zur Erkennung von
> Masken, soll in dieser Arbeit die For-schung nicht nur auf das Tragen
> von Masken, sondern auch auf die Arten von Mas-ken erweitert werden.
> In dieser Arbeit wird dargestellt, wie Deep Learning, CNNs und AI
> bereits in ähnlichen Projekten zur Gesichtserkennung eingesetzt
> wurden. Die Verwendung tiefer neuronaler Netze (Deep Neural Networks,
> DNN) in der Bild-verarbeitung hat insbesondere in der Objektdetektion
> signifikante Fortschritte er-möglicht.
>
> Ausgehend von den aktuellen DNN Architekturen soll zunächst durch
> Transfer-Learning die Verlässlichkeit der Detektion von Masken in
> Gesichtern im Allgemei-nen untersucht werden. Hierzu soll auch eine
> annotierte Bild-Datenbank aus unter-schiedlichen Quellen und
> Kameraauflösungen für den Einsatz in der Forschung er-stellt werden.
> Im weiteren Verlauf dieser Arbeit wird die Detektion schrittweise
> er-weitert und verfeinert. Insbesondere sollen Klassen für
> verschiedene Maskentypen (Alltags-Maske (OP-Maske), FFP2-Schutzmaske,
> Gesichtsschutz…) untersucht werden und die Art des Tragens
> (Mundschutz, Mund- und Nasenschutz) detektiert werden.
>
> VIII

<img src="./esyvmdrf.png"
style="width:1.81861in;height:0.30625in" />

> **1** **Einleitung**
>
> **1.1** **Ziel**
>
> In dieser Arbeit wurden die wichtigstenArchitekturen auf Basis der
> Bildverarbeitung, insbesondere in der Bilderkennung und
> Bildklassifikation untersucht. Die für diese Arbeit ausgewählten
> Architekturen werden auf Bilder von Menschen mit und ohne Maske
> angewendet und später Verarbeitungs- und Auswertungstests unterzogen.
> Ziel ist es die Leistung der Netzwerke und die Leistungsfähigkeit
> derArchitektur zu ermitteln.
>
> **1.2** **Aufbau** **der** **Arbeit**
>
> DieseArbeit ist in siebenAbschnitte unterteilt, einschließlich einer
> Einleitung. InAb-schnitt zwei werden die theoretischen Grundlagen der
> Computer Vision vorgestellt. Der erste Teil von Abschnitt drei befasst
> sich mit Deep Learning und neuronalen Netzen und der zweite Teil mit
> Methoden der tiefen neuronalen Netze und deren unterschiedlichen
> Architekturen. Der Abschnitt vier beschäftigt sich zum anfangs mit
> Objekterkennung basierend auf Deep Neural Networks. Insbesondere wird
> in diesem Abschnitt Grundwissen über CNN und der Yolo-Architektur,
> welche im Be-reich der Erkennung von Gesichtern und Gesichtsmasken
> vorgeschlagen und durchgeführt wurden, erläutert. Des Weiteren wird
> die eingesetzte Hardware und Computer Vision Bibliotheken, welche im
> Rahmen der Realisierung des Projekts verwendet werden, vorgestellt. In
> Abschnitt fünf wird die Arbeit der verschiedenen Autoren auf dem
> Gebiet der Gesichtserkennung behandelt, welche die Grundlage für die
> Methoden zur Erkennung von verschiedenen Masken Typen darstellt.
> Ab-schnitt sechs stellt die Forschung über Maskentypen und
> experimentellen Ergeb-nissen dar. Die Schlussfolgerung wird in
> Abschnitt sieben dargelegt.
>
> **1.3** **Forschungsstand**
>
> Die Convolutional Neural Networks (CNN) \[1\] , inspiriert von
> biologischen Erkennt-nissen im visuellen Cortex von Säugetieren,
> wurden bereits zur Lösung von Klassi-fikations- und
> Erkennungsproblemen eingesetzt. Basierend auf der Architektur von CNN
> haben mehrere Autoren sehr robuste und effiziente
> Klassifikationsmethoden vorgestellt. So stellte Zu, Hu et al. (Hg.)
> 2015 – in Human centered computing \[2\] die Gesichtserkennungsmethode
> basierend auf Deep Learning vor. Diese Methode legte den Grundstein
> für die Forschungen im Bereich der Maskenerkennungsver-fahren.
>
> **1.4** **Wissenschaftliche** **Ergebnisse**
>
> Die Techniken, welche im Bereich der Objekterkennung mit Hilfe von
> Computer Vi-sion eingesetzt werden, haben ihre Leistungsfähigkeit
> unter Beweis gestellt. Diese Methoden haben jedoch nicht alle die
> Genauigkeit, welche Deep-Learning-Metho-den bieten. Grundsätzlich gibt
> es zwei Methoden: Two-Stage Methoden und Single Shot MultiBox
> Detector.
>
> 9

<img src="./nkex2b1f.png"
style="width:1.81861in;height:0.30625in" /><img src="./ujv1oblv.png"
style="width:6.01319in;height:2.57014in" />

> 1.4.1 Single Shot Multi Box Detektor
>
> SSD ist ein Single-Shot-Detektor. Dieser hat kein delegiertes
> Regionsvorschlags-netzwerk und ermittelt die Bounding
> Box(Begrenzungsrahmen) und die Klassen di-rekt aus Feature Maps in
> einem einzigen Durchgang. Sie betrachten die Objekter-kennung als ein
> Regressionsproblem, welche mithilfe eines neuronalen Netzes aus den
> Pixeln desEingangsbildes,Objekte ermittelt werden.Hierbei wird
> einerkanntes Objekt durch die Bounding Box beschrieben, um die
> Position und Größe eindeutig zu bestimmen. Zur SSD-Familie gehören
> **YOLO** und RetinaNet. Single Shot Detek-tor ist schneller als
> Zwei-Schritt Detektoren, jedoch mit schlechteren Resultaten.
>
> 1.4.2 Two-stage Detektion
>
> Bei dieser Technik wird die Methode des Regionsvorschlags verwendet,
> um poten-zielle Begrenzungsrahmen in einem Bild zu erzeugen. Two-Stage
> Methoden \[3\] müssen in einem ersten Schritt sogenannte
> Region-Proposals, also Vorschläge für Bereiche in denen sich Objekte
> befinden, betrachten. Zum zweiten Schritt werden diese Regionen
> verwendetund der Inhaltals Klassifikationsproblem betrachtet. Das
> heißt die Klasse des abgebildeten Objekts ermittelt. Dies führt dazu,
> dass die Zeit, um ein Bild zu verarbeiten sehr hoch ist. Zur
> Zwei-Stufen-Objekterkennung-Familie gehören R-CNN, FPN, Mask R-CNN.
>
> Abbildung 1 : Übersichtsdiagramm des **Single-Shot-Detektors** (SSD)
> und des **Two-Shot-De-tektors** (Faster RCNN, R-FCN) in der
> Meta-Architektur.
>
> *Quelle* *:*
> *https://clear.ml/blog/the-battle-of-speed-accuracy-single-shot-vs-two-shot-detection/*
>
> 10

<img src="./s23bv5dq.png"
style="width:1.81861in;height:0.30625in" />

> **2** **Einführung** **in** **die** **Computervision**
>
> **2.1** **Computer** **Vision**
>
> ComputerVision ist eineTechnik der künstlichen Intelligenz,welche die
> Analyse von Bildern ermöglicht, welche von Geräten wie z.B. einer
> Kamera aufgenommen wur-den. Diese Technik nutzt Deep Learning, um die
> neuronalen Netzwerke zu trainie-ren, welche die Systeme bei der
> Verarbeitung und Analyse ihrer Daten anleiten. Nach vollständigem
> Training sind Computer-Vision-Modelle in der Lage, Objekte zu
> erkennen, Personen zu erfassen und zu erkennen. Sogar die Ermittlung
> von Ob-jektbewegungen kann damit realisiert werden. Die meisten
> Bildverarbeitungsan-wendungen folgen dem gleichenAblauf.AmAnfang
> werden das Bild oder die Daten erfasst. Und später werden diese Daten
> oder Bilder verarbeitet. Auch werden ver-schiedene Analyse- und
> Erkennungsschritte durchgeführt. Am Ende wird eine Vor-hersage auf der
> Basis der extrahierten Informationen erstellt \[4\].
>
> **2.2** **Anwendungen** **des** **Computer** **Vision**
>
> Die Fähigkeit von Computern Objekte in Fotos und Videos zu
> klassifizieren, wird heute von KI-Systemen übertroffen.
>
> Ziel ist es nicht, alle Anwendungen von DL aufzulisten, sondern viel
> mehr einen allgemeinen Überblick über einige ihrer Algorithmen zu
> geben. So bewährt sich DL in verschiedenen Bereichen wie zum Beispiel
> in der Robotik, bei autonomenAutos, welcheStraßenbilder
> erkennenkönnen, imKinomit MotionCapture, bei
> Gesichtser-kennungssystemen in Smartphones und in weiteren Bereichen.
> Dank des enormen Anstiegs der Rechenleistung und der Menge an
> verfügbaren Daten, haben KI und DL in vielen komplexen Bereichen der
> visuellen Wahrnehmung außergewöhnliche Leistungen erzielt.
>
> **2.3** **Bildklassifizierung**
>
> Die Vorhersage der Klasse, zu der ein Objekt in einem Bild gehört,
> wird als Klassi-fizierung bezeichnet. Die Bildklassifikation ist oft
> ein überwachtes Lernproblem. Hierbei wird eine Menge von Objekten
> definiert, welche in Bildern identifiziert wer-den sollen und mit
> Hilfe von gelabelten Beispielen ein Modell zur Erkennung dieser
> Objektetrainiert. Es werden,umObjektezuerkennenundzuklassifizieren,
> mehrere wichtige Parameter berücksichtigt. So können z. B. die
> Umgebungsbeleuchtung, die Position des Objekts, der Hintergrund hinter
> dem Objekt, der Kamerawinkel und der Fokus Schwankungen in den
> Pixel-Rohdaten erzeugen. Die Korrektur dieser großen Unterschiede
> durch die Bildung der gewichteten Mittelwerte der RGB (Rot, Grün und
> Blau) Werte der Pixel, kann sehr aufwendig sein.
>
> 11

<img src="./vbeyssf4.png"
style="width:1.81861in;height:0.30625in" />

> **2.4** **Objekterkennung** **und** **Lokalisierung**
>
> Nachdem die Klasse des Objekts vorhergesagt wurde, sollte dessen
> Position im Bild bestimmt und einen Rahmen, um seine Ausdehnung zu
> ziehen. Dies wird als Lokalisierung bezeichnet.
>
> Bei der Objekterkennung handelt es sich um eine Methode zur
> Feststellung des Vorhandenseins einer Instanz (Objekterkennung) oder
> einer Klasse von Objekten in einem digitalen Bild. Mit dieser Technik
> lassen sich Orte, Personen, Objekte und viele andere Elemente in einem
> Bild identifizieren und durch Analyse Schlussfolge-rungen ziehen.
>
> Es gibt so verschiedene Aufgaben, welche die Bilderkennung erfüllen
> kann:
>
> • **Einstufung.**
>
> Dies ist die Identifizierung der Klasse oder Kategorie, zu der ein
> Bild gehört. Ein Bild kann nur eine Klasse haben.
>
> • **Beschriftung**
>
> Diese Aufgabe wird auch als Labelling bezeichnet und ist eine
> Klassifizie-rungsaufgabe, allerdings mit einem höheren
> Genauigkeitsgrad. Es erkennt das Vorhandensein mehrerer Begriffe oder
> Objekte in einem Bild.
>
> • **Erkennung**
>
> • Dies ist notwendig, wenn Sie ein Objekt in einem Bild lokalisieren
> möchten. Sobald die Lokalisierung erfolgreich war, wird ein Rechteck(
> die so genannte Bounding Box), um das betreffende Objekt gelegt.
>
> • **Segmentierung**
>
> Die Segmentierung ist ein Vorgang, welcher für jedes einzelne Pixel
> eine Entscheidung trifft, ob es zu einem Objekt gehört oder nicht. Die
> Segmentie-rung kann ein Element in einem Bild bis zum nächstgelegenen
> Pixel lokali-sieren.
>
> 12

<img src="./41o4riyr.png"
style="width:1.81861in;height:0.30625in" />

> **3** **Deep** **Learning** **und** **neural** **Networks**
>
> **3.1** **Neuronale** **Netzwerke**
>
> Ein Neuronales Netzwerk ist ein Computersystem, welches von der
> Funktionsweise des menschlichen Gehirns zum Lernen inspiriert wurde.
> Es handelt sich dabei um eine Art von Deep Learning-Technologie \[5\],
> welche Teil der Unterkategorie des maschinellen Lernens der
> künstlichen Intelligenz ist. Maschinelles Lernen ist eine Methode der
> Datenanalyse, welche die Erstellung von Analysemodellen
> automati-siert. Durch den Einsatz von Algorithmen, welche iterativ aus
> Daten lernen, können Computer mitHilfedes
> maschinellenLernensversteckte Informationenfinden,ohne dass sie
> explizit programmieren müssen, wo sie zu suchen sind. In einem
> Wettbe-werb, welcher von ImageNet \[6\] organisiert wurde, ist es
> einem Neuronalen Netz-werk im Jahr 2012 zum ersten Mal für eine
> Bilderkennung gelungen, den Menschen zu übertreffen. Daher steht diese
> Technologie wieder im Mittelpunkt des Interesses der Wissenschaftler,
> insbesondere bei der Erkennung und Klassifizierung von Ob-jekten.
> Schematisch kann das Neuron in drei große Einheiten aufgeteilt werden:
> Erstens einem Zellkörper, zweitens eine Reihe von Dendriten, und
> schließlich ein Axon.

<img src="./o4yetbbu.png"
style="width:5.94333in;height:0.39333in" /><img src="./dqahisqj.png"
style="width:5.96458in;height:2.06125in" />*Abbildung* *2* *:* *Links:*
*Nervenzelle* *(Neuron),* *rechts:* *künstliches* *Neuron*
*(Perzeptron).* *Quelle:* *Nina* *Schaa*

> **3.2** **Perceptrons**
>
> Ein Perceptron, auch künstlichesNeurongenannt,
> isteinneuronalesNetzwerk, wel-ches bestimmte Berechnungen durchführt,
> um Merkmale zu erkennen. Hierbei han-delt es sich um ein
> einschichtiges neuronales Netzwerk, das als linearer Klassifika-tor
> bei der Verarbeitung eines Eingangsdatensatzes verwendet wird. Es
> funktioniert ähnlich wie ein biologisches Neuron (Abbildung 2). Es
> gibt zwei Arten von Percept-rons:
>
> 1\. **Einschichtige** **Perceptrons**
>
> Einschichtige Perceptrons können nur linear separierbare Modelle
> lernen.
>
> 2\. **Mehrschichtige** **Perceptrons**
>
> 13

<img src="./5jwv01e0.png"
style="width:1.81861in;height:0.30625in" /><img src="./xwmyhgus.png" style="width:5.85417in;height:2.3in" />

> Multilayer-Perceptrons(mehrschichtige Perceptrons) mit zwei oder mehr
> Schichten, haben eine höhere Rechenleistung. Daher wird jedem
> Eingangsknoten ein Ge-wichtswert, auch als Verbindungsgewicht
> bezeichnet, zugewiesen, welcher seine Wichtigkeit darstellt.
>
> **3.3** **Künstliche** **neuronale** **Netze(KNN)**
>
> Das künstliche neuronale Netz (KNNs) stellt bestimmte Fähigkeiten des
> Gehirns nach. Beispielsweise die Modellerkennung oder die Fähigkeit,
> Entscheidungen und Fehler im Zusammenhang mit Daten zu visualisieren.
> Sie werden häufig zur Lösung von Problemen der Klassifizierung,
> Vorhersage, Kategorisierung, Optimierung, Mustererkennung eingesetzt.
>
> **3.4** **Aufbau** **neuronaler** **Netze**
>
> Ein neuronales Netz hat mindestens eine Eingangsschicht (Input Layer)
> und eine Ausgangsschicht (Output Layer). Dazwischen gibt es
> theoretisch eine oder unbe-grenzte Anzahl von sogenannten versteckten
> Schichten. Ein Neuron mit vielen ver-schreckten Schicht wird Deep
> neurale Network genannt. Die Komplexität eines Net-zes, seine Tiefe
> und die benötigte Rechenleistung sind umso höher, je mehr ver-steckte
> Schichten es hat.
>
> Abbildung 3: Simple und Deep Learning Neural Network. \[Vázquez,
> 2017\]
>
> 14

<img src="./wv3bfegp.png"
style="width:1.81861in;height:0.30625in" /><img src="./zjiyftpy.png"
style="width:4.87847in;height:2.18417in" />

> **3.5** **Aktivierungsfunktionen**
>
> Das Perceptron sollte nur für signifikante Daten aktiviert werden. Zu
> diesem Zweck muss eine Aktivierungsfunktion angegeben werden.
> Aktivierungsfunktionen führen Nichtlinearität in neuronale Netze ein,
> welche zur Lösung komplexer Probleme not-wendig ist. Sie wird
> verwendet, um das Aktivitätsniveau der Neuronen zu berech-nen. Dazu
> werden die Gewichte und der Schwellenwert addiert. Der Zweck dieser
> Funktion ist die Aktivierung der Neuronen. Sie entscheidet, ob ein
> Neuron aktiviert werden soll oder nicht, indem sie die gewichtete
> Summe berechnet, und ein Bias hinzufügt. Als Aktivierungsfunktion wird
> häufig die Sigmoidfunktion oder ReLU-Funktion verwendet, welche in
> letzter Zeit an Popularität gewonnen hat.
>
> <img src="./55taugi1.png" style="width:4.37in;height:0.42833in" />Abbildung
> 4 Aktivierungsfunktionen
>
> **3.6** **Wahl** **der** **Aktivierungsfunktion**
>
> Welche Aktivierungsfunktion sollte für ein Projekt gewählt werden, da
> es mehrere gibt? Im Prinzip lassen sich die Funktionen testen, um zu
> sehen, was sie leisten. Man kann zum Beispiel mit **ReLu** oder
> **Soft** **Max** beginnen \[7\]. Führt eine dieser Methoden nicht zu
> einem guten Ergebnis, wird eine andere verwendet und so wei-ter. Esist
> bekannt, dass Sigmoidfunktionen und ihre Kombinationen im Allgemeinen
> am besten für Klassifikatoren geeignet sind.
>
> 15

<img src="./fj2zat50.png"
style="width:1.81861in;height:0.30625in" /><img src="./lclurdg5.png"
style="width:6.23333in;height:2.525in" />

> **3.7** **Modell** **und** **Verlustfunktion**
>
> Die Verlustfunktion wird als Maß für die Genauigkeit verwendet, um
> festzustellen, ob das neuronale Netzwerk die Modelle anhand der
> Trainingsdaten richtig gelernt hat oder nicht. Dabei wird die
> Differenz zwischen den vom neuronalen Netzwerk erzeugten Vorhersagen
> und den beim Training verwendeten tatsächlichen Be-obachtungswerten
> ausgewertet. Die Leistung des neuronalen Netzwerks ist umso besser, je
> mehr das Ergebnis dieser Funktion minimiert wird.
>
> **Abbildung** **5:** Verlustkurven mit verbesserter Segmentierung über
> Epochen
>
> *Quelle* *:*
> *https://ichi.pro/de/verlustfunktionen-fur-computer-vision-modelle-153173389506159*
>
> 16

<img src="./c1rzir3e.png"
style="width:1.81861in;height:0.30625in" /><img src="./gaawfkio.png"
style="width:3.65833in;height:1.91111in" />

> **4** **Objekterkennung** **mit** **Deep** **Neural** **Networks**
> **(DNN)**
>
> 4.1.1 Convolutional Neural Network (CNN)
>
> Ein Convolutional Neural Network (CNN, oder ConvNet) ist eine
> spezielle Art von mehrschichtigen neuronalen Netzen, welche entwickelt
> wurden, um visuelle Pat-terns direkt aus Pixelbildern mit minimaler
> Vorverarbeitung zu erkennen . Er ist die wichtigste Schicht im CNN und
> spielt in der Geschichte der Bilderkennung und -klassifizierung eine
> größere Rolle.
>
> 4.1.2 Filter
>
> In der Praxis werden die Filter eines neuronalen Faltungsnetzes mit
> einem Kernel, Stride und Padding im Voraus definiert. Dabei werden
> ihre Werte bei der Initialisie-rung zufällig erzeugt. Dann, wenn das
> Netzwerk lernt, werden die Werte der Filter aktualisiert, um die
> Ergebnisse des CNN zu optimieren: die Werte der Filter sind also Teil
> der Variablen (Gewichte, Bias...), die das Netzwerk während des
> Lernens ändert .

Abbildung 6: Faltung eines 5x5x1-Bildes mit einem 3x3x1-Kernel, um ein
3x3x1-gefaltetes Merkmal zu erhalten.

> 4.1.3 Faltungsschicht
>
> Die Faltung ist ein einfaches mathematisches Werkzeug, das in der
> Bildverarbei-tung weit verbreitet ist, was erklärt, warum sich
> neuronale Netze mit Faltung beson-ders gut für die Bilderkennung
> eignen. Die Faltung wirkt wie ein Filter. Hierbei wird eine
> Fenstergröße definiert, die sich über das gesamte Bild bewegt. Zu
> Beginn der Faltung wird das Filterfenster ganz oben links im Bild
> positioniert und bewegt sich dann eine bestimmte Anzahl von Feldern
> nach rechts(Abbindung 5). Und wenn er das letzte Ende des Bildes
> erreicht, bewegt er sich eine Stufe nach unten und so weiter, bis der
> Filter das gesamte Bild abgedeckt hat. Das Ziel ist es, bei jedem
> Vorgang die Werte zu verwenden, welche im Filter vorhanden sind. Wenn
> man z. B. ein 3 x 3-Fenster definiert, entspricht dies 9 Zellen des
> Arrays (d. h. 9 Pixel). Die Faltung führt eine Operation mit den neun
> Pixeln durch. Die Faltungsfilterung wird auf ein Graustufenbild
> angewendet. Farbbilder setzen sich aus drei Schichten zu-sammen, z. B.
> Rot, Grün und Blau. Jede Ebene kann als Graustufenbild betrachtet
>
> 17

<img src="./fex5kvy0.png"
style="width:1.81861in;height:0.30625in" /><img src="./jzkidfvx.png"
style="width:3.74167in;height:1.59028in" />

> werden. Daher muss jede Ebene separat verarbeitet werden, um ein
> Farbbild zu filtern \[8\].
>
> 4.1.4 Pooling Layer
>
> Die Pooling-Operation besteht darin, die Größe der Eingabematrix zu
> reduzieren, ohne dass viele Funktionen verloren gehen. Andernfalls
> wäre die Anzahl der Para-meter sehr hoch und damit auch die
> Berechnungszeit.
>
> **4.1.4.1** **Max** **Pooling**
>
> Der Maximum Pooling berechnet den Maximalwert für jede Fläche in der
> Feature-Map. Es ist am häufigsten eingesetzt, weil er schnell zu
> berechnen ist.
>
> **4.1.4.2** **Avarage** **Pooling**
>
> Die Average Pooling berechnet den Durchschnittswert für jede Fläche im
> Kennfeld. Es wird die Summe aller Werte berechnet und durch die Anzahl
> der Werte dividiert. Auf diese Weise erhält man einen Mittelwert,
> welcher diese Gruppe von Pixeln re-präsentiert.
>
> Abbildung 7 : Pooling Layer
>
> 4.1.5 Fully-connected Layer
>
> ● Beim Fully Connected Layer oder **Dense** **Layer** handelt es sich
> um eine nor-male neuronale Netzstruktur, welcher alle Neuronen mit
> allen Inputs und al-len Outputs verbunden sind.
>
> ● In einem **regulären** **neuronalen** **Netzwerk** wird die Eingabe
> durch eine Reihe von **versteckten** **Schichten** mit mehreren
> Neuronen transformiert.
>
> ● Jedes Neuron ist mit allen Neuronen in der vorherigen und der
> folgenden Schicht verbunden. Diese Anordnung wird als **vollständig**
> **verbundene** **Schicht** **bezeichnet** und ist hier die letzte
> Schicht der Ausgabeschicht.
>
> 18

<img src="./z0nat0ul.png"
style="width:1.81861in;height:0.30625in" /><img src="./odnxls1w.png"
style="width:4.51861in;height:1.45194in" />

> 4.1.6 CNN Model
>
> CNN-Netzwerk besteht aus einer Eingabeschicht, mehreren versteckten
> Schichten und einer Ausgabeschicht. Es handelt sich um eine tiefe
> Faltungsschicht, weil sie aus mehreren Faltungsschichten besteht, und
> deren Aufgabe es ist, die wichtigen Merkmale nach einem Training zu
> extrahieren. Aus diesen Merkmalen, welche durch das CNN-Netzwerk
> extrahiert werden, wird eine Bildklassifizierung vorge-nommen
>
> Abbildung 8 Network Architecture.
>
> <img src="./d5dqi4wh.png"
> style="width:4.17833in;height:0.43833in" />Quelle :
> https://www.scitepress.org/Papers/2021/104831/104831.pdf
>
> 4.1.7 Allgemeine Trainingsgrundsätze des Convnet
>
> Beim Training des CNN-Netzes werden die Koeffizienten ausgehend von
> einer zu-fälligen Initialisierung optimiert. Dies zielt darauf ab, den
> Klassifikationsfehler des Ausgangs zu minimieren. Es wird die
> Koeffizienten des Faltungs-Kernels gelernt, um relevante Merkmale zu
> extrahieren. Mit der Methode des sogenannten Gradi-enten Abstiegs
> \[9\] können die Koeffizienten des Netzes verändert werden, um die
> aufgetretenen Klassifikationsfehler zu korrigieren. Diese Gradienten
> werden im Netz von der Ausgabeschicht aus backpropagiert, daher der
> Name Backpropaga-tion. Neben der Backpropagation gibt es auch eine
> schnellere Methode. Dies ist die Batch-Trainingsmethode. Diese besteht
> darin, den Klassifizierungsfehler durch Gruppen von Bildern
> backpropagieren zu lassen. Sie ist deutlich stabiler als das Verfahren
> von Bild zu Bild, da die Fehlergradienten eine geringere Varianz
> aufwei-sen. Leider kann die Verwendung zu vieler Bilder pro Batch zu
> Speicherproblemen bei der Ausführung des Codes führen \[10\].
>
> 19

<img src="./tmt2jove.png"
style="width:1.81861in;height:0.30625in" /><img src="./erhyezk2.png"
style="width:5.90417in;height:2.28194in" />

> **4.2** **You** **Only** **Look** **Once** **(YOLO)**
>
> YOLO (You Only Look Once) ist ein weit verbreitetes Object-Detection
> Verfahren \[11\], welche im Jahr 2015 von Redmon et al. \[12\]
> veröffentlicht und seitdem in meh-reren Schritten weiterentwickelt
> wurde. Yolo betrachtet die Objekterkennung als ein Regressionsproblem,
> bei dem mithilfe eines neuronalen Netzes aus den Pixeln des
> Eingangsbildes Objekte ermittelt werden. Es ist schneller als 2-stage
> detector Algo-rithmen. Was also ihren Algorithmus betrifft, so müssen
> in dieser Arbeit nicht meh-rere Komponenten neu trainiert werden. Es
> gibt keine Notwendigkeit für eine Sup-port-Vektor-Maschine oder ein
> zugrunde liegendes lineares Regressionsmodell.
>
> 4.2.1 Das neuronale Netzwerk
>
> Yolo v1ist das Basismodell. Dies hat 24Faltungsschichten,
> gefolgtvon2vollständig verbundenen Schichten. Es werden 1 x 1
> Reduktionsschichten verwendet, gefolgt von einer 3 x 3
> Faltungsschicht. Diese verfügt über 24 Faltungsschichten, darunter 4
> Max-Pooling-Schichten und zwei voll verbundene Schichten. Eine mit
> 4096 Neu-ronen und die andere mit 1470 Neuronen. Dieses Modell nimmt
> zur Objekterken-nung Farbbilder der Größe 448 x 448. Die Autoren
> verwendeten die PASCAL VOC-Datensätze 2007 und 2012 \[13\], um ein
> Objekterkennungsmodell zu erstellen und zu trainieren. Wie in
> Abbildung 9 unten zu sehen ist, wird als Aktivierungsfunktion die
> Leaky Rectified Linear Unit (Leaky ReLU) verwendet. Dies ist im
> Schaubild nach jeder Faltungsschicht und in der ersten FC-Schicht zu
> sehen.
>
> Abbildung 9: YOLOv1 Network Architecture
>
> 20

<img src="./z5dds3kh.png"
style="width:1.81861in;height:0.30625in" /><img src="./eh2vqbl5.png"
style="width:3.81125in;height:3.84861in" />

> **4.3** **Yolo** **v3**
>
> Die verschiedenen Tests, welche von mehreren Autoren durchgeführt
> wurden, zei-gen, dass Yolo v3 in einem weiten Bereich der
> Bildauflösung gut abschneidet. Bei einer Eingabeauflösung von 608 x
> 608 im COCO-Validierungsset 2017 erreichte Yolo v3 einen Wert von 37
> mAP. Im Vergleich zu anderen Architekturen wie dem Faster-RCNN-
> ResNet50 ist er weit voraus. Nur die Mobilenet ,SSD-Architektur
> er-reichen einen mAP von 30. Die neuen Versionen Yolo v4 und V5 zeigen
> ebenfalls eine große Leistung im Vergleich zu Yolo v3.
>
> 4.3.1 Netzwerkstruktur
>
> Darknet-53 ist die Basis von YOLOv3,welches ein Eingangsbild nimmt und
> dieFea-ture-Map extrahiert. YOLOv3 verwendet die Netzstruktur
> Darknet53 und enthält 53 Faltungsschichten. In jedem dieser Schichten
> sind Faltungsfunktionen wie Batch-Normalisierung und
> Leaky-Relu-Aktivierungsfunktionen enthalten. Darknet53 setzt sich aus
> fünf Residualblöcken zusammen, welche von der Architektur des
> neurona-len Netzwerks Resnet \[14\] inspiriert sind. Durch die
> Verwendung einer Residualein-heit soll die Tiefe des Netzwerks erhöht
> werden, um den Verlustgradienten zu ver-meiden. Es kann auch
> festgestellt werden, dass eine Faltungsschicht mit Stride (2)
> verwendet wird, um die Feature Map zu reduzieren. Zum anderen kann man
> bei Yolov3 das Fehlen von Pooling-Schichten feststellen.
>
> <img src="./ote0z0vo.png"
> style="width:3.97833in;height:0.41667in" />*Abbildung* *10* *YOLO-V3*
> *Architecture*
>
> 21

<img src="./upc3s50w.png"
style="width:1.81861in;height:0.30625in" /><img src="./o3tmrhyq.png"
style="width:2.84167in;height:2.175in" />

> 4.3.2 Training
>
> Bei YOLOv3 werden schrittweise 3 × 3 und 1 × 1 Faltungsschichten
> verwendet. Die Detektion erfolgt durch die Anwendung von
> Detektions-Kerneln auf Feature-Maps von drei verschiedenen Größen an
> drei verschiedenen Stellen im Netzwerk. Die Form des Erkennungskerns
> wird wie folgt dargestellt: 1 × 1 × (B × (5 + C)). Wobei B die Anzahl
> der Bounding Boxes ist, welche eine Zelle in der Feature-Map
> vorher-sagen kann. Die Zahl 5 steht für die 4 Bounding-Box-Attribute
> und das Vertrauen eines Objekts. Das C steht für die Anzahl der
> Klassen. Yolov3 verwendet die Me-thode der mehrschichtigen Detektion.
> Diese Methode versucht, das Problem der Detektion kleiner Objekte zu
> beheben. Diese Methode ermöglicht es, ein vortrai-niertes Modell in
> einem ähnlichen Projekt zu verwenden, so dass das Lernen schneller
> erfolgen kann. Die Bilder sind in ein Gitter von Zellen (13×13, 26×26
> und 52×52) unterteilt. Für die Detektionsaufgabe wurde ein zweites
> Netzwerk mit 53 Schichten hinzugefügt, welches der ersten bis auf die
> letzten Schichten ähnlich ist, um so eine vollständig faltige
> Architektur mit 106 Schichten zu ergeben. Dies ist das Prinzip des
> Transferlernens \[15\]. Wenn das Modell gelernt wird, werden die
> Ge-wichte dieses zweiten Netzes an die Daten des Trainingssatzes
> angepasst. Dies ist nicht der Fall für die Gewichte des ersten
> Netzwerks, die festgelegt werden \[16\].
>
> 4.3.3 Anchor Box
>
> Ankerboxensindein Paar vordefinierter Bounding boxenmit einer
> bestimmtenHöhe und Breite. Für jede Gitterzelle kann **ein**
> **einzelnes** **Objekt** erkannt werden. Aber es kann einige Probleme
> mit diesem Ansatz geben, wenn sich mehrere Objekte in ei-nem Raster
> befinden. Daraus folgt in diesemFall, dass, die Mittelpunkte **(x,y)**
> beider Objekte in der gleichen Rasterzelle liegen. Aus diesem Grund
> werden die Formen der Ankerboxen vorgegeben: Es wird davon
> ausgegangen, dass die erkannten Ob-jekte (mit hoher
> Wahrscheinlichkeit) unterschiedliche Formen haben.
>
> Abbildung 11:Ankerboxen für die Objekterkennung
>
> 22

<img src="./hmz23lni.png"
style="width:1.81861in;height:0.30625in" />

> 4.3.4 Bounding Boxes
>
> In Yolov3 verwenden die Autoren den Begriff Bounding Box für die Box,
> die durch einen Anchor definiert wird. Die Objekte, welche erkannt
> werden sollen, sollten ide-alerweise einen Objektivitätswert von 1
> haben. Bei dieser Methode kann nur eine Bounding Box pro Objekt der
> Grundwahrheit berücksichtigt werden. Für die Berech-nung des Verlustes
> werden die Werte der Vorhersage (tx,ty) verwendet.
>
> <img src="./hugfslmc.png"
> style="width:2.7825in;height:2.40889in" />bx = σ (tx) + cx
>
> by = σ (ty) + cy
>
> bw = pwetw
>
> bh = pheth
>
> Pr (ob ject) × IoU (b, ob ject) = σ (to)
>
> <img src="./pgmkmnbe.png" style="width:3.18167in;height:0.44in" />Abbildung
> 12: Bounding boxes with dimension priors and location
>
> **Mit**
>
> *bx,by* = Koordinaten der Bounding Box, die das erkannte Objekt
> beinhaltet
>
> *cx,cy* = Koordinaten der Rasterzelle, zu der die Box gehört
>
> *pw,ph* = Breite und Höhe der Anchor Box (aus k-Means)
>
> *bw,bh* = Breite und Höhe der Bounding Box, die das erkannte Objekt
> beinhaltet
>
> *σ*(*to*)=Confidence Score der Box.
>
> 23

<img src="./5gycmypx.png"
style="width:1.81861in;height:0.30625in" /><img src="./gfm315zm.png"
style="width:3.1743in;height:1.99083in" /><img src="./gaxthfgf.png"
style="width:2.15722in;height:2.16875in" /><img src="./aoupjr0x.png"
style="width:5.86722in;height:1.91875in" />

> 4.3.5 IOU
>
> Interzeption over Union ist eine Bewertungsmetrik, welche die
> Genauigkeit eines Objektdetektors auf einem bestimmten Datensatz
> misst.
>
> Abbildung 13: Verständnis der Konzepte Intersection Over Union
>
> 4.3.6 Non-maximum Suppression
>
> Eines der häufigsten Probleme von Objekterkennungsalgorithmen ist,
> dass sie die Tendenz haben, ein Objekt mehrfach zu erkennen. Der
> Yolo-Algorithmus gibt viele Boxen aus, welchen die meisten irrelevant
> / redundant sind. Zu diesem Zweck wird eine Technik eingesetzt, um
> nicht benötigte Boxen herauszufiltern und zu verwer-fen. Non-maximum
> Suppression Funktion ist diese Technik und ist für die Löschung
> unnötiger Bounding Boxes verantwortlich.
>
> Abbildung 14: Verständnis der Konzepte Non-maximum Suppression
>
> 24

<img src="./rrjpifhl.png"
style="width:1.81861in;height:0.30625in" /><img src="./og3ratcl.png"
style="width:2.88889in;height:0.70555in" /><img src="./pe4tiyb1.png"
style="width:3.53542in;height:0.55764in" /><img src="./ck4n2hxm.png"
style="width:3.74097in;height:2.26597in" />

> 4.3.7 Loss-Funktion
>
> Wie bereits erwähnt, sagt Yolo mehrere Bounding box pro Rasterzelle
> voraus. Jede räumliche Zelle in den Ausgabeschichten des Gitters sagt
> mehrere Boxen voraus. Um den Verlust des wahren Positivs zu berechnen,
> ist es daher von Vorteil, dass nur einer von ihnen für das Objekt
> verantwortlich ist. Das Objekt mit dem höchsten IoU wird ausgewählt.
> Zur Berechnung des Verlusts verwendet Yolo die Summe der quadratischen
> Fehler zwischen den Vorhersagen und der Grundwahrheit \[17\].
>
> Quelle:
> https://ichi.pro/de/echtzeit-objekterkennung-mit-yolo-yolov2-und-jetzt-yolov3-44743782178952
>
> Die Verlustfunktion von YOLO v3 lässt sich wie folgt zusammenfassen:

• **Box** **Koordinaten**

> Diese Gleichung(Box Koordinaten) berechnet den Verlust im Verhältnis
> zur vorher-gesagten Position der Bonding Box (x, y). Die Funktion
> berechnet die Summe über jeden Bounding Box Prädiktor und ist wie
> folgt definiert:
>
> Die Summe dieser Funktion ergibt **1,** wenn ein Objekt in der
> Gitterzelle *i*vorhanden ist und der *j-te* Bounding-Box-Prädiktor für
> diese Vorhersage verantwortlich. Sonst ist er 0.
>
> Die (x, y) sind die vorhergesagte Position des Begrenzungsrahmens und
> (x, ŷ) sind die tatsächliche Position aus den Trainingsdaten.
>
> • **Box-Seitenverhältnis**
>
> Für die Größenabweichungsstrafe wird wie folgt berechnet:
>
> Dies ist der Verlust bezogen auf die vorhergesagte Breite / Höhe der
> Box.
>
> 25

<img src="./e2i01e5t.png"
style="width:1.81861in;height:0.30625in" /><img src="./vvpn2oty.png"
style="width:2.89305in;height:0.48264in" />

> •**Confidence** **loss** (**Objektfehler)**
>
> <img src="./mk51mwrt.png"
> style="width:2.30694in;height:1.05903in" />Wenn ein Objekt erkannt
> wurde und diese Box auch für das Objekt verantwortlich war. Die Box
> wäre auch für das Objekt zuständig: Hier wird der Verlust berechnet,
> welcher mit dem Konfidenzwert für jeden Prädiktor in der Bounding Box
> verbunden ist. C ist der Konfidenzwert und Ĉ ist die Schnittmenge auf
>
> der Union der vorhergesagten Bounding Box mit der Ground Truth. 𝟙 obj
> ist gleich eins, wenn sich ein Objekt in der Zelle befindet, und sonst
> gleich 0. 𝟙 noobj ist das Gegenteil.
>
> • **Der** **Klassifizierungsfehler**
>
> Hier, wenn ein Objekt erkannt wird, ist der Klassifikationsverlust in
> jeder Zelle der quadratische Fehler der klassenbezogenen
> Wahrscheinlichkeiten für jede Klasse.
>
> Für die Klassifizierungsdaten wird für alle Klassendaten in jeder
> Bounding Box wie folgt berechnet:
>
> 𝟏𝑶𝒃𝒋=1 ,wenn in Zelle *i* ein Objekt vorkommt, sonst 0
>
> 𝑷𝒊(𝑪) bezeichnet die bedingte Kalsswahrscheinlichkeit für die Klasse c
> in Zelle *i*.
>
> Was bedeutet die Parameter **λ** **?** Die Parameter **λ** werden
> verwendet, um die Teile der Verlustfunktionen unterschiedlich zu
> bewerten. Dies ist die Voraussetzung, um die Modellstabilität zu
> verbessern. Die höchste Konventionalstrafe gilt für die
> Koor-dinatenvorhersagen ( λ coord = 5) und die niedrigste für die
> Vorhersagen ohne Ob-jekt Konfidenz ( λ noobj = 0,5).
>
> 4.3.8 Klassen Ermittlung
>
> Die Bounding Boxen mit den Klassen vorhersagen werden ermittelt. Eine
> Bounding Box wird durch Koordinaten **(x,y,w,h)** und einem
> **Confidence-Score** beschrieben.
>
> ▪**x,y** Koordinaten beschreiben das Zentrum der Bounding Box als
> relativen Offset zu der Zelle, zu der sie gehören.
>
> ▪ **w,h** Koordinaten beschreiben die Höhe und Breite der Box relativ
> zum gesam-ten Bild. Mit den Bounding Boxes können somit Position und
> Größe von Objek-ten auf Bildern definiert werden.
>
> **Der** **Confidence** **Score** : beschreibt, ob die jeweilige
> Bounding Box ein Objekt be-inhaltet und wie gut sie sich mit diesem
> Objekt deckt.
>
> **Pr(Object)** ist der Objectness-Score, der bestimmt, wie
> wahrscheinlich es ist, dass die Box ein Objekt beinhaltet. *Pr*
> *(Classi\|Object)\*Pr(Object)\*IOU* *=* *Pr(Classi)\*IOU*
>
> Mit den Bounding Boxes können somit Position und Größe von Objekten
> auf Bildern definiert werden.
>
> 26

<img src="./nmrp3edq.png"
style="width:1.81861in;height:0.30625in" />

> 4.3.9 Klassenermiltlung verfahren
>
> Mit den Bounding Boxes können somit Position und Größe von Objekten
> auf Bildern definiert werden. Der Ausgang PCs ist entweder 0 oder 1,
> je nachdem, ob sich ein Objekt in dieser Rasterzelle befindet oder
> nicht.
>
> Die Koordinaten *bx,by,bh,bw* sind festgelegt, um Objekts zu
> bestimmen(Abbindung 15). Die C1,C2 sind Bezeichnungen für die Klassen
> Person mit Maske, und No-Mask.
>
> <img src="./itkmdv5y.png"
> style="width:4.25542in;height:2.73764in" />In der nachstehenden
> Abbildung sind die fol-genden Prozesse zu sehen. Die erste
> Git-terzelle unten links enthält kein zu erken-nendem Objekt. Der
> Beschriftungsvektor y für diese Gitterzelle hat daher pc= 0. Die-ser
> Vorgang wird in je-der Gitterzelle wieder-holt, welche keine Ob-jekte
> von Interesse
>
> <img src="./u0nmgg2z.png" style="width:4.25833in;height:0.42in" />enthält,
> welche er-*Abbildung* *15:Klassenermiltlung* *verfahren* kannt werden
> sollen.
>
> Für die oberste Zelle (hier links grün eingekreist) wird die
> y-Etikette jedoch einen anderen Wert haben. Sie enthält ein
> notwendiges Element, welches erkannt werden muss (hier das Ge-sicht).
> Dies bedeutet, dass pc den Wert eins hat (PC = 1). Es folgen die
> Zeichen *bx,by,bh,bw*, welche die Position des Begrenzungsrahmens
> angeben. C1 und C2 sind die beiden definierten Klassen. Hier zum
> Beispiel wird c1 gleich Null sein, wenn das gesuchte Objekt oder
> Element in der Zelle kein Gesicht mit einer Maske ist. Das c2 wird
> gleich eins sein (c2= 1). Dabei wird das gesuchte Element gefunden,
> hier ein Gesicht mit Maske.

4.3.10 Residual Block

> Darknet-53 verwendet eine Art von Block, den so genannten Restblock.
> Tiefe neu-ronale Netze sind schwer zu trainieren. Mit zunehmender
> Tiefe des Netzes, wird auch die Genauigkeit des Netzes gesättigt. Dies
> führt zu einem höheren Trainings-fehler. Der Zweck des Restblocks
> besteht darin, diesem Problem zubeseitigen. Von einem Restblock
> spricht man, wenn die Aktivierung einer Schicht schnell auf eine
> tiefere Schicht des neuronalen Netzes übertragen wird.
>
> 27

<img src="./5s5f4msn.png"
style="width:1.81861in;height:0.30625in" />

> **4.4** **Objekterkennung** **mit** **YOLO**
>
> YOLO-Algorithmus teilt das Eingangsbild in ein SxS-Gitter auf .Wenn
> der Mittel-punkt eines Objekts auf das Raster fällt, dann ist das
> Raster für die Vorhersage des Objekts zuständig. Entscheidend ist
> also, dass man das Eingabebild erst einmal in mehrere Zellen aufteilen
> müssen.
>
> <img src="./rbz4uihf.png"
> style="width:5.26042in;height:3.21167in" /><img src="./pccd4y5m.png" style="width:4.63in;height:0.39167in" />Abbildung
> 16 Yolo Detektion und Klassifikation
>
> 4.4.1 Geschwindigkeit / Genauigkeit
>
> Auf der Webseite YOLO: Real-Time Object Detection von pjreddie.com
> steht diese Aussage: „*YOLOv3* *is* *extremely* *fast* *and*
> *accurate.* *In* *mAP* *measured* *at* *.5* *IOU* *YOLOv3* *is* *on*
> *par* *with* *Focal* *Loss* *but* *about* *4x* *faster.* *Moreover,*
> *you* *can* *easily* *tradeoff* *between* *speed* *and* *accuracy*
> *simply* *by* *changing* *the* *size* *of* *the* *model,* *no*
> *retraining* *required!* “ YOLOv3-ist einer der effizientesten
> Algorithmen zur Objekter-kennung. Bei der Recherche zu Yolo zeigt
> sich, dass die meisten Autoren die Ver-sion 3 verwendet haben, um
> Bilderkennungsmodell aufzubauen. Die folgende Gra-fik zeigt den
> Kompromiss zwischen Vorhersageleistung und
> Algorithmus-Ausfüh-rungszeit. Anhand des Kompromisses zwischen
> Geschwindigkeit und Genauigkeit auf der mAP bei einer 0,5 IOU-Metrik
> stellt man fest, dass YOLOv3 gut ist, weil es sehr hoch und weit links
> liegt (Abbindung 17).
>
> 28

<img src="./exe1rb1g.png"
style="width:1.81861in;height:0.30625in" /><img src="./w2mlc454.png"
style="width:5.66486in;height:3.13375in" />

> <img src="./5k03khue.png"
> style="width:5.755in;height:0.38167in" />Abbildung 17: YOLOv3
> Comparison to Other Detectors
>
> Wie die Grafik zeigt, erreicht YOLOv3 im Vergleich zum MS
> COCO-Datensatz die beste Geschwindigkeit und Genauigkeit. Mit einer
> durchschnittlichen Genauigkeit (mAP) von 57,9% in 51 ms übertrifft
> YOLOv3 RetinaNet-101 um 57,5% in 198 ms.
>
> 4.4.2 Metriken

<img src="./evln1jrg.png"
style="width:3.31875in;height:1.97917in" />Zur Bewertung der Leistung
eines Systems wie in dieser Arbeit müssen mehrere Kriterien
berücksichtigt werden. Im Allgemeinen werden Kriterien wie Genauigkeit,
Effizienz (Ausführungsgeschwindig-

> keit) und Datenmenge, welche ab-gespeichert und verwendet wird,
> verwendet. Außerdem gibt es einige externe Faktoren, welche die
> Ge-nauigkeit des Systems beeinflussen können. Diese Faktoren sind:
> Zu-nächst die Umgebung (zum Zeit-punkt der Datenerhebung). Zum zweiten
> die unterschiedlichen Positi-

Abbildung 18: Berechnung von Precision, Recall und onen der zugehörigen
Sensoren. Accuracy in der Konfusionsmatrix. Sensoren, die Interaktionen
zwi-***Quelle:**https://www.researchgate.net/figure/Calcula-* schen dem
Nutzer und den Geräten
*tion-of-Precision-Recall-and-Accuracy-in-the-confu-* zu erkennen.

*sion-matrix_fig3_336402347*

> 29

<img src="./ghqgiwbm.png"
style="width:1.81861in;height:0.30625in" /><img src="./hb2qj10r.png"
style="width:2.76597in;height:0.54028in" />

> • **Accuracy** = TP+TN/TP+FP+FNTN.
>
> Die Genauigkeit bei Klassifikationsproblemen ist die Anzahl der
> richtigen Modellvor-hersagen geteilt durch die Gesamtzahl der
> Vorhersagen. Aber Genauigkeit ist keine gute Wahl für unausgewogene
> Klassen. Beispiel: Wenn der Testsatz 100 Bilder ent-hielt und das
> Modell 80 Bilder richtig vorhersagte, ist das Ergebnis 80/100. Dies
> ergibt eine Genauigkeit von 0,8 oder 80 %. Genauigkeit ist nützlich,
> wenn die Ziel-klassen ausgewogen sind. Daher ist es notwendig, andere
> Parameter zu betrach-ten, um die Leistung des Modells zu bewerten. Im
> Allgemeinen werden die folgen-den Parameter am häufigsten verwendet:
> Präzision und Recall.
>
> • **Präzision**
>
> Die Präzision ist dem Recall sehr ähnlich. Dadurch lässt sich die
> Anzahl der positi-ven Vorhersagen ermitteln, welche gut getroffen
> wurden.
>
> Das heißt, es ist die Anzahl der richtig vorhergesagten positiven
> Ergebnisse (True Positive) geteilt durch die Gesamtzahl der
> vorhergesagten positiven Ergebnisse (True Positive + False Positive).
>
> • **Recall**
>
> Der Recall gibt an, wie viel Prozent der positiven Fälle von dem
> Modell richtig vor-hergesagt wurden.
>
> Es handelt sich also um die Anzahl der gut vorhergesagten positiven
> Ergebnisse (True Positive) geteilt durch die Gesamtheit der positiven
> Ergebnisse (True Positive + False Negative).
>
> • **F1-Score**
>
> Obwohl beide nützlich sind, können weder die **Präzision** noch die
> **Recall** ein Modell des maschinellen Lernens vollständig auswerten.
> Separat betrachtetsind diese bei-den Messgrößen nutzlos.
>
> Wenn ein Modell ständig "positiv" vorhersagt, ist die Rückrufquote
> hoch. Im Gegen-teil, wenn das Modell niemals "positiv" vorhersagt, ist
> die Genauigkeit hoch.
>
> F1-Score kombiniert die beiden. Es ermöglicht eine gute Bewertung der
> Leistung eines Modells und wird benötigt, wenn man ein Gleichgewicht
> zwischen Precision und Recall suchen will. Es wird wie folgt
> berechnet:
>
> 30

<img src="./xvdz3uyd.png"
style="width:1.81861in;height:0.30625in" />

> 4.4.3 Probleme des trainierten Netzes
>
> Um die Daten währenddes Lernens auszuwerten, wird ein vereinfachter
> Ansatz des supervised learning (überwachten Lernens) verwendet. Sie
> wird in der Regel durch eine grafische Kurve dargestellt und soll die
> Lernleistung (Performance) eines Mo-dells anhand von Erfahrung oder
> Zeitverlauf zeigen. Diese Methode ist von größter Bedeutung für die
> Ermittlung von Lernproblemen, wie z. B. ein nicht ausreichend
> angepasstes oder übermäßig angepasstes Modell, sowie für die
> Feststellung, ob die Trainings- und Validierungsdatensätze ausreichend
> repräsentativ sind. Diese Leistung kann in zwei Kategorien von
> Problemen unterteilt werden.
>
> • Überanpassung (Overfitting)
>
> Das Modell passt sich zu sehr an das Datenrauschen an. Dies führt
> häufig zu einer niedrigen Fehlerquote bei den Trainingssätzen, aber
> eine hohe Fehlerquote bei den Test-/Validierungssätzen.
>
> • Underfitting
>
> Das Modell erfasst den zugrunde liegenden Datenverlauf nicht und passt
> nicht gut genug zu den Daten. Geringe Varianz, aber hohe Verzerrung.
> Eine schlechte An-passungsleistung ist oft das Ergebnis eines zu
> einfachen Modells.
>
> **4.5** **Eingesetzte** **Computer** **Vision** **Bibliotheken**
>
> Für die Umsetzung dieser Arbeit wurden die Ressourcen von google colab
> \[10\] ver-wendet. Diese Ressourcen bieten Vorteile, insbesondere bei
> der Visualisierung der Auswertung der Modellleistung. Google Colab ist
> für Deep-Learning-Aufgaben ge-dacht. Es bietet kostenlosen Zugang zu
> freien Grafikprozessoren (CPU und GPU), welche 12 Stunden lang
> kontinuierlich laufen können.
>
> 4.5.1 Hardware
>
> Zur UmsetzungundzumTrainingder
> neuronalenNetzewurdendiefolgendenHard-und Softwarekomponenten
> verwendet:
>
> Prozessor: Intel(R) Core(TM) i7-7500U CPU @ 2.70 GHz,290GHz
>
> Betriebssystem: Windows 10 Pro 64-bit
>
> Festplatte: 256 GB SSD
>
> Arbeitsspeicher: 8,00 GB RAM
>
> Grafikkarte: Intel(R) HD Graphics 520.
>
> 31

<img src="./f4aglvdm.png"
style="width:1.81861in;height:0.30625in" />

> 4.5.2 Technologie
>
> **A-**Python
>
> Python \[18\] ist eine sehr beliebte und vielseitige
> Programmiersprache. Eine seiner besonderen Eigenschaften ist die
> Fähigkeit, Standardbibliotheken zu sammeln. Für maschinelles Lernen
> und Data Science ist sie die am der häufigsten verwendete Sprache. Die
> Python-Software gibt es in mehreren Versionen.
>
> **B-**PyCharm
>
> PyCharm ist Jet-Brains' \[19\] integrierte Entwicklungsumgebung für
> die Program-miersprache Python. Es unterstützt sowohl die
> Webentwicklung als auch die Da-tenverarbeitung mit Anaconda \[20\].
>
> 4.5.3 Eingesetzte Python-Bibliotheken
>
> Für die Implementierung der Gesichts- und Maskserkennung wurde die
> Python 3.8 verwandelt. Es müssen zuerst einige Bibliotheken
> installiert werden. OpenCV \[21\] ist eine der wichtigsten und
> notwendigsten Bibliotheken für die Bildverarbeitung. Es ist eine
> Open-Source-Bibliothek für Computer Vision, maschinelles Lernen und
> Bild-verarbeitung. Es verfügt über einen Viola-Jones-Sensor zur
> Gesichtserkennung \[22\]. Im Vergleich zu anderen Bibliotheken ist sie
> schnell, denn sie ist in C/C++ ge-schrieben. Es funktioniert am besten
> auf Systemen mit wenig RAM und unterstützt die meisten Betriebssysteme
> wie Windows, Linux und MacOS. Es enthält sowohl einen Trainer (Cascade
> Training) als auch einen Detektor. Es bietet jedoch vordefi-nierte
> Klassifikatoren für die Erkennung von Dingen, wie zum Beispiel das
> mensch-liche Gesicht, den ganzen Körper, Körperteile und
> Gesichtsteile. Es werden daher in dieser Arbeit die vorhandenen
> Klassifikatoren der OpenCV-Bibliothek verwendet.
>
> **Dlib** \[23\] stellt Algorithmen für Bildverarbeitung und
> maschinelles Lernen bereit. Sie enthält die notwendige Implementierung
> für die Erstellung der Gesichtsdarstellun-gen und für den eigentlichen
> Erkennungsprozess. Die face_recognition-Bibliothek, welche von Adam
> Geitgey \[24\] erstellt wurde, umfasst die
> Gesichtserkennungsfunk-tionalität der **dlib**.
>
> 32

<img src="./zxa1wjt5.png"
style="width:1.81861in;height:0.30625in" />

> **Die** **weiteren** **installierten** **Bibliotheken** **sind** **:**

||
||
||
||
||
||

> **EINRICHTUNG** **DER** **UMGEBUNG**

||
||
||
||
||
||

> 33

<img src="./ielwqdea.png"
style="width:1.81861in;height:0.30625in" />

> **5** **Von** **der** **Gesichtserkennung** **zur**
> **Gesichtsmaskener-**
>
> **kennung**
>
> Am Ende der Vorbereitung der technischen Umgebung, begann die
> Recherche im Internet. Die Themen Gesichtserkennung und
> Identifizierung des Maskenträgers wurden einzeln betrachtet. Die
> Unterschiede und Vergleichspunkte zwischen den beiden Methoden wurden
> diskutiert. Zu beiden Methoden gab es im Internet viele Ergebnisse,
> aber nur wenige relevante und entscheidende Aussagen.
>
> **5.1** **Gesichtserkennung** **mit** **Deep** **Learning**
>
> In der Geschichte der Wissenschaft wurden viele Algorithmen zur
> Gesichtserken-nung entwickelt, aber die Genauigkeit und die
> Geschwindigkeit haben die Erwartun-gen nicht erfüllt. Zum Glück wurden
> signifikante Fortschritte gemacht, welche viel-versprechend sind.
> DieCNN wurden in verschiedenen Bildverarbeitungsanwendun-gen
> eingesetzt, einschließlich der Erkennung von Gesichtsausdrücken
> (Facial Ex-pression Recognition, FER). In mehreren Studien auf dem
> Gebiet des Deep Ler-nens werden Convolutional Neural Networks (CNN)
> verwendet\[25\]. Die Fähigkeit der Bilderkennung ist mit dem Einsatz
> von Deep Learning enorm gestiegen. Es wur-den bereits Prototypen von
> Gesichtserkennungsanwendungen entwickelt, welche gut funktionieren. So
> kann das Modell des Deep Neural Network heute jedes Ele-ment in einer
> Szene erkennen, wenn es dafür trainiert wurde. Zum Beispiel bei
> Fa-cebook, wo man mit nur wenigen Trainingsbildern einen Freund mit
> 95-98 % Ge-nauigkeit finden und identifizieren kann.
>
> 5.1.1 KI-Methoden und deren Vorbereitung zum Einsatz
>
> Damit ein Gesicht sofort erkannt werden kann, arbeiten
> Gesichtserkennungssys-teme \[26\] mit künstlicher Intelligenz. Mit
> Deep Learning werden Algorithmen darauf trainiert, menschliche
> Gesichter aus zahlreichen Fotos und Videos zu erkennen. Viele
> Unternehmen trainieren ihre neuronalen Netzwerke auf den Milliarden
> von Gesichtsfotos, welche von Instagram, Facebook oder Google im
> Internet gespei-chert werden. Für die Gesichtserkennung ist folgender
> Prozess erforderlich: Zu-nächst muss das Bild (Gesichter) von Personen
> in einem gut positionierten Bereich mit einer Kamera erfasst werden.
> Diese Gesichter werden dann in einer durchsuch-baren Datenbank
> gespeichert. Zur Erkennung der Gesichter verwendet das System
> schließlich die in der Datenbank gespeicherten Bilder und vergleicht
> sie mit bekann-ten Gesichtern. Es wurden bereits mehrere Algorithmen
> zur Gesichtserkennung im-plementiert. Die Viola-Jones-Methode \[27\]
> zur Gesichtserkennung ist die älteste, aber immer noch relevant. Die
> Algorithmen der Gesichtserkennung unterscheiden sich nicht wesentlich
> von den Algorithmen der Gesichtsmaskenerkennung. Die bei-den
> Algorithmen haben die gleichen Ziele aber unterscheiden sich in den
> Details. Entscheidend ist daher, den richtigen Algorithmus für die
> jeweilige Anwendung zu verwenden.
>
> 34

<img src="./tnsps3ix.png"
style="width:1.81861in;height:0.30625in" /><img src="./ucwtynnv.png"
style="width:1.975in;height:2.77847in" />

> 5.1.2 Gesicht Erkennung Algorithmus
>
> Deep Learning hat die Techniken der Gesichtserkennung durch den
> Einsatz von Algorithmen revolutioniert, welche Adam Geitgey \[24\]
> hier in drei Schritten versucht hat zu ordnen.
>
> **Zuallererst:** Der Algorithmus sieht sich ein Foto an und findet
> alle Gesichter darauf.
>
> **Zweitens:** Der Algorithmus muss sich auf jedes Gesicht
> konzentrieren und in der Lage sein, zu verstehen, dass es sich immer
> um dieselbe Person handelt, unab-hängig von der Position oder bei
> schlechter Beleuchtung des Bildes(Gesicht).
>
> **Drittens** **:** Er muss in der Lage sein, eindeutige
> Gesichtsmerkmale zu erkennen, anhand derer er sich von anderen
> Personen unterscheiden kann - wie Augengröße, Gesichtslänge usw.
> Vergleicht schließlich die einzigartigen Merkmale dieses Ge-sichts mit
> denen aller Personen, die er bereits kennt, um den Namen der Person zu
> bestimmen.
>
> Dieses Konzept ermöglicht es, die Forschung auf die geeigneten
> Algorithmen zu konzentrieren, welche die besten Ergebnisse für die
> anstehenden Forschungsar-beiten liefern werden.
>
> Fig 1 : Generischer Ablauf eines Gesichtserkennungssystems .
>
> Quelle :
> *https://www.h-brs.de/files/20171215_fbinf_mclab_ss15_gesichtserken-nung_malz_nawid_msmk.pdf*
>
> 35

<img src="./fh2zp4nm.png"
style="width:1.81861in;height:0.30625in" /><img src="./tui1icz2.png"
style="width:5.96667in;height:2.85625in" />

> 5.1.3 Theorie zum Gesichtserkennung mit OpenCV
>
> Die Theorien zur Gesichtserkennung werdenvon mehrerenAutorenin
> ihrenArtikeln diskutiert. Wie Mohamed Elgendy in seinem Buch "Deep
> Learning for Vision
>
> Basierend auf der Veröffentlichung in dem berühmten Buch Handbook of
> Face Recognition (Li et al., Springer, 2011) fasst er die
> Gesichtserkennung durch dieses Bild zusammen (Abbildung 19)
>
> Abbildung 19 Beispiel für Gesichtsverifizierung (links) und
> Gesichtserkennung (rechts) *Quelle* :
> *https://live-book.manning.com/book/grokking-deep-learning-for-computer-vision/chapter-1/84*
>
> 5.1.4 Datensatz
>
> Da es sich um ein Testprojekt handelt, werden nicht mehrere Bilder
> benötigt. Eine Suche im Internet ermöglichte es, passende Bilder für
> den Text zu finden.
>
> **5.2** **Die** **Verfahren** **kurz** **beleuchtet**
>
> Als Grundlage der Arbeit mit dem Gesicht Erkennung-Algorithmus diente
> ein Tuto-rial im Internet \[28\], welches von mehreren Personen, die
> sich mit dem Thema be-schäftigen vorgeschlagen wurde. Dort wurde ein
> fertiges Beispiel in Code über GitHub \[29\] bereitgestellt und
> einzelnen Code-Fragmente erklärt. Für das Verständ-nis dieser Arbeit
> musste sich im Detail mit dem Code beschäftigt werden, sowie
> Hintergrundwissen zum Verfahren Gesicht/Maskdetektion erarbeitet
> werden. An-fangswurde das bereitgestellte Tutorial
> durchgearbeitet.Hier mussten viele„Python Bibliothek“ installiert
> werden \[30\]. Nachdem dies auf den Computer ausgeführt wer-den
> konnte, wurde ein Plan zur weiteren Vorgehensweise erstellt. So war es
> sehr wichtig den vorbereiteten Datensatz in den Code einzuarbeiten.
> Nach längerem Probieren war es möglich, das Projekt mit Python zu
> durchzuführen.
>
> Der Gesichtserkennungsalgorithmus ist folgendermaßen unterteilt.
> Zunächst das Bild in Graustufen umwandeln. Dann wird der
> HOG-Algorithmus (Histogram of Ori-ented Gradients) zur Vereinfachung
> des Bildes angewendet. Dieses Bild wird an
>
> 36

<img src="./cczubqzx.png"
style="width:1.81861in;height:0.30625in" />

> den Haar-Kaskaden-Algorithmus gesendet, welcher sich um das Finden der
> Ge-sichter kümmert. Es wird das bereits trainierte Haar-Cascade-Modell
> verwendet, welches als "haarcascade_frontalface_alt2.xml" gespeichert
> ist.
>
> Nachdem alle Codes bekannt sind, geht es nun darum, die Gesichter zu
> vergleichen und Ähnlichkeiten zu finden. Um das Bild Paket(Datensatz)
> zu vergleichen, wird einer der maschinellen Lernmethoden der lineare
> *SVM-Klassifikator* verwendet. Die Funktion „*compare_faces“* wird
> dafür verwenden, um festzustellen, ob die Gesich-ter übereinstimmen.
> Diese Funktion gibt *True* oder *False* zurück. In ähnlicher Weise
> kann die Funktion *face_distance* verwendet werden, um herauszufinden,
> wie wahr-scheinlich die Übereinstimmung der Gesichter in Bezug auf die
> Anzahl ist. Dies ist besonders hilfreich, wenn es mehrere Gesichter zu
> erkennen gibt. Es gab viele Al-gorithmen zur Gesichtserkennung \[31\]
> .
>
> 5.2.1 Versuchsaufbau
>
> Der Quellcode, welcher in dieser Arbeit verwendet wird, ist auf GitHub
> verfügbar. Parallel zum Quellcode muss auch die Datei VGG-Face
> heruntergeladen werden. Die Aufgabe dieser Datei ist es, die Vektoren
> zu konstruieren, welche die in diesem Projekt verwendeten Bilder
> darstellen. Wie in den anderen Projekten ist auch hier Python 3 am
> besten geeignet. Es wurde die Version 3.6.8 von Python gewählt, da sie
> über die notwendigen Bibliotheken für die Bildverarbeitung und die
> Kamera ver-fügt. Nachdem die Vorbereitung der Python-Umgebung
> abgeschlossen ist, müssen nun einige sehr wichtige Bibliotheken
> importiert werden. So werden Bibliotheken wie : Os, Numpy usw.…
> importiert.
>
> Einzelheiten zum Code werden hier nicht angegeben. Im Internet sind
> jedoch meh-rere Quellcodes verfügbar. Man kann sowohl einen einfachen
> als auch einen kom-plexen Code verwenden. Hier wird der einfache Code
> verwendet, weil es nicht not-wendig ist, eine Funktion zu verwenden,
> welche die Kamera aktiviert oder die Frame-Leistung verbessert. Es
> geht nur darum, die Funktion zu implementieren, welche zwei Bilder
> vergleicht und die Unterschiede oder Ähnlichkeiten erkennt.
>
> <u>Codeausschnitt</u>
>
> *def* *\_extract_face(filepath,* *face_cascade):*
>
> *"""Extrahiert* *den* *Gesichtsbereich* *aus* *filepath* *mithilfe*
> *von* *face_cascade.* *Args:*
>
> *filepath* *(str):* *Pfad* *der* *Bilddatei*
>
> *face_cascade* *(cv2.CascadeClassifier):* *Kaskadenklassifizierer*
> *für* *Gesichter.* *Returns* *(Rückgabe):ndarray:* *Bereich* *oder*
> *Region* *des* *Gesichts*
>
> *"""*
>
> *img* *=* *Image.open(filepath).convert('L')* *img* *=*
> *np.array(img,* *np.uint8)*
>
> *\#* *führt* *die* *Gesichtserkennung* *mit* *den*
> *Standardeinstellungen* *aus* *face* *=*
> *face_cascade.detectMultiScale(img)*
>
> *\#* *lässt,* *wenn* *es* *nicht* *genau* *ein* *Gesicht* *gibt* *if*
> *len(face)* *!=* *1:*
>
> 37

<img src="./xigzdqvn.png"
style="width:1.81861in;height:0.30625in" /><img src="./ay4xuztc.png"
style="width:5.94514in;height:1.91806in" />

> *sys.exit("* *{}* *keinGesicht!".format(filepath))* *\#* *extrahiert*
> *das* *Gesicht* *aus* *dem* *Bild*
>
> *face* *=* *face\[0\]* *x,* *y,* *w,* *h* *=* *face*
>
> *face_region* *=* *img\[y:y+h,x:x+w\]* *return* *face_region*
>
> *def* *load_data(face_cascade,* *data_dir='yalefaces'):* *"""Lädt*
> *die* *Trainings-* *und* *Testdaten.........*
>
> 5.2.2 Ergebnisse
>
> Fig. 2: Gesichtserkennung
>
> Bild Quelle:
> https://www.tagesspiegel.de/politik/corona-gipfel-mit-der-kanzlerin-mer-kel-fordert-nationale-kraftanstrengung-im-november/26568550.html
>
> ▪ 1 - zeigt die Gesichtserkennung (True).
>
> ▪ *2* **-** Keine Gesichtserkennung, also (False).
>
> Fakt ist, dass der Gesichtserkennungsalgorithmus auf bestimmten Teilen
> des Ge-sichts basiert, wie Nase, Mund, Augen und Haare... Da das
> Gesicht maskiert ist, erkennt der Algorithmus nach Durchführung des
> Bildvergleichs nicht, dass es sich um dasselbe Gesicht handelt.
>
> 38

<img src="./pjlivfdr.png"
style="width:1.81861in;height:0.30625in" /><img src="./qihb2ruu.png"
style="width:2.36139in;height:1.8425in" /><img src="./mfevural.png"
style="width:2.53903in;height:1.90764in" />

> **5.3** **Aufbau** **einer** **Gesichtsmaskenerkennung** **mit**
> **Deep** **Learning**
>
> Abbildung 20 : Gesichtsmaskenerkennung
>
> *Quelle* *:* *https://github.com/chandrikadeb7/Face-Mask-Detection*
>
> Die Erkennung von Gesichtsmasken besteht darin, festzustellen, ob eine
> Person eine Maske trägt oder nicht. Dieser Ansatz ist ähnlich wie der
> vorherige. Es geht einfach darum, das Problem auf eine andere Weise zu
> betrachten, um die Antwort auf das Problem zu finden, welches gestellt
> wurde. Wie gesagt, die Algorithmen, welche für dieses Problem
> verantwortlich sind, folgen dem gleichen Prinzip. Zu-nächst wird ein
> Gesicht erkannt. Dann sollte erkannt werden, ob eine Maske auf das
> Gesicht gesetzt wird oder nicht. Es wurden von verschiedenen
> Wissenschaft-lern unterschiedliche Lösungsansätze entwickelt. Jeder
> dieser Ansätze hat seine eigenen Vor- und Nachteile. In dieser Arbeit
> soll es um einen der populären Ansätze gehen.
>
> 5.3.1 Der Einsatz eines vortrainierten Modells
>
> Transferlernen ist die Anwendung von Wissen, das bei der Durchführung
> einer Auf-gabe gewonnen wurde, um ein anderes, aber ähnliches Problem
> zu lösen. Bei der Durchführung unserer Arbeit war es sehr schwierig,
> eigene zuverlässige Daten zu erhalten. Außerdem ist es zeitaufwändig,
> ein mehrschichtiges CNN von Grund auf zu trainieren. Um dieses Problem
> zu lösen, wurde ein Verfahren verwendet, das als Transfer Learning
> bekannt ist. Einigen Autoren zufolge würden die Arbeit mit einer
> unzureichenden Datenmenge zu einer Leistungsminderung führen. Das
> bedeutet in dem Fall, dass man mit einem vortrainierten Modell
> beginnen und so bessere Mo-delle erstellen können. Das Ziel ist ein
> allgemeines Netz, das sich ohne Umstruktu-rierung und Schulung an
> unterschiedliche Bedürfnisse anpassen kann. Normaler-weise verwenden
> Datenwissenschaftler einen Datensatz wie ImageNet, eine
> Bild-datenbank, welche für Forschungsprojekte verwendet wird und als
> Referenz für die Bildklassifizierung und Objekterkennung gilt. Der
> ImageNet-Datensatz enthält 14197122 Bilder, die gemäß der
> WordNet-Hierarchie annotiert sind. Im Netz findet man eine Liste mit
> verschiedenen vortrainierten Modellen auf der Grundlage von ImageNet.
> Beispiele sind ResNet50 ,MobileNetV2, VGG16...
>
> 39

<img src="./pdcj5hdz.png"
style="width:1.81861in;height:0.30625in" /><img src="./hndnxhmv.png"
style="width:3.84583in;height:1.67153in" />

> **5.4** **MobileNetV2**
>
> Eine der an den häufigsten verwendeten Architekturen für die
> Implementierung von Gesichtsmasken ist MobinetV2. Wie der Name schon
> sagt, basieren MobileNets auf einer optimierten Architektur, die
> tiefen-separierbare Faltungen verwendet, um leichtgewichtige tiefe
> neuronale Netze aufzubauen.
>
> MobilelNet ist eine der besten CNN-Architekturen, da sie leicht in
> mobilen Anwen-dungeneingesetzt werden kann. MobileNetV2-Architektur
> führt invertierteResiduen und lineare Engpässe ein, um die Leistung
> von MobileNets zu verbessern. Sein besonderes Merkmal sind die in der
> Tiefe trennbaren Faltungen(Depthwise Sepa-rable Convolutions). Bei
> einer trennbaren Faltung wird ein normales Faltungskernel in zwei
> Kernel aufgeteilt. So wird beispielsweise aus einem 4x4-Kernel ein
> 4x1-Kernel und ein 1x4-Kernel. Diese Trennung macht sie effizienter,
> da sie die Anzahl der für die Durchführung der Faltung erforderlichen
> Operationen reduziert. Im Un-terschied zu MobilNetV1 wird in der
> MobileNetV2-Architektur ein weiteres Modul mit einer invertierten
> Reststruktur eingeführt. In den schmalen Schichten werden zum Beispiel
> die Nichtlinearitäten entfernt. Diese Änderungen in MobileNetV2 machen
> es zu einer besseren Architektur für die Objekterkennung und
> semantische Seg-mentierung. In Kera werden sie mittels der Funktion:
> *keras.layers.Separab-leConv2D* *oder* *tf.layers.separable_conv2d*
> *implementiert* *\[32\]* verdeutlicht*.*
>
> 5.4.1 Netzwerke Struktur
>
> Die MobileNetV2-Architektur enthält eine erste volle Faltungsschicht
> mit 32 Filtern, gefolgt von 19 restlichen Engpassschichten. Dabei ist
> **t** der Erweiterungsfaktor, **c** die Anzahlder Ausgangskanäle,
> **n**die Anzahl der Wiederholungen und **s** der Schritt. Für die
> räumliche Faltung werden 3×3 Kernel verwendet. Für beide Arten von
> Blö-cken gibt es 3 Schichten. Die erste Schicht ist eine 1×1-Faltung
> mit ReLU6 (ReLU6 als Nichtlinearität wegen seiner Robustheit bei
> Berechnungen mit geringer Genau-igkeit). Die zweite Schicht ist die
> Tiefenfaltung. Die dritte Schicht ist eine weitere 1×1-Faltung, jedoch
> ohne jegliche Nichtlinearität.
>
> <img src="./vmd1xl2l.png"
> style="width:3.08667in;height:0.425in" />Abbildung 21:
> MobileNetV2-Architektur
>
> 40

<img src="./cexegimj.png"
style="width:1.81861in;height:0.30625in" /><img src="./r33vsbcd.png"
style="width:5.775in;height:2.05903in" />

> 5.4.2 Objekt Detektion
>
> Ein Experiment mit dem COCO-Datensatz (Figure 2)hat gezeigt, dass
> MobileNetV2 + SSDLite mit weitaus weniger Parametern und geringerer
> Rechenkomplexität eine konkurrenzfähige Genauigkeit erzielt. Es kann
> auch leicht beobachtet werden, dass die MobileNetV2-Inferenzzeit
> schnellerist als MobileNetV1. MobileNetV2 + SSDLite ist 20-mal
> effizienter und 10-mal kleiner und dabei immer noch leistungsfähiger
> als YOLOv2.
>
> Fig. 3: MobileNetV2 Performance
>
> 5.4.3 Modellaufbau Gesichtsmaskenerkennung mit Python
>
> Dieser Teil ist eine Fortsetzung des für die Gesichtserkennung
> implementierten Al-gorithmus, jedoch mit einigen Modifikationen. Wir
> benötigen einen Klassifikator, der in der Lage ist, Gesichter mit und
> ohne Maske zu unterscheiden. Mit dem Mo-bileNetV2-Netzwerk \[32\], das
> auf dem ImageNet-Datensatz trainiert wurde, steht uns hierfür bereits
> ein vortrainiertes Netzwerk zur Verfügung. Zur Detektion von
> Ge-sichtsmasken schlugen die Autoren einen auf Deep Learning
> basierenden Ansatz mit TensorFlow, Keras und OpenCV dar. Der
> SSDMNV2-Ansatz verwendet den **Single** **Shot** **Multibox**
> **Detector** als Gesichtsdetektor und die MobilenetV2-Archi-tektur als
> Rahmen für den Klassifikator.
>
> 5.4.4 Datensatz Gesicht-Maske-Erkennung
>
> Die Erstellung eines Maskendetektors mit YOLO erfordert relevante
> Daten. Wir be-nötigen annotierte Daten mit Bounding Boxes. Viele
> bereits trainierte Datensätze sind im Netz zu finden. Daher wird einen
> der beliebtesten Datensätze ausgewählt werden. Es wird den Face Mask
> Detection-Datensatz von Kaggle \[33\], herunterge-laden und in dem
> Google Drive gespeichert. Der Datensatz umfasst 10.000 Bilder. Es wird
> versucht, einige der Bilder zu entfernen, da sie nicht wirklich zu den
> ge-wünschten Bildern passen. Nach Bereinigung der Daten erhielt man
> 4650 Bilder. 3500 werden für Tests und 1150 für die Validierung
> verwendet. Der Datensatz, den der Autor verwendet hat, besteht aus
> 1376 Bildern, welcher zu zwei Klassen gehö-ren: with_mask: 690 Bilder
> without_mask: 686 Bilder.
>
> 41

<img src="./o0webq55.png"
style="width:1.81861in;height:0.30625in" />

> 5.4.5 Gesichtsmaskenerkennung Algorithmus
>
> Wie die Gesichtserkennung umfasst auch die Gesichtsmaskenerkennung
> mehrere Schritte.
>
> -Zunächst muss das Modell mit einem geeigneten Datensatz trainiert
> werden.
>
> -Der zweite Schritt besteht darin, ein genaues
> Gesichtserkennungsmodell anzu-wenden, damit das Modell in der Lage
> ist, Gesichter mit Maske und Gesichter ohne Maske zu klassifizieren.
>
> 5.4.6 Aufbau des Modells
>
> In diesem Abschnitt wird nicht auf die Einzelheiten der
> Bibliotheksimporte eingegan-gen. Der Fokus liegt auf der Konstruktion
> der Modellstruktur.
>
> <img src="./1tw3oego.png"
> style="width:5.66111in;height:1.77444in" /><img src="./rfkeragq.png" style="width:5.66167in;height:0.29in" />Fig.
> 4: Die Erstellung des Modells
>
> ▪ Mit **Sequentiel()** kann man in Keras ein Modell Schicht für
> Schicht aufbauen. Die Funktion **'add()'** fügt unserem Modell
> Schichten hinzu.
>
> ▪ **Conv2D-Schichten**. Dies sind Faltungsschichten, die sich mit
> unseren Ein-gabebildern befassen, die als 2-dimensionale Matrizen
> angesehen werden.
>
> ▪ **32** **in** **der** **ersten** **Schicht** **und** **64** in der
> zweiten Schicht sind die Anzahl der Knoten in jeder Schicht. Diese
> Zahl kann je nach Größe des Datensatzes höher oder niedriger
> eingestellt werden.
>
> ▪ **(3,3)** Kernelgröße ist die Größe der Filtermatrix für unsere
> Faltung. Eine Kernelgröße von 3 bedeutet also, dass man eine
> 3x3-Filtermatrix hat.
>
> ▪ **activation=**'relu' : ist die Aktivierungsfunktion für den Layer.
> Die hier verwen-dete Aktivierungsfunktion ist die ReLU oder Rectified
> Linear Activation.
>
> ▪ **150,150,3** **:** ist die Form jedes Eingabebildes wobei die 3
> bedeutet, dass die Bilder RGB sind.
>
> ▪ Zwischen den Conv2D-Ebenen und der dichten Ebene befindet sich eine
> Ebene **Flatten:** Flatten dient als Verbindung zwischen der Faltung
> und den dichten Schichten.
>
> 42

<img src="./3khh4bnt.png"
style="width:1.81861in;height:0.30625in" /><img src="./t5igykh2.png"
style="width:4.70347in;height:4.00722in" />

> ▪ **Dense:** ist der Layertyp, welche für den Ausgabelayer verwendet
> ist. Dense ist ein Standard-Layer-Typ, welche in vielen Fällen für
> neuronale Netze ver-wendet wird. Hier hat man **256** Knoten in der
> Ausgabeschicht. Die Aktivie-rung ist **sigmoid.** die Sigmoidfunktion
> wird auf die Summe der gewichteten Eingabewerte angewendet, um die
> Ausgabe des Neurons zu erhalten.
>
> <img src="./xoqoeplx.png"
> style="width:3.85833in;height:0.375in" />Abbildung 22 : ModellAufbau
>
> 5.4.7 Evaluation
>
> Es zeigt sich, dass das Modell nach 2-3 Epochen beginnt die
> Trainingsdaten zu überanpassen. Die durchschnittliche Genauigkeit,
> welche in dem Validierungssatz erhalten, beträgt etwa 69 %. Das ist
> ein faires Ergebnis, aber es lässt sich noch verbessern. Es wird
> versucht, das Modell durch Hinzufügen zusätzlicher Schichten zu
> erweitern (Abbildung 22). Die erste Beobachtung nach dem Hinzufügen
> zusätz-licher Schichten ist, dass sich das Modell schnell anpasst(Fig
> 3).
>
> Die folgenden Änderungen werden vorgenommen: Das Modell wird auf 30
> Epoc trainiert, aber es wurde keine Leistung beobachtet. Es wird
> danach auf einigen Videos getestet, aber das Ergebnis war nicht so
> gut, wie es erwartet ist. So wird später versucht, das Modell durch
> Anpassen der Ebene zu ändern.
>
> 43

<img src="./xjky3zdm.png"
style="width:1.81861in;height:0.30625in" />

> <img src="./efaqgbnu.png"
> style="width:2.80986in;height:2.14319in" /><img src="./mkt04z0f.png"
> style="width:0.46167in;height:0.29667in" /><img src="./0wocfgot.png"
> style="width:2.65833in;height:2.04458in" /><img src="./zchufgx4.png"
> style="width:0.46333in;height:0.35667in" />(a) (b)
>
> <img src="./yi1ky1pj.png"
> style="width:5.86833in;height:0.35833in" />**Fig.** **5** (a) & (b)
> Trainings- und Validierungsgenauigkeit des Modells über 120 Epochen
>
> Nachdieser Änderungwird ein weiteres Trainingmit 120Epochedurchgeführt
> (Abb. 5).Es ändertesich immer nochnichts. Anstattdie
> Lehrlingsquotezuerhöhen, wurde entschieden, sie zu senken. Dieses Mal
> ist das Ergebnis viel besser als beim letzten Mal. Die folgende
> Tabelle zeigt das bisherige Ergebnis im Vergleich zum anderen
> Ergebnis. Die Endwerte des Verlusts, welche nach ~60 Epochen erhalten
> wurden, sind: Trainingsverlust 0,2 & Genauigkeit 0,9.
>
> <img src="./0azbqyfk.png"
> style="width:2.81805in;height:1.95986in" /><img src="./wquppiux.png"
> style="width:0.455in;height:0.30167in" /><img src="./t3ey5cnu.png"
> style="width:0.45667in;height:0.30167in" /><img src="./yzs01stm.png"
> style="width:2.90722in;height:1.95847in" />(a) (b)

**Fig.** **6** (a) & (b) Training Validierungsverlust- und
Validierungsgenauigkeit des Modells

> 44

<img src="./gtiuao4f.png"
style="width:1.81861in;height:0.30625in" />

> 5.4.8 Training Ergebnis der verwendeten Arbeit
>
> Hier sind die Ergebnisse der Autoren, welche sich bereits mit diesem
> Thema be-schäftigt haben, in Bezug auf Genauigkeit undGeschwindigkeit
> \[34\].Vergleicht man das Ergebnis mit dem der Quellenarbeit, so
> stellt man fest, dass unser Ergebnis nicht besser ist. Wir haben
> weniger Daten verwendet als der Autor, weil man die Daten bereinigt
> hat. Es ist daher offensichtlich, dass das Ergebnis umso weniger mit
> der Arbeit des Autors vergleichbar ist, je weniger Daten man hat. Es
> ist auch möglich, dass die Konfiguration und die Umgebung, wo der Test
> durchgeführt wurde, weniger effizient sind als die des Autors. Eine
> weitere Beobachtung, welche man feststellen konnte, ist die
> Veränderung der Ergebnisse, welche man erhält, wenn wir die Anzahl der
> Epoc erhöhen.
>
> Die Verwendung der MobileNetV2-Architektur auf dem verwendeten
> Mask/Non-Mask-Datensatz ermöglichte es dem Autor ~99% Genauigkeit auf
> dem Testsatz zu erzielen. Offensichtlich zeigen die Kurven für
> Genauigkeit und Trainingsverlust eine hohe Genauigkeit und kaum
> Anzeichen für eine Überanpassung der Daten. Ein Blick auf die
> Abbildung 23 zeigt, dass es kaum Anzeichen für eine Überanpassung
> gibt, wobei der Validierungsverlust niedriger ist als der
> Trainingsverlust.
>
> <img src="./i12foyzw.png"
> style="width:5.25903in;height:3.16319in" />Abbildung 23 :
> Trainingsverlust und Genauigkeitskurven
>
> Quelle : https://github.com/akashkam559/Covid19-Face-Mask-Detector
>
> 45

<img src="./0e3t4hb4.png"
style="width:1.81861in;height:0.30625in" /><img src="./u4gii0mp.png"
style="width:5.96667in;height:2.95833in" />

> **5.5** **Gesichtsmasken-Erkennung** **mit** **YOLOv3**
>
> 5.5.1 Verwandte Arbeiten
>
> Wie bereits eingangs erwähnt, wurden bereits mehrere Algorithmen zur
> Erkennung von Gesichtsmasken von Autoren entwickelt.
>
> Abbildung 24 : Netzwerkarchitektur YOLOv3
>
> Quelle :
> <https://link.springer.com/article/10.1007/s11042-021-10711-8>
>
> 5.5.2 Modellbeschreibung
>
> Der YOLO-Algorithmus \[35\] verwendet nur einen
> Vorwärtspropagationsdurchlauf \[36\], um Objekte in einem einzigen
> Eingangsbild zu erkennen. Die Autoren des Mo-dells verwendeten daher
> Yolov3 , um die Maskenerkennung auf dem Gesicht zu implementieren
> \[37\]. Der vorgeschlagene Algorithmus zur Gesichtsmaskenerken-nung
> \[38\] besteht aus drei Schritten: Vorverarbeitung, Gesichtserkennung,
> Masken-erkennung. Der erste Schritt (Vorverarbeitung)besteht darin,
> die Qualität des Ein-gangsbildes zu verbessern und auch die Kanten mit
> einem Unschärfefilter zu ver-bessern.
>
> Der zweite Schritt ist die Erkennung der Gesichtsregionen. Wie bereits
> im Kapitel 2 zur Gesichtserkennung beschrieben, wurde auch hier der
> von Viola-Jones\[3\] vor-geschlageneHaar-Kaskaden-Klassifikator
> zurErkennungder Bildgrößenregionver-wendet. Der letzte Schritt
> (Maskenerkennung )besteht darin, zu erkennen, ob die Person die Maske
> trägt oder nicht. Dazu wird den Vorhersageprozess auf 3 Ebenen
> aufgebaut:13x13,26x26, und 52x52. Die letzte Erkennungerfolgt durch
> die Schicht 106, mit einer Größe von 52x52x27.
>
> 46

<img src="./fo0mxaqh.png"
style="width:1.81861in;height:0.30625in" />

> 5.5.3 Datensatz
>
> Für das Experiment verwenden den Autoren den Datensatz MAFA \[39\] ,
> der aus 35.806 maskierten Gesichtern mit einer Mindestgröße von 32x32
> besteht. Der Da-tensatz ist in drei Teileunterteilt, die jeweils 5000,
> 1000und1000 Bilder für Training, Validierung und Test enthalten.
>
> 5.5.4 Training
>
> Das Training wurde mit 70 Epochen durchgeführt. Die Fig. 7 zeigt den
> Verlust von dem Training und der Validierung. Die in der Kurve
> dargestellten Ergebnisse zei-gen, dass der Trainingsverlust 5,15 % und
> der Validierungsverlust 5,27 erreichen kann.
>
> <img src="./nm3hxmom.png"
> style="width:3.30333in;height:0.25667in" /><img src="./3k2mprfm.png"
> style="width:3.75625in;height:1.89986in" />Fig 7: Der Trainings- und
> Validierungsverlust
>
> 5.5.5 Leistung
>
> Die Präzision gibt die Genauigkeit des Algorithmus auf Basis des
> Klassifizierungs-ergebnisses an. Der Recall beschreibt die Fähigkeit,
> alle relevanten Objekte in ei-nem Datensatz zu finden. Die
> nachstehende Fig. 8 zeigt die Leistungsmessungen des vorgeschlagenen
> Algorithmus und einer anderen Methode, welche das lokal lineare
> Integrationsfaltungsnetz (LLE-CNN) \[40\] verwendet. Die Genauigkeit
> des vorgeschlagenen Algorithmus erreicht 90,1 % und ist damit etwas
> höher als die der anderen Methoden.

||
||
||
||
||

> *Fig* *8* *:* *Vergleich* *zwischen* *dem* *vorgeschlagenen*
> *Algorithmus* *und* *anderen*
>
> 47

<img src="./cepwcx0h.png"
style="width:1.81861in;height:0.30625in" />

> **6** **Selbst** **modifizierter** **YOLO-Ansatz**
>
> Einer der wichtigsten Teile unserer Arbeit besteht auch darin, zu
> erkennen, ob die Maske tatsächlich getragen wird und welche Art von
> Gesichtsmasken die Person trägt. Handelt es sich um eine FFP2-Maske,
> eine chirurgische Maske oder eine selbstgebaute Maske? In seiner
> Publikation:" How to Correctly Detect Face-Masks for COVID-19 from
> Visual Information?" befasst sich der Autor Batagelj \[39\], mit
> demselben Thema und schlägt außerdem einen Algorithmus zur Erkennung
> von Gesichtsmasken vor. Seine Methoden sind auch die Grundlage für
> unsere For-schung und die Problematik dieses Themas.
>
> **6.1** **Bilder** **Vorbereitung** **Erkennungsraten**
>
> Die Erstellung eines Maskendetektors mit YOLO erfordert relevante
> Daten. Es wur-den annotierte Daten mit Bounding Boxes benötigt. Viele
> bereits trainierte Datens-ätze sind im Netz zu finden. Aber man kann
> auch Bilder in Internet suchen, welche man selbst annotieren kann .
> Die Recherche nach den Bildern(Datensatz), war nicht einfach. Die
> Daten stammen aus verschiedenen Quellen und sind daher un-einheitlich.
> Manchmal werden Bilder aus Screenshots von Fernsehnachrichten oder von
> YouTube oder von Fußballspielen, bei denen die Zuschauer Masken
> tru-gen, genommen. Letztendlich ist es gelungen, 1115 Daten zu
> erhalten: 815 für Tests und 300 für die Validierung.
>
> Es soll berücksichtigt werden, dass die Bilder aus dem Video-Stream
> oft von der Qualitätder Kameraund unterschiedlichen Lichteinstellungen
> abhängig sind. Daher ist der Datensatz vielfältig in Bezug auf
> Gesichter verschiedener Altersgruppen, Maskentyp und Maskenfarbe, aber
> auch den Bildhintergrund.
>
> **6.2** **Training** **Yolov3**
>
> Um an der Erkennungder verschiedenen Kategorien von Masken zu
> arbeiten, sollte zunächst das YOLOv3-Modell trainiert werden. Für das
> Training wird die vorhande-nen vortrainierten Gewichte des Darknets
> verwendet, welche bereits auf einem gro-ßen Datensatz trainiertwurden.
> Diese Gewichte können auf der Website des Autors Joseph Redmon \[41\]
> gefunden werden. Die Datei yolov3.cfg wurde angepasst und einige
> Parameter geändert, die für den Zweck dieser Arbeit erforderlich sind.
> Die Datei yolov3.cfg wird unbenannt in *cov_yolov3.cfg*.
> Darknet53.conv wurde ur-sprünglich für die Klassifizierung auf dem
> ImageNet-Datensatz trainiert und dient als Extraktor. Um es für die
> Erkennung zu verwenden, werden die zusätzlichen Ge-wichte im
> YOLOv3-Netzwerk vor dem Training zufällig initialisiert. Ihre
> richtigen Werte werden in der Trainingsphase ermittelt\[23\]. In dem
> Darknet gibt es eine Datei namens Makfile. In dieser Datei werden
> einige Änderungen vorgenommen.
>
> 48

<img src="./p1ybd4t2.png"
style="width:1.81861in;height:0.30625in" /><img src="./vvvf0jrs.png"
style="width:6.01528in;height:2.26389in" /><img src="./nhc1kfmx.png"
style="width:3.21806in;height:2.56944in" />

> **6.3** **Vorbereitung** **der** **Daten**
>
> Die verwendeten Bilder sind auf png-Format Andere Format konnten auch
> verwen-det werden. Es ist wichtig zu prüfen, ob die Bildformate alle
> dasselbe Format haben. Sind nicht alle Formate konform, z. B. wenn es
> mit Bildern im jpg-Format gemischt ist, funktioniert das Training.
> Jedoch werden die Dateien nicht geladen. Diese Da-teien werden in dem
> Trainingsmodell fehlen, was sich auf das Training und die Ge-nauigkeit
> auswirken wird.
>
> Fig 9: Modifikation in Darknet
>
> Fig 10 : Modifikation in Darknet
>
> Im Makefile (Fig.5) werden einige Änderungen vorgenommen. Das Training
> kann mit den bereits trainierten Darknet-Gewichten \[42\] vorgenommen
> werden, welche bereits auf großen Datensätzen trainiert wurden. Die
> Gewichte Yolov3 (Fig.6). Oder yolov4conv.127 von Alexey \[43\] google
> Drive link wurden heruntergeladen.
>
> 49

<img src="./ixgrficq.png"
style="width:1.81861in;height:0.30625in" /><img src="./v4mm4q45.png"
style="width:2.80569in;height:2.68472in" /><img src="./dazdbdnn.png"
style="width:2.48305in;height:2.58167in" /><img src="./3lhx5k5h.png"
style="width:1.32374in;height:0.77393in" /><img src="./xkzavg0l.png"
style="width:2.60139in;height:0.90272in" /><img src="./ycweybn4.png"
style="width:1.99083in;height:0.90567in" />

> Folgende Änderung wurden gemacht:
>
> • Die Datei yolov3.cfg wird unbenannt in *cov_yolov3.cfg*
> •     Subdivisions auf 64.
>
> • Zeile max_batches in 64
>
> • Filter auf 18 anstelle von 255.
>
> • Eingabegrößen auf den Standardwert width=416, height=416.
>
> Die folgenden Grafiken zeigen die Änderungen, welche an der Datei
> vorgenommen wurden (Fig 7). Diese Änderungen sind sehr wichtig, denn
> wenn man versucht, ohne sie zu trainieren, stürzt das System ab.
>
> Fig 11 Modifikation in Darknet
>
> <img src="./c3u3e21n.png"
> style="width:3.86667in;height:0.33667in" />Fig 12: Definition von
> Klassen
>
> 50

<img src="./0wbtm50l.png"
style="width:1.81861in;height:0.30625in" /><img src="./wqy4ep1z.png"
style="width:6.01528in;height:3.11958in" />

> **6.4** **Klassen** **für** **verschiedene** **Maskentypen**
>
> Um die verschiedenen Arten von Masken zu klassifizieren, müssen wir
> dem Com-puter beibringen, zwischen einem Gesicht, das keine Maske
> trägt, und einem, das eine Maske trägt, zu unterscheiden. Wir können
> durch Hinzufügen mehrerer Mas-kentypen erweitern. Die begrenzte Anzahl
> der verfügbaren Bilder ermöglicht uns dies jedoch nicht. Hierfür
> werden 300 Bilder annotiert. Es wurde das Vorhandensein des Maskentyps
> durch eine einfache und präzise Beschriftung gekennzeichnet. Zu diesem
> Zweck werden die folgenden vier Klassen erstellt: \[FFP2_Mask,
> Nio_Mask, OP_Mask, No_Mask\].
>
> <img src="./22mey0q2.png"
> style="width:3.745in;height:0.35833in" />*Abbildung* *25:* *Klassen*
> *für* *Masken* *Typen*
>
> 51

<img src="./5gofrlnu.png"
style="width:1.81861in;height:0.30625in" />

> **6.5** **Annotation** **Data**
>
> <img src="./oxfn500a.png"
> style="width:6.15417in;height:2.51528in" />Für die Annotation der
> Bilder stehen mehrere Annotationswerkzeuge zur Verfü-gung. Unter
> anderem gibt es
> [LabelMe,](https://www.v7labs.com/blog/best-image-annotation-tools#labelme)
> [Labelimg,](https://www.v7labs.com/blog/best-image-annotation-tools#labelimg)
> [VoTT,](https://www.v7labs.com/blog/best-image-annotation-tools#vott)
> [ImgLab.](https://www.v7labs.com/blog/best-image-annotation-tools#imglab)
> Für dieses Projekt wurde [*Makesense.ai*](http://makesense.ai/)
> verwendet. [Makesense.ai](http://makesense.ai/) ist ein kostenloses
> Online-Tool zum Beschriften von Fotos. Es ist keine erweiterte
> Installation erforderlich. Die Er-stellung verschiedener Maskenklassen
> erfordert die Anfertigung eines eigenen Da-tensatzes, welcher den
> Anforderungen der Forschung entspricht. Dazu haben wer-den im Internet
> zahlreiche Bilder gesammelt, welche später annotiert werden.

||
||
||
||
||

> **6.6** **Data** **Augmentation**
>
> Eines der Hauptprobleme beim Training dieser CNN- und YOLO-Detektoren
> ist die Anzahl der Bilder mit den Merkmalen, die für das Training der
> Klassifikatoren benö-tigt werden, sowie die Qualität der Bilder.
> Aufgrund der Schwierigkeiten, genügend Bilder zu sammeln, diezu guten
> Ergebnissen führen können, ist es manchmal wich-tig, Methoden der
> Datenerweiterung auf unsere bereits vorhandenen Daten anzu-wenden.
> Durch Augmentierungstechniken \[44\] können Bildvariationen erzeugt
> wer-den, welche die Fähigkeit der Trainingsmodelle verbessern. Dies
> verbessert die Leistung des Modells erheblich. Bei der Augmentation
> werden Methoden wie Dre-hen, Verschieben, Zoomen, Scheren und Spiegeln
> des Bildes angewendet. Ziel ist es viele Versionen eines ähnlichen
> Bildes zu erzeugen. Daher wird nicht versucht weitere Daten zu finden
> und zu beschriften, sondern neue Daten werden auf der Grundlage
> dessen, was man hat erstellt. Diese Technik wurde bereits in ähnlichen
> Projekten eingesetzt, vor allem in „Masked Face Recognition with
> Generative Data Augmentation and Domain Constrained Ranking" \[45\].
>
> 52

<img src="./xqordct5.png"
style="width:1.81861in;height:0.30625in" /><img src="./t31qqr5o.png"
style="width:5.77083in;height:2.325in" />

> **6.7** **Versuchsaufbau**
>
> Das Training mit der CPU ist sehr langsam (es kann Tage dauern, bis
> ein einfaches Modell fertig ist).
>
> Die Trainingszeit kann durch den Einsatz eines Grafikprozessors
> drastisch verbes-sert werden (mehr als das 500-fache der Zeit). Wir
> werden also eine GPU verwen-den, welche Google Colab kostenlos zur
> Verfügung stellt.
>
> Zunächst wird geprüft , ob der Grafikprozessor des Systems CUDA
> unterstützt und sicherstellt, dass die Runtime des Grafikprozessors
> verwendet wird. Der Befehl *!nvi-dia-smi* in der Google-Colab liefert
> die Ergebnisse dieser Überprüfung. Dies ist ein Zeichen dafür, dass
> Google-Colab-Umgebung für Tests bereit ist.
>
> Abbildung 27: !nvidia-smi Google-Colab-Umgebung
>
> **6.8** **Testphase**
>
> Nach der Lernphase wird überprüft, was das Netzwerk gelernt hat. Das
> heißt, es wird geprüft, ob passende Gewichtsanpassungen vorgenommen
> wurden. Dies wird als Validierung des Modells bezeichnet. Dazu werden
> sowohl der gelernte als auch der ungelernte Datensatz verwendet. Das
> Hauptziel ist es, zu überprüfen, ob das Modell in der Lage war, die
> Trainingsobjekte zu erfassen, aber auch und vor allem, ob es die
> allgemeinen Anforderungen korrekt löst.
>
> 53

<img src="./jz54xrfy.png"
style="width:1.81861in;height:0.30625in" /><img src="./3xyr11gd.png"
style="width:5.7868in;height:2.06667in" />

> **6.9** **Training**
>
> Das folgende Diagramm zeigt, wie die Daten aufgeteilt sind. Um das
> Modell zu trai-nieren und zu validieren, werden die Daten in zwei
> Teile geteilt. Man hat also 80 % der Daten zum Trainieren und 20 % zum
> Testen. Die Dateien *train.txt* und *test.txt* sehen dann etwa so aus:
>
> **Fig.13** : Aufteilung der Daten Train und Testset
>
> **6.10Evaluation** **und** **Diskussion** **der** **Ergebnisse**
>
> 6.10.1 Evaluation
>
> <img src="./c201sc3h.png"
> style="width:2.57292in;height:1.81903in" /><img src="./s5n2zzxy.png" style="width:2.5in;height:0.48667in" /><img src="./dlmq0fgo.png"
> style="width:2.56847in;height:1.82167in" /><img src="./hyuapcxj.png" style="width:2.91667in;height:0.39in" />Die
> Grafikenuntenzeigen die Ergebnisse für das ModellYolov3.Nach
> demTraining über 70 Epochen beobachten wir, dass nach 5
> Trainingsepochen der Validierungsverlust zu steigen beginnt, während
> der Trainingsverlust weiter abnimmt. Dies ist ein Zeichen für eine
> Überanpassung. Betrachtet man die Anzahl der Epochen als
> Hyperparameter. Wenn die Anzahl der Epochen auf 30 begrenzt wird und
> das Modell neu trainiert wird, sind die Ergebnisse besser. Und wie das
> nachstehende Diagramm zeigt, erreicht das Modell eine Genauigkeit von
> 95 % für den Testsatz.
>
> Fig.14: Trainings- undValidierungsgenauigkeit des Modells über 30
> Epochen

Fig.15 : Trainings- und Validierungsverlustdes Modells über 30 Epochen

> 54

<img src="./myi1rg25.png"
style="width:1.81861in;height:0.30625in" /><img src="./sculfwwm.png"
style="width:2.49986in;height:2.2175in" /><img src="./wjqbz5of.png"
style="width:2.22222in;height:2.26097in" />

> 6.10.2 Ergebnisse
>
> <img src="./h5k1lqol.png"
> style="width:2.42389in;height:2.25847in" /><img src="./ulrm2nzu.png"
> style="width:2.48167in;height:0.345in" /><img src="./vbuazqy5.png"
> style="width:2.80333in;height:0.39333in" /><img src="./1toxaqhk.png"
> style="width:2.22208in;height:2.31139in" />Es werden vier gängige
> Klassen für Masken definiert (siehe Abb. 25 ). Als Referenz für die
> Ergebnisse werden Foto mit der Laptop Kamera aufgenommen, welche das
> Ergebnis der Identifizierung der verschiedenen Maskentypen zeigt. Die
> Detektion der Gesichtsmaske in Echtzeit, siehe Fig 16 , Fig 17, Fig
> 18, Fig 19.
>
> Fig 16: FFP2-Mask-Erkennung
>
> <img src="./u2nmxhyh.png" style="width:2.56in;height:0.34667in" />Fig
> 18: No-Mask-Erkennung
>
> Fig 17: OP-Mask-Erkennung

<img src="./eid34qat.png"
style="width:2.415in;height:0.34667in" />Fig 19: Nio_Mask Erkennung

*Abbildung* *28:* *Die* *Detektion* *der* *verschiedenen*
*Gesichtsmaske* *in* *Echtzeit.*

> 55

<img src="./tkvccsak.png"
style="width:1.81861in;height:0.30625in" />

> 6.10.3 Diskussion und Ausblick
>
> Einer der Hauptnachteile des Deep Learning, insbesondere des
> überwachten Ler-nens, besteht darin, dass es für das Training auf
> große Mengen von Daten mit menschlichen Anmerkungen angewiesen ist.
> Diese Technik ist nicht in allen Berei-chen anwendbar. Manchmal ist es
> schwierig, große Mengen an professionell an-notierten Daten zu
> erhalten. Das ist zum Beispiel bei diesem Projekt der Fall. Die
> meisten Daten wurden in unbearbeiteter Form gesammelt und mit Hilfe
> eines neuen Tools annotiert, welches die Qualität der Daten noch nicht
> bewiesen hat. Dennoch können damit zufriedenstellende Ergebnisse
> erzielt werden.
>
> Die Fig. 16 ist ein TP (True positive). Denn sie zeigt, dass das
> Modell eine Maske vorhersagt, und diesisteine positive Vorhersage.
> Außerdem wird deutlich, dass das System das Licht als notwendiges
> Erkennungsobjekt betrachtet. Dies wird als fal-sches Positiv(FP)
> bezeichnet. Das Licht ist vorhanden, gehört aber nicht zu dem zu
> erfassenden Objekt oder Element.
>
> Die Erkennungen sindalle korrekt, da sie genau das Ergebnis liefern,
> welches man erwartet. Es wird auch festgestellt, dass das System
> manchmal ein Papier oder ein Tuch für eine Maske hält. Wenn ein Papier
> oder ein Tuch auf das Gesicht gelegt wird, neigt es dazu, es als Maske
> zu erkennen. Diese Erkennung dauert nur 1 Se-kunden oder weniger und
> verschwindet dann. Diese Instabilität der Erkennung ist auch bei
> einigen Anwendungen zu beobachten, z. B. bei der
> [*<u>https://facemask-de-tection.com/</u>*](https://facemask-detection.com/)
> <u>.</u>
>
> 6.10.4 Limite
>
> Die Suche nach frei zugänglichen Datensätzen für diese Arbeit war gar
> nicht so einfach. Es wurde viel Zeit damit verbracht, geeignete
> Gesichtsmaskenbilder zu sammeln und vorzubereiten. Es sind nämlich
> nicht genügend Daten verfügbar. Ins-besondere, um Daten über Personen
> zu finden, die ihre Masken nicht korrekt tra-gen. Selbst die bereits
> verfügbaren Daten werden künstlich erzeugt und sind in der Regel
> verfälscht. Aus diesem Grund ist es schwierig, ein System mit allen
> ge-wünschten Aspekten und Leistungen zu entwickeln.
>
> 56

<img src="./uhaarzpq.png"
style="width:1.81861in;height:0.30625in" />

> **7** **Fazit**
>
> Die Ergebnisse dieser Arbeit sind zufriedenstellend,insbesondere das
> Erkennungs-und Klassifizierungssystem für die verschiedenen
> Maskentypen. Der Ansatz des Deep Learning zur Erkennung von
> Gesichtsmasken funktioniert sehr gut, auch wenn die verfügbaren Daten
> nicht ausreichend sind. Die Vorbereitung war sehr zeit-aufwendig und
> es mussten viele Probleme gelöst werden, welche nichts mit dem Prozess
> zu tun hatten. Die Verarbeitung der Parameter führte jedoch später zu
> sehr guten Ergebnissen. In diesem Projekt wurden moderne Techniken im
> Bereich der Computer Vision und des Deep Learning eingesetzt. Für eine
> effektive Kontrolle der Einhaltung der Maskenpflicht an öffentlichen
> Orten kann dieses System verwendet werden. Natürlich mit weiteren
> Verbesserungen, insbesondere bei der Genauigkeit, aber auch bei der
> Erkennungsgeschwindigkeit. Neben der Benutzerfreundlichkeit sollte
> auch die Sicherheit berücksichtigt werden, da mit den zugewiesenen
> Bildern sensible Daten verfügbar sind.
>
> Es wäre interessant, die Arbeit auf andere Arten von Wetterbedingungen
> auszuwei-ten, wie z. B. das Hinzufügen von Schnee, die Verwendung von
> Kameratypen mit unterschiedlichen Auflösungen (z. B. Infrarotkamera,
> Wärmebildkamera). Dieses Ziel wurde nicht erreicht. Leider wurde diese
> Arbeit mitten in der Covid-19-Pande-mie durchgeführt und die
> Eindämmungsmaßnahmen ließen dies nicht zu.
>
> 57
>
> **8** **References**
>
> \[1\] “3 Convolutional neural networks · Deep Learning for Vision
> Systems,” 7/27/2021,
> https://livebook.manning.com/book/grokking-deep-learning-for-computer-vision/chapter-3/.
>
> \[2\] Q. Zu, B. Hu, N. Gu, et al., eds., *Human* *centered*
> *computing*: *First* *internati-onal* *conference,* *HCC* *2014,*
> *Phnom* *Penh,* *Cambodia,* *November* *27* *-* *29,* *2014* *;*
> *revised* *selected* *papers*, Springer, Cham, 2015.
>
> \[3\] X. Zhou, V. Koltun, and P. Krähenbühl, “Probabilistic two-stage
> detection,” 3/12/2021, https://arxiv.org/pdf/2103.07461.
>
> \[4\] *29th* *IEEE* *Conference* *on* *Computer* *Vision* *and*
> *Pattern* *Recognition*: *CVPR* *2016* *:* *proceedings* *:* *26*
> *June-1* *July* *2016,* *Las* *Vegas,* *Nevada*, IEEE, Pis-cataway,
> NJ, 2016.
>
> \[5\] K. Simonyan and A. Zisserman, “Very Deep Convolutional Networks
> for Large-Scale Image Recognition,” 9/4/2014,
> https://ar-xiv.org/pdf/1409.1556v6.pdf.
>
> \[6\] “ImageNet,” 7/27/2021,
> https://www.image-net.org/challen-ges/LSVRC/2017/index#introduction.
>
> \[7\] H. S, “Activation Functions : Sigmoid, tanh, ReLU, Leaky ReLU,
> PReLU, ELU, Threshold ReLU and Softmax basics for Neural Networks and
> Deep Learning,” *Medium*, 19.01.2019.
>
> \[8\] “Les réseaux de neurones convolutifs,” *Natural* *Solutions*,
> 17.04.2018. \[9\] “Grundlegendes zum Gradientenabstieg und zur
> Adam-Optimierung,”
>
> 13.06.2020.
>
> \[10\]C. Touzet, “LES RESEAUX DE NEURONES ARTIFICIELS, INTRODUC-TION
> AU CONNEXIONNISME,”
> https://hal-amu.archives-ouvertes.fr/hal-01338010/file/Les_reseaux_de_neurones_artificiels.pdf.
> 27.07.2021
>
> \[11\]M. Vinette, “Comment détecter les objets plus efficacement avec
> YOLO,” *Aqsone*, 12.04.2021.
>
> \[12\]J. Redmon, S. Divvala, R. Girshick et al., “You Only Look Once:
> Unified, Real-Time Object Detection,” in *29th* *IEEE* *Conference*
> *on* *Computer* *Vision* *and* *Pattern* *Recognition*: *CVPR* *2016*
> *:* *proceedings* *:* *26* *June-1* *July* *2016,* *Las* *Vegas,*
> *Nevada*, IEEE, Piscataway, NJ, 2016.
>
> \[13\]“The PASCAL Visual Object Classes Challenge 2007 (VOC2007),”
> 1/1/2019, http://host.robots.ox.ac.uk/pascal/VOC/voc2007/index.html.
>
> \[14\]V. Feng, “An Overview of ResNet and its Variants - Towards Data
> Science,” *Towards* *Data* *Science*, 15.07.2017.
>
> \[15\]“Die Macht des Transferlernens im Deep Learning,” 12.07.2021.
>
> \[16\]B. Bhavya Sree, V. Yashwanth Bharadwaj, and N. Neelima, “An
> Inter-Com-parative Survey on State-of-the-Art Detectors—R-CNN, YOLO,
> and SSD,” in *Intelligent* *Manufacturing* *and* *Energy*
> *Sustainability*: *Proceedings* *of* *I-CIMES* *2020,* A. Reddy, D.
> Marla, M. N. Favorskaya et al., Eds., pp. 475– 483, Springer
> Singapore; Imprint: Springer, Singapore, 2021.
>
> \[17\]“Echtzeit-Objekterkennung mit YOLO, YOLOv2 und jetzt YOLOv3,”
> 26.11.2020
> https://ichi.pro/de/echtzeit-objekterkennung-mit-yolo-yolov2-und-jetzt-yolov3-44743782178952.
>
> \[18\]“3 Introduction to Keras and TensorFlow · Deep Learning with
> Python, Se-cond Edition MEAP V07,” 9/26/2021,

<img src="./0pwaw5hw.png"
style="width:1.81861in;height:0.30625in" />

> https://livebook.manning.com/book/deep-learning-with-python-second-edi-tion/chapter-1/v-7/129.
>
> \[19\]JetBrains, “Integrierte Entwicklertools – Features \| PyCharm,”
> 9/26/2021,
> https://www.jetbrains.com/de-de/pycharm/features/tools.html.
>
> \[20\]“Anaconda \| Pyston Team Joins Anaconda to Expand Open-Source
> Pro-ject…,” 9/26/2021,
> https://www.anaconda.com/blog/pyston-team-joins-ana-conda.
>
> \[21\]G. Serebryakov, “OpenCV-Python for Apple’s M1 Chip: A Detective
> Story With A Happy Ending,” *OpenCV*, 26.07.2021.
>
> \[22\]“Der Viola-Jones-Gesichtserkennungsalgorithmus,” 09.03.2020.
> \[23\]PyImageSearch, “Face detection with dlib (HOG and CNN) -
>
> PyImageSearch,” 4/17/2021,
> https://www.pyimagesearch.com/2021/04/19/face-detection-with-dlib-hog-and-cnn/.
>
> \[24\]GitHub, “ageitgey/face_recognition,” 1/26/2021,
> https://gi-thub.com/ageitgey/face_recognition#face-recognition.
>
> \[25\]S. Singh and F. Nasoz, “Facial Expression Recognition with
> Convolutional Neural Networks,” *2020* *10th* *Annual* *Computing*
> *and* *Communication* *Workshop* *and* *Conference* *(CCWC)*, pp.
> 324–328, 2020.
>
> \[26\]S. Singh and F. Nasoz, “Facial Expression Recognition with
> Convolutional Neural Networks,” in *2020* *10th* *Annual* *Computing*
> *and* *Communication* *Workshop* *and* *Conference* *(CCWC)*, pp.
> 324–328, 2020.
>
> \[27\]K. C. Kirana, S. Wibawanto, and H. W. Herwanto, “Redundancy
> Reduction in Face Detection of Viola-Jones using the Hill Climbing
> Algorithm,” in *2020* *4th* *International* *Conference* *on*
> *Vocational* *Education* *and* *Training* *(ICO-VET)*, pp. 139–143,
> 2020.
>
> \[28\]PyImageSearch, “Face recognition with OpenCV, Python, and deep
> learn-ing - PyImageSearch,” 7/13/2021,
> https://www.pyimagese-arch.com/2018/06/18/face-recognition-with-opencv-python-and-deep-learn-ing/.
>
> \[29\]M. S. Ejaz and M. R. Islam, “Masked Face Recognition Using
> Convolutional Neural Network,” in *2019* *International* *Conference*
> *on* *Sustainable* *Techno-logies* *for* *Industry* *4.0* *(STI)*, pp.
> 1–6, IEEE, 24.12.2019 - 25.12.2019.
>
> \[30\]S. Sethi, M. Kathuria, and T. Kaushik, “Face mask detection
> using deep learning: An approach to reduce risk of Coronavirus
> spread,” *Journal* *of* *Biomedical* *Informatics*, vol. 120, p.
> 103848, 2021.
>
> \[31\]“Der Viola-Jones-Gesichtserkennungsalgorithmus,” 09.03.2020.
>
> \[32\]M. Sandler, A. Howard, M. Zhu et al., “MobileNetV2: Inverted
> Residuals and Linear Bottlenecks,” *The* *IEEE* *Conference* *on*
> *Computer* *Vision* *and* *Pattern* *Recognition* *(CVPR)*.
>
> \[33\]P. Mitra, “COVID Face Mask Detection Dataset,” 7/15/2020,
> https://www.kaggle.com/prithwirajmitra/covid-face-mask-detection-dataset.
>
> \[34\]GitHub, “GitHub - akashkam559/Covid19-Face-Mask-Detector:
> Covid19 Face Mask Detector,” 9/1/2021,
> https://github.com/akashkam559/Covid19-Face-Mask-Detector.
>
> \[35\]KDnuggets, “How to Implement a YOLO (v3) Object Detector from
> Scratch in PyTorch: Part 1 - KDnuggets,” 7/27/2021,
> https://www.kdnuggets.com/2018/05/implement-yolo-v3-object-detector-py-torch-part-1.html.
>
> 59

<img src="./fctodxuj.png"
style="width:1.81861in;height:0.30625in" />

> \[36\]S. Weidman and J. W. Lang, *Deep* *Learning* *-* *Grundlagen*
> *und* *Implemen-tierung*: *Neuronale* *Netze* *mit* *Python* *und*
> *PyTorch* *programmieren*, O'Reilly, Heidelberg, 2020.
>
> \[37\]T. Q. Vinh and N. T. N. Anh, “Real-Time Face Mask Detector Using
> YOLOv3 Algorithm and Haar Cascade Classifier,” in *2020*
> *International* *Conference* *on* *Advanced* *Computing* *and*
> *Applications* *(ACOMP)*, pp. 146– 149, 2020.
>
> \[38\]“IEEE Xplore Full-Text PDF,” 7/28/2021,
> https://ieeex-plore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9353070.
>
> \[39\]B. Batagelj, P. Peer, V. Štruc et al., “How to Correctly Detect
> Face-Masks for COVID-19 from Visual Information?,” *Applied*
> *Sciences*, vol. 11, no. 5, p. 2070, 2021.
>
> \[40\]Shiming Ge, Jia Li, Qiting Ye et al., “Detecting Masked Faces in
> the Wild with LLE-CNNs,” *undefined*, 2017.
>
> \[41\]J. Redmon, “Survival Strategies for the Robot Rebellion,”
> 7/28/2021, https://pjreddie.com/.
>
> \[42\]J. Redmon, “YOLO: Real-Time Object Detection,” 9/1/2021,
> https://pjred-die.com/darknet/yolo/.
>
> \[43\]GitHub, “GitHub - AlexeyAB/darknet: YOLOv4 / Scaled-YOLOv4 /
> YOLO -Neural Networks for Object Detection (Windows and Linux version
> of Dark-net ),” 9/1/2021, https://github.com/AlexeyAB/darknet.
>
> \[44\]S. Kumar, “Data Augmentation Increases Accuracy of your model —
> But how ?,” *Secure* *and* *Private* *AI* *Writing* *Challenge*,
> 21.07.2019.
>
> \[45\]Mengyue Geng, Peixi Peng, Yangru Huang et al., “Masked Face
> Recogni-tion with Generative Data Augmentation and Domain Constrained
> Ran-king,” *undefined*, 2020.
>
> 60

<img src="./ta3o0tyt.png"
style="width:1.81861in;height:0.30625in" /><img src="./qrsimdln.png"
style="width:6.10278in;height:2.90764in" /><img src="./1klhd0jd.png"
style="width:6.14028in;height:3.84861in" />

> **Anhang**
>
> Screenshot der Übersicht über den Code
>
> **Anhang** **1**: Gesichtserkennung
>
> **Anhang** **2** : Gesichtsmasken-Erkennung
>
> 61

