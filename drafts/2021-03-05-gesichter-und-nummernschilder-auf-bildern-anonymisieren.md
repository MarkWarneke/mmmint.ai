---
title: Bilder Anonymisieren.
subtitle: >-
  Mit der Anwendung von Künstlicher Intelligenz automatisiert Kennzeichen und Gesichter in Bildern anonymisieren.
excerpt: >-
  Visuelle Medien nehmen einen zunehmenden Stellenwert in einer digitalisierten Welt ein. Immer mehr Plattformen integrieren das Hochladen von Bilddateien. Dabei können datenschutzrechliche Risiken durch den Upload von Bildern entstehen. Unsere Künstliche Intelligenz anonymisiert Bilder für diverse Anwendungsszenarien.
date: '2021-03-05'
time: 2 Minute
thumb_img_path: images/solutions/anonymizer/undraw_both_sides_hbv3.png
share-img: images/solutions/anonymizer/undraw_both_sides_hbv3.png
layout: post
compare:
  city:
    inline: true
    image:
      left:
        src: /images/solutions/anonymizer/city-original.jpg
        alt: Original
      right:
        src: /images/solutions/anonymizer/city-blurred.jpg
        alt: Anonymisiert
  m4:
    image:
      left:
        src: /images/solutions/anonymizer/m4-original.jpg
        alt: Original
      right:
        src: /images/solutions/anonymizer/m4-blurred.jpg
        alt: Anonymisiert
---

Visuelle Medien nehmen einen zunehmenden Stellenwert in einer digitalisierten Welt ein. Immer mehr Plattformen integrieren das Hochladen von Bilddateien. Dabei können datenschutzrechliche Risiken durch den Upload von Bildern entstehen. Diese sollten anonymisiert werden. Die manuelle Anonymisierung ist mit einem hohem Zeitaufwand verbunden, insbesondere wenn es sich um Videos, sowie Serienaufnahmen handelt. Unsere Künstliche Intelligenz setzt an dieser Problemstellung an und automatisiert den Prozess der Anonymisierung.

![Anonymized demo face and car](/images/solutions/anonymizer/2314f3fed78c77b29373568b0740aac2124dab9150c8247c15ff7be374baa262.jpg)

Der [<mark>Anonymizer-Service</mark>](/solutions/anonymizer/) kann für diverse Anwendungsszenarien operationalisiert werden. Dies schließt z. B. die Anonymisierung von Datensätzen für die Entwicklung von selbstfahrenden Autos, die Anonymisierung von virtuellen Rundgängen auf Google-Maps oder Produktfotos auf Plattformen wie Ebay-Kleinanzeigen oder mobile.de ein. Aber auch bewegte Bilder wie TV-Medien lassen sich mithilfe unserer Künstlichen Intelligenz anonymisieren.

## Wie funktioniert unsere Künstliche Intelligenz?

Mithilfe von Deep Learning werden personenbezogene Inhalte in Bildern lokalisiert. Durch die Verwendung von State-of-the-Art Computer Vision lässt sich eine zuverlässige Lokalisierung der personenbezogenen Inhalte gewährleisten. Dafür wurden zunächst große Datenmengen (teils öffentlich Zugänglich, teils synthetisch erzeugte Daten) verwendet, um die Deep Learning Modelle von mmmint.ai zu trainieren. In unserem Service werden mehrere Deep-Learning Modelle orchestriert und je nach Konfiguration des Services angesprochen. 

Es steht Ihnen frei, ob Sie mit unserem SaaS Gesichter und/oder Kennzeichen auf Fotos automatisiert unkenntlich machen möchten. Zur Anonymisierung stehen verschiedene Möglichkeiten zur Verfügung. Der Bereich lässt sich verpixeln, verdecken oder auch deformieren. Für Marketingzwecke ist insbesondere die Verdeckung mit einem individualisierten Logo interessant. In urbanen Szenarien und Bildern mit "chaotischen Momentaufnahmen und Zuständen" liefert z. B. der Blurr-Effekt ein ästhetisches Ergebnis, wie folgender Vorher-Nachher-Vergleich zeigt:

 {% include image_compare_block.html section=page.compare.city %}

Sowohl die Person zwischen den Autos, obwohl Sie nicht direkt in die Kamera blickt, als auch das Nummernschild des roten SUVs werden von unserer Künstlichen Intelligenz automatisiert und erkannt und anonymisiert. Das Bild verliert dabei nicht an Aussagekraft und die sensiblen Daten werden entfernt. Datenschutz sollte Sie nicht daran hindern Ihr Bildmaterial für Marketingzwecke effizient zu verwenden - nutzen Sie unseren Service, um in Echtzeit Ergebnisse erzielen zu können.

## Wie kann ich den Anonymizer-Service nutzen?

Die Einbinung des Anonymizer-Service in Ihre Systeme ist dank einer standardisierten Schnitstelle einfach und schnell möglich. Aktuell wird der [<mark>Anonymizer-Service</mark>](/solutions/anonymizer/) als REST-API zur Verfügung gestellt und bietet Entwicklern damit einen einfachen Zugang zu unserer Künstlichen Intelligenz. [Hier finden Sie unsere Dokumentation](/solutions/anonymizer_api.html)

Das Frontend für den Upload von Bildern & Videomaterial befindet sich aktuell in der Entwicklung. Sie möchten mit Ihrem Anwendungsfall einen Pilot mit uns starten? Sprechen Sie uns gerne an! Wir freuen uns auf einen Austausch und sind gespannt auf Ihren Anwendungsfall.

> "Hier sehen Sie einen Auszug aus der Plattform Ebay Kleinanzeigen. Wir sind uns sicher, das geht auch leichter."

![Opel Zafira manuelle Anoymisierung von Auto Kennzeichen](/images/solutions/anonymizer/opel_zafira_crop.jpeg)

<section id="call-to-action" class="block cta-block bg-accent outer">
  <div class="inner-large">
    <div class="grid">
      <div class="cell block-content">
        <h2 class="block-title">Jetzt Zeit sparen...</h2>
      </div><!-- .block-content -->
      <div class="cell block-buttons">
        <a href="mailto:info@mmmint.ai" class="button white large">... und eine Demo anfordern!</a>
      </div><!-- .block-buttons -->
    </div><!-- .grid -->
  </div><!-- .inner -->
</section>

### Quellen

- [Audi: Audi TT RS 2019](audi.com)
- [Unsplash: City](https://unsplash.com/photos/jViepQKI01Q)
- [Unbekannt: Opel Zafira](https://www.langweiledich.net/bilderparade-dlvi/3/#DLVI_74)
