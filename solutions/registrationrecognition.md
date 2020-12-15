---
title: Fahrzeugschein Erkennung
subtitle: Mithilfe unserer Fahrzeugscheinerkennung können Sie ihre Fahrzeugscheine automatisiert auslesen. 
sections:
  - section_id: registrationrecognition
    component: features_block.html
    type: featuresblock
    bg: gray
    featureslist:
      - title: Künstliche Intelligenz zur Optimierung Ihrer Prozesse
        image: images/product_registration_recognition.png
        content: >-
          Mithilfe unserer Fahrzeugscheinerkennung können Sie ihre Fahrzeugscheine automatisiert auslesen. 
          <br/><br/>
          Wir verwenden deep-learning-based Object Detection und Texterkennung um die Fahrzeugscheine zu verarbeiten. Um eine sehr hohe Genauigkeit zu erreichen, wurde unsere Künstliche Intelligenz mit mehreren Tausend Bildern angelernt. Folgende Postitionen kann unsere Künstliche Intelligenz automatisiert extrahieren:

          * Vorname und Nachname

          * Anschrift

          * Kennzeichen

          * FIN

          * Nächste HU und Erstzulassung

          * Codehersteller und Codetyp
    actions:
      - label: Go To API
        url: /solutions/fahrzeugschein.html

  - section_id: call-to-action
    component: cta_block.html
    type: ctablock
    title: Jetzt Demo anfordern!
    subtitle: Schicken Sie uns eine E-Mail und erhalten Sie eine Teststellung zu unserer Fahrzeugschein Erkennung.
    actions:
      - label: Get Started
        url: 'mailto:info@mmmint.ai'
  - section_id: pricing
    component: pricing_block.html
    type: pricingblock
    bg: gray
    title: Pricing Plans
    subtitle: Wir bieten verschiedene Preismodelle an. 
    pricingplans:
      - title: Basic
        price: €300/m
        details: |-
          * 1000 Bilder inklusive,
          * dann €0.15 pro Bild
          * Volle Fahrzeugschein Digitalisierung
          * Bereistellung der API Spezifikation
        actions:
          - label: Order Now
            url: mailto:info@mmmint.ai
      - title: Professional
        price: €500/m
        details: |-
          * 2000 Bilder inklusive,
          * dann €0.08 pro Bild
          * Support: 24 Stunden Reaktionszeit
          * Volle Fahrzeugschein Digitalisierung
          * Fahrzeugschein Overlay
          * Einführung in die API Spezifikation
          * Einführung in Python SDK
        highlight: true
        actions:
          - label: Order Now
            url: mailto:info@mmmint.ai
      - title: Enterprise
        price: individuell
        details: |-
          * Volle Fahrzeugschein Digitalisierung
          * Individuelle Vertragsvereinbarung
        actions:
          - label: Order Now
            url: mailto:info@mmmint.ai
  - section_id: faq
    component: faq_block.html
    type: faqblock
    bg: gray
    title: Frequently Asked Questions
    subtitle: Hier sind die meist gestellten Fragen
    faqitems:
      - question: Wie kann ich die Fahrzeugschein API benutzen? 
        answer: >-
          For usage of the registration recognition API an APIKey (`access_token`) is required.
          Please get in contact with us to request a test environment.
          <br/>
          For support reach out to [info@mmmint.ai](mailto:info@mmmint.ai). 
      - question: Wird die DSGVO eingehalten?
        answer: >-
          The provided service is hosted in german datacenters. Submitted data is encrypted in transit and at rest. The submitted date can only be accessed using the used APIKey.
      - question: Wie funktioniert die Fahrzeugschein API?
        answer: >-
          For support reach out to [info@mmmint.ai](mailto:info@mmmint.ai). For usage of the registration recognition API an APIKey (`access_token`) is required.

            1. In order to use the registration recognition API you start by submitting an image via file upload, or with a publicly accessible image of the registration, using a POST to `/fahrzeugschein`.
            2. The asynchronous processing of the the recognition can be checked using the `/fahrzeugschein/status/` {sessionId} resource.
            3. After the status is finished, the recognized data can be retrieved using `/fahrzeugschein/{id}` resource.
            4. The bounding boxes and associated cropped images can be retrieved using the `/detection` resources.
            5. To retrieve all sessions for the submitted registration use the `/session` resource. The sessions will also indicate the status of all submissions.

layout: features
---
