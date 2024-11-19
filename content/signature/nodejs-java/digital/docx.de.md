



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:18
draft: false
lang: de
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Digitale elektronische Signaturen zu DOCX-Dateien mit JavaScript hinzufügen"
head_description: "Fügen Sie einer DOCX-Datei mit JavaScript in nur wenigen Codezeilen eine digitale Signatur hinzu. Verwenden Sie GroupDocs.Signature for Node.js via Java, um zahlreiche Dateiformate zu signieren."

############################# Header ############################
title: "DOCX mit digitalen Zertifikaten schützen" 
description: "Sichern Sie Ihre Geschäftsdokumente, indem Sie digitale Zertifikate mit den erweiterten Funktionen von GroupDocs.Signature for Node.js via Java einbetten. Wir bieten flexible Optionen zum Schutz und zur Authentifizierung Ihrer Dokumente."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ist eine umfassende Lösung zum Signieren, die entwickelt wurde, um eine Vielzahl von Dokumentenverarbeitungsbedürfnissen zu erfüllen. Es ermöglicht Ihnen, Text, Bilder, digitale Zertifikate und Stempel in über 60 verschiedene Dateiformate, einschließlich PDF, MS Office, Bilder und ZIP-Dateien, einzufügen. Darüber hinaus können signierte Dokumente bei Bedarf einfach durchsucht, überprüft, bearbeitet oder gelöscht werden.

############################# Steps ############################
steps:
    enable: true
    title: "Richtlinien zum Sichern von DOCX mit digitalen Zertifikaten in JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ermöglicht Entwicklern von Node.js via Java, DOCX-Dokumente vor Änderungen durch digitale Signaturen zu schützen. Verbessern Sie Ihre Geschäftsanwendungen mit umfassenden Datensicherheitsfunktionen.
      
      1. Übergeben Sie das DOCX-Dokument an den Konstruktor der Signature-Klasse.
      2. Wenden Sie ein digitales Zertifikat und das entsprechende Passwort an, um das Dokument zu sichern.
      3. Fügen Sie gegebenenfalls eine visuelle Darstellung der digitalen Signatur auf den Dokumentseiten hinzu.
      4. Signieren Sie das Dokument, um zukünftige Änderungen zu verhindern.
   
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

        // Verwenden Sie Signature, um eine digitale Signatur auf das Dokument anzuwenden
        const signature = new signatureLib.Signature('input.docx');

        // Geben Sie das erforderliche digitale Zertifikat und das Passwort an
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Konfigurieren Sie bei Bedarf die visuellen Signatur-Einstellungen
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Verschlüsseln Sie das Dokument mit dem digitalen Zertifikat
        const result = signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimieren oder sichern Sie Dokumenteninhalt mit Signaturen"
  description: "GroupDocs.Signature for Node.js via Java wurde entwickelt, um alle gängigen Dateiformate zu signieren und bietet Ihnen die Möglichkeit, verschiedene Arten von Signaturen hinzuzufügen, anzupassen, zu überprüfen oder zu entfernen."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Wesentliche Funktionen von GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signaturen zu Ihren Dokumenten hinzufügen"
      content: "Platzieren Sie Text-, Bild-, Barcode-, QR-Code- oder Stempel-Signaturen ganz einfach auf jeder Seite unterstützter Dokumente. Sie können auch versteckte Metadaten wie EXIF in Bildern einfügen oder bearbeiten. Schützen Sie den Inhalt Ihres Dokuments vor unbefugten Änderungen mit digitalen Zertifikaten."

    # feature loop
    - title: "Signaturen finden und überprüfen"
      content: "Nach der Signatur kann Ihr Dokument mehreren Überprüfungen unterzogen werden. Bestätigen Sie die Integrität des signierten Inhalts oder führen Sie eine detaillierte Suche durch, um alle vorhandenen Signaturen aufzulisten."

    # feature loop
    - title: "Vorhandene Signaturen überarbeiten"
      content: "Die meisten Signaturtypen ermöglichen nach der Erstellung Änderungen. Sie können Text ganz einfach bearbeiten, Elemente neu positionieren, Farben anpassen, die Größe ändern und andere erforderliche Änderungen vornehmen."

    # feature loop
    - title: "Unnötige Signaturen entfernen"
      content: "Unsere Lösung ermöglicht vollständige CRUD-Operationen für Signaturen. Bei Bedarf können Sie verschiedene Signaturtypen, einschließlich digitaler Zertifikate, aus Ihrem Dokument entfernen."
      
  code_samples:
    # code sample loop
    - title: "Dokumente mit digitalen Signaturen schützen"
      content: |
        Erfahren Sie, wie Sie ein Dokument gegen Änderungen mit digitalen Signaturen sperren.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Geben Sie das Dokument an, das signiert werden muss
        const signature = new signatureLib.Signature('input.docx');

        // Verwenden Sie ein entsprechendes digitales Zertifikat und dessen Passwort
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Fügen Sie zusätzliche Textinformationen hinzu
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // Fügen Sie visuelle Elemente wie Bilder für die Darstellung der Signatur hinzu
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // Speichern Sie das digital gesicherte Dokument an einem bestimmten Ort
        const result = signature.sign('output.docx', options);
        ```
        {{< /landing/code >}}


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
    title: "Lernen Sie unsere Hauptfunktionen kennen"
    exclude: "digital"
    description: "Wir unterstützen stolz eine umfassende Palette von Signaturoptionen und -funktionen."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Dokumente in mehreren Formaten signieren"
    exclude: "DOCX"
    description: "Die Node.js via Java API unterstützt über 60 Formate und ermöglicht es Ihnen, eine Vielzahl von Signaturen auf jeder Seite anzuwenden, die Sicherheit des Inhalts mit digitalen Zertifikaten durchzusetzen und Signaturen innerhalb des Dokuments effektiv zu verwalten."
    items: 
          
        # format loop 1
        - name: "PDF schützen"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX schützen"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "PPTX schützen"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "XLSX schützen"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---