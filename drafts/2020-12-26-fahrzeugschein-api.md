---
layout: post
title:  "Fahrzeugschein auslesen mittels Künstlicher Intelligenz"
subtitle: "Unsere Künstliche Intelligenz digitalisiert Fahrzeugscheine und optimiert Ihre Prozesse."
excerpt: >-
    Unsere Künstlicher Intelligenz digitalisiert Fahrzeugscheine innerhalb weniger Sekunden. Durch
    einen zweistufigen Ansatz erreichen werden dabei Genauigkeiten, die die Ergebnisse einer herkömmlicher Texterkennung deutlich übersteigen.
date: 2020-12-26
thumb_img_path: images/glenn-carstens-peters-npxXWgQ33ZQ-unsplash.jpg
---

Ob in der Autowerkstatt oder in der Versicherung: Täglich werden in Deutschland tausende von Fahrzeugscheinen erfasst und digitalisiert. Dieser Prozess ist aufwendig und birgt Fehlerpotenzial. Digitalisierung stellt an dieser Stelle eine Lösung dar. Allerdings ist die Erfassung eines Fahrzeugscheines mitteles herkömmlicher Texterkennung eine Herausforderung. In diesem Blogbeitrag stellen wir am Beispiel der Fahrzeugscheinerkennung einen Ansatz vor, wie komplexe Texterkennungsaufgaben bei strukturierten Dokumenten mittels Künstlicher Intelligenz gelöst werden können.

# Dreistufiger Erkennungsansatz für optimales Auslesen von Fahrzeugscheinen.

Der Mensch kann den Fahrzeugschein (wenn er diesen zuvor studiert hat oder dieser bekannt ist) einfach erfassen. Woran liegt das? Der Fahrzeugschein ist ein strukturiertes Dokument. Jede Angabe hat seinen festen Platz. Beispielsweise ist für das Kennzeichen ein Feld vorgegeben. Dieses befindet sich relativ gesehen immer an derselben Stelle auf dem Fahrzeugschein. Zudem weist ein Kennzeichen eine semantische Struktur auf. Diese Tatsachen haben wir uns bei der Entwicklung der Künstlichen Intelligenz zum Vorteil gemacht und einen mehrstufigen Erkennungs- und Analyseprozess implementiert.

1. **Lokalisierung relevanter Positionen** Mithilfe eines deep-learning Object Detection Modells werden relevante Positionen ermittelt. Object Detection ist eine Methode aus dem Gebiet Computer Vision. Mithilfe von Object Detection lassen sich Objekte auf Bildern lokalisieren und mittels eine Begrenzungsrahmen markieren. In unserem speziellen Fall sind die "Objekte" die auszulesenden Felder auf dem Fahrzeugschein. Das Modell ist dabei in einem Transferleaning Ansatz auf synthetisch erzeugten Bildern trainiert worden, die zuvor manuell gelabelt wurden. Labeln bedeutet, dass manuell ein Trainingsdatensatz erzeugt werden muss, auf dem die Positionen der Objekte markiert sind. Nach Abschluss des Trainingsprozesses wurde das Object Detection Modell auf einem unabhängigen Testdatensatz evaluiert. Die Lokalisierungsaufgabe konnte dabei vom Modell extrem gut gelernt werden. Auf real-world Bildern generalisiert das Modell bei Fahrzeugscheinen sehr gut (Accuracy der Lokalisierungsaufgabe von über 98,5 %).

2. **Auslesen der relevanten Positionen** Auf Basis der lokalisierten Positionen werden speziell die erkannten Bildbereiche durch eine Texterkennung digitalisiert. Dadurch enstehen zwei Vorteile: 1. Je auzulesendem Feld wird nur der Text ausgelesen, der auch zur entsprechenden Position gehört. 2. Aufgrund Lokalisierung muss nicht der gesamte Fahrzeugschein ausgelesen werden, sondern nur die zugeschnittenen Bereiche, wodurch eine effiziente Auslesung gewährleistet werden kann.

3. **Semantische Analyse und Verrifikation** Die ausgelesenen Texte werden weiter regelbaisert ausgewertet. Beispielsweise erfolgt beim Auslesen der Anschrift ein Abgleich mit einer Datenbank mit Postleitzahlen oder bei der Fahrzeugidentifizierungsnummer erfolgt ein Quercheck zum Feld des Herstellers. Durch die semantische Analyse und Verrifikation wird sichergestellt, dass keine falschen Ergebnisse von der Künstlichen Intelligenz zurückgeliefert werden.

# Bereitstellung mithilfe von Fast-API und Kubernetes.
Die Bereitstellung der Künstlichen Intelligenz erfolgt über eine REST-Schnittstelle. Dafür wurde das Python-Modul Fast-API verwendet. Fast-API bietet den Vorteil, das eine Automatisierte Dokumentation erstellt wird. Die Dokumentation unserer Fahrzeugscheinerkennung können sie [hier](https://api.mmmint.ai/fahrzeugschein/v1/docs) einsehen. ... Kubernetes ...


# More about mmmint

Analog zur Auslesung von Fahrzeugscheinen kann unsere Methodik auch zur digitalen Erfassen von anderen sturkturierten Dokumenten verwendet werden, wenn extrem hohe Genauigkeiten gefordert sind. Sie müssen Dokumente strukturiert erfassen? Sprechen Sie uns gerne an.

1. [Facebook](https://www.facebook.com/mmmintai/)
2. [Instagram](https://instagram.com/mmmint.ai/)
3. [Twitter](https://twitter.com/mmmint_ai/)
4. [Linkedin](https://linkedin.com/company/mmmint-ai/)
5. [GitHub](https://github.com/mmmint-ai/)
