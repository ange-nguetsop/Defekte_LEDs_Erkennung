# Defekte_LEDs_Erkennung

## Introduction

In einem ständig wandelnden technologischen Umfeld ist die Anpassung an innovative Entwicklungen von entscheidender Bedeutung, um am Fortschritt teilzuhaben. Das Jahr 2023 markierte einen Wendepunkt im Wachstum der künstlichen Intelligenz (KI) und ihrer Integration in verschiedene Lebensbereiche. Dieses Dokument zielt darauf ab, die Anwendung von maschinellem Lernen (Machine Learning, ML) zur Identifizierung und Lösung potenzieller Störungen in industriellen Produktionsprozessen zu untersuchen, was die Betriebseffizienz steigert.

Der Schwerpunkt des Projekts liegt auf der automatischen Erkennung defekter Leuchtdioden (LEDs) auf Lichtleisten. Während ein menschlicher Beobachter eine fehlerhafte LED unter ihren funktionierenden Pendants auf einem Bild leicht erkennen kann, stellt sich die Frage, ob eine Maschine mittels eines künstlichen Sehsystems ähnliche Unterscheidungen treffen kann. Diese Herausforderung wirft die Möglichkeit auf, einer Maschine die Fähigkeit zu verleihen, eine defekte LED in einem funktionierenden Set zu identifizieren, ein Thema, das im weiteren Verlauf dieses Dokuments vertieft wird.


## Datenerfassung und -vorbereitung

Im Bereich des maschinellen Lernens sind die Datenerfassung und -vorbereitung grundlegende Schritte von höchster Bedeutung. Ein fortschrittliches maschinelles Lernmodell ist durch die Qualität seines Datensatzes begrenzt. Daher ist es unerlässlich, eine sorgfältige Datensammlung und -annotation durchzuführen. Für dieses Projekt wurden etwa 500 Bilder gesammelt, was eine robuste Datenbasis bildet.

Die Annotation wurde mit Hilfe von Roboflow durchgeführt, einem anerkannten Werkzeug, das die Datenetikettierung und das Training von Modellen, die für spezifische Probleme geeignet sind, erleichtert. Diese Wahl war aufgrund der Effektivität von Roboflow in diesem Bereich selbstverständlich. Nach der Annotation wurden die Daten in drei separate Sets aufgeteilt: 70\% für das Training, 15\% für die Validierung und 15\% für Tests. Diese Daten wurden anschließend für das Training mit dem YOLOv5-Modell importiert.

Für weitere Informationen über Roboflow und YOLOv5 wird empfohlen, deren jeweilige Websites zu konsultieren

## Modelltraining mit Yolov5

Das Training des Modells erfolgte gemäß den detaillierten Anleitungen von Roboflow, die in ihrer offiziellen Dokumentation zugänglich sind. 

## Konfusionsmatrix
Die Analyse der Konfusionsmatrix hat gezeigt, dass das Modell in der Lage ist, defekte LEDs mit einer Genauigkeit von 99,0\% unter einem Set funktionierender LEDs zu identifizieren.
![Alt](https://github.com/ange-nguetsop/Defekte_LEDs_Recognition/blob/main/ConfusionMatrixLED.png)

## Ergebnis 
Die nach dem Training erzielten Ergebnisse demonstrieren die Zuverlässigkeit und Effektivität des Modells bei der Erkennung defekter LEDs und unterstreichen somit das Potenzial des maschinellen Lernens bei der Optimierung industrieller Prozesse.
![Alt](https://github.com/ange-nguetsop/Defekte_LEDs_Recognition/blob/main/Result.png)

## Anwendung
Ein solches Bildverarbeitungssystem, das auf der Analyse von Bildern aus einem spezifischen Verzeichnis basiert, könnte in der Automobilindustrie eine hochgradig innovative und effiziente Anwendung finden, insbesondere im Kontext der Qualitätssicherung und Funktionsprüfung von LED-basierten Beleuchtungssystemen in Fahrzeugen.

In der modernen Automobilherstellung sind LED-Leuchtsysteme aufgrund ihrer hohen Effizienz, Langlebigkeit und der Möglichkeit zur Realisierung komplexer Beleuchtungsmuster weit verbreitet. Diese Systeme spielen eine entscheidende Rolle in Bezug auf die Sicherheit, Ästhetik und Funktionalität der Fahrzeuge. Dementsprechend ist es von äußerster Wichtigkeit, sicherzustellen, dass jede einzelne LED innerhalb dieser Systeme fehlerfrei funktioniert, um die Einhaltung strenger Qualitätsstandards zu gewährleisten.

Ein automatisiertes Bildverarbeitungssystem könnte in diesem Kontext eingesetzt werden, um die Integrität und Funktionalität jedes LED-Elements innerhalb eines Fahrzeugs zu überprüfen. Durch die Analyse von Bildern der beleuchteten LED-Systeme könnte das System Unregelmäßigkeiten wie nicht funktionierende LEDs. 
