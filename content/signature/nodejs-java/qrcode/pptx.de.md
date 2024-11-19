



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: de
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "QR-Codes in PPTX-Dokumenten mit JavaScript erstellen"
head_description: "Nutzen Sie die GroupDocs.Signature-API, um 2D-Barcodes in PPTX-Dateien zu erstellen und zu integrieren. Platzieren Sie QR-Codes mühelos auf jeder Seite des Dokuments."

############################# Header ############################
title: "QR-Codes für PPTX erstellen" 
description: "Erstellen und integrieren Sie 2D-Barcodes mit anpassbarem Inhalt, einschließlich Text und numerischen Daten, in verschiedenen Dokumenttypen wie PDFs, Word, Excel und Bilder mit GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt kostenlos testen"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java-Funktionen entdecken"
    link: "/signature/nodejs-java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) bietet fortschrittliche Dokumentenverbesserungswerkzeuge, mit denen die Erstellung und Einbettung mehrerer Signaturtypen, einschließlich QR-Codes, in gängige Dateiformate möglich ist. Signieren und sichern Sie PDFs, Word-Dokumente, Excel-Tabellen, PowerPoint-Präsentationen und Bilder mit Text-, Bild-, Barcode-, QR-Code-, Metadaten-, Digital- und Stempelsignaturen.

############################# Steps ############################
steps:
    enable: true
    title: "Leitfaden zur Erstellung und Einbettung eines QR-Codes an beliebiger Stelle in einem PPTX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ermöglicht die Erstellung von QR-Codes in verschiedenen verbreiteten Formaten und deren Integration in PPTX-Seiten. Unterstützen Sie über 10 verschiedene QR-Code-Typen, kann unsere Lösung nahtlos in Node.js via Java-Anwendungen integriert werden, um diese mit QR-Code-Signierungsfunktionen zu bereichern.
      
      1. Stellen Sie die PPTX-Datei oder den Stream für die QR-Code-Signatur bereit.
      2. Geben Sie den gewünschten Text in die QrCodeSignOptions-Instanz ein.
      3. Passen Sie visuelle Einstellungen wie Farbe, Positionierung, Größe usw. an.
      4. Speichern Sie das Dokument mit dem QR-Code.
   
    code:
      platform: "nodejs-java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Beispielunterschriften"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "Klicken zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Erstellen Sie eine Signature-Instanz und übergeben Sie den Dokumentenpfad.
        const signature = new signatureLib.Signature('input.pptx');

        // Nutzen Sie QrCodeSignOptions, um einen QR-Code in das Dokument einzufügen.
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Definieren Sie den Signaturtyp und den Platzierungsort auf der Seite.
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Speichern Sie das Dokument mit dem neu hinzugefügten QR-Code.
        signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Umfassende Integration von Signaturen und QR-Codes"
  description: "Mit der GroupDocs.Signature for Node.js via Java-API können Sie ein breites Spektrum von Signaturen verwalten. Generieren, anpassen, verifizieren, suchen und entfernen Sie Signaturen mühelos in verschiedenen Dokumenttypen und bieten Sie unübertroffene Flexibilität für Ihre Workflows."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Funktionen für Signaturen und QR-Codes"
  features:
    # feature loop
    - title: "Dokumentensignierung in mehreren Formaten"
      content: "Fügen Sie verschiedene Arten von Signaturen hinzu, einschließlich Text-, Bild-, Barcode-, QR-Code- und Stempelsignaturen, zu jedem unterstützten Dateiformat. Platzieren Sie sie auf jeder Seite und verwalten Sie die Dokumentenmetadaten. Stellen Sie die Dokumentensicherheit durch digitale Zertifikate sicher, um unbefugte Änderungen zu verhindern."

    # feature loop
    - title: "Effiziente Signaturvalidierung"
      content: "Überprüfen Sie alle Signaturen innerhalb eines Dokuments, um sicherzustellen, dass sie den erforderlichen Standards entsprechen. Holen Sie sich mühelos Signaturen über die integrierte Suchfunktion."

    # feature loop
    - title: "Flexible Signaturbearbeitung"
      content: "Aktualisieren oder ändern Sie vorhandene Signaturen, indem Sie Aspekte wie Inhalt, Standort, Größe und Farbe anpassen, um den Anforderungen Ihres Dokuments nach der ursprünglichen Unterzeichnung zu entsprechen."

    # feature loop
    - title: "Einfaches Entfernen von Signaturen"
      content: "Entfernen Sie unerwünschte oder veraltete Signaturen, einschließlich digitaler Zertifikate, mühelos. Volle Kontrolle über die Signaturverwaltung sorgt für ein sauberes und gut organisiertes Dokument."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Anpassung eines generierten QR-Codes"
      content: |
        Dieses Beispiel beschreibt den Prozess, um einen angepassten QR-Code auf einer PPTX-Seite hinzuzufügen.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Holen Sie sich das Dokument, das signiert werden soll, und übergeben Sie es an Signature.
          const signature = new signatureLib.Signature('input.pptx');

          // Richten Sie die QR-Code-Optionen mit dem erforderlichen Text ein.
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Bestimmen Sie die Position des QR-Codes auf der Seite.
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Geben Sie den Abstand der Signatur an.
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Wählen Sie die Farbe des QR-Codes.
          signOptions.setForeColor(signatureLib.Color.RED);

          // Definieren Sie die Schriftartoptionen für die begleitende Nachricht.
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Passen Sie die Hintergrundfarbe und den Pinsel für den QR-Code an.
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Fügen Sie den QR-Code in das Dokument ein.
          signature.sign('output.pptx', signOptions);
          ```
        platform: "nodejs-java"
        copy_title: "Kopieren"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "Klicken zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pptx"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "NPM herunterladen"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Verstehen Sie unsere Hauptfunktionen"
    exclude: "qrcode"
    description: "Wir bieten eine breite Auswahl an Signaturformaten und -operationen, die auf Ihre Bedürfnisse zugeschnitten sind."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/nodejs-java/text/pptx/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/nodejs-java/image/pptx/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/nodejs-java/search/pptx/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pptx/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "QR-Codes in verschiedenen Dateiformaten integrieren"
    exclude: "PPTX"
    description: "Nutzen Sie die Node.js via Java-API, um QR-Codes zu generieren und in eine Vielzahl von weithin verwendeten Dateiformaten einzubetten. Kapseln Sie wichtige Daten in diesen Barcodes für nahtlose Integration und zukünftige Abrufbarkeit."
    items: 
          
        # format loop 1
        - name: "QR-Code für PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "QR-Code für DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "QR-Code für JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "QR-Code für PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "QR-Code für XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---