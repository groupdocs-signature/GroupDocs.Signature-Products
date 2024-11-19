



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:10
draft: false
lang: de
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Bildunterschriften zu PDF-Dateien mit JavaScript hinzufügen"
head_description: "Fügen Sie Bildunterschriften zu PDF-Dateien für Node.js mit nur wenigen Codezeilen hinzu. Verwenden Sie die GroupDocs.Signature for Node.js via Java-API, um Bilder hinzuzufügen."

############################# Header ############################
title: "PDF-Dateien mit Bildunterschriften signieren" 
description: "Nutzen Sie die Funktionen von GroupDocs.Signature for Node.js via Java, um Bilder in eine Vielzahl von Office-Dokumentformaten wie PDF, Word, Excel und verschiedenen Bilddateien einzufügen. Das Hinzufügen eines Unternehmenssignaturbildes kann die Professionalität und Glaubwürdigkeit Ihrer Dokumente erheblich steigern und eine raffinierte Präsentation schaffen."
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
    title: "GroupDocs.Signature for Node.js via Java vorstellen"
    link: "/signature/nodejs-java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ermöglicht es Benutzern, Bildunterschriften an beliebiger Stelle in ihren Dokumenten einzufügen. Dieses Tool ermöglicht es Unternehmen, ihre Workflows zu optimieren, indem Bilder in PDFs, Word, Excel, PowerPoint und gängige Bildformate eingefügt werden, wodurch die Effizienz des Dokumentenmanagements verbessert wird.

############################# Steps ############################
steps:
    enable: true
    title: "Anleitung zum Hinzufügen von Bildern in PDF mit JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ermöglicht es Node.js via Java-Anwendungen, Bildunterschriften mühelos in PDF-Dokumente zu integrieren. Erweitern Sie die Fähigkeiten Ihrer Anwendung mit unserer umfassenden Bibliothek.
      
      1. Signature mit dem PDF-Dokument instanziieren
      2. ImageSignOptions verwenden, um das Signaturbild festzulegen
      3. Das Bild präzise auf einer beliebigen Seite positionieren
      4. Das signierte Dokument am gewünschten Speicherort speichern
   
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

        // Signature mit dem Pfad zum Dokument initialisieren
        const signature = new signatureLib.Signature('input.pdf');

        // ImageSignOptions konfigurieren, um die gewünschte Bildunterschrift einzuschließen
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // Das Bild in der oberen linken Ecke aller Seiten platzieren
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // Das Dokument mit der angewendeten Bildunterschrift speichern
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Funktionen zur Dokumentensignatur"
  description: "Unsere API bietet ein umfassendes Funktionspaket, das elektronische Signaturen vereinfacht. Sie können verschiedene Arten von Signaturen, einschließlich Bildunterschriften, hinzufügen, ändern, entfernen, suchen und validieren."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Bildunterschriften"
  features:
    # feature loop
    - title: "Bilder in Office-Dokumente einfügen"
      content: "Platzieren Sie Bildunterschriften überall in Ihrem Dokument, sei es in PDF-, Word- oder Excel-Dateien. Verbessern Sie Ihre Dokumente, indem Sie Bilder, Barcodes, Metadaten oder digitale Zertifikate für zusätzliche Funktionalität hinzufügen."

    # feature loop
    - title: "Signaturen suchen und validieren"
      content: "Stellen Sie die Authentizität Ihrer signierten Dokumente sicher, indem Sie die Signaturen überprüfen. Nutzen Sie die Suchfunktion, um alle in Ihrem Dokument eingebetteten Signaturen abzurufen und zu überprüfen."

    # feature loop
    - title: "Vorhandene Signaturen ändern"
      content: "Unsere API ermöglicht es Benutzern, Signaturen nach Bedarf zu aktualisieren und anzupassen. Ändern Sie die Größe, Position oder andere Attribute einer zuvor hinzugefügten Signatur für Flexibilität im Dokumentenhandling."

    # feature loop
    - title: "Unnötige Signaturen entfernen"
      content: "Verwalten Sie Ihre Dokumente effizient, indem Sie Signaturen entfernen, die nicht mehr benötigt werden. Unsere API unterstützt vollständige CRUD-Operationen für fast alle Signaturtypen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Dokumente mit Bildunterschriften verbessern"
      content: |
        Erfahren Sie, wie Sie Bilder in Geschäftsdokumente einfügen, um zusätzliche Informationen hinzuzufügen.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Wählen Sie das zu signierende Dokument aus
          const signature = new signatureLib.Signature('input.pdf');

          // Bilderoptionen mit dem Bildpfad konfigurieren
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // Die Größe der Bildunterschrift anpassen
          options.setWidth(100);
          options.setHeight(100);

          // Das Bild in der unteren rechten Ecke platzieren
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Falls erforderlich, Padding von den Seitenrändern hinzufügen
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Optional einen benutzerdefinierten Rahmen um das Bild hinzufügen
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Die Bildunterschrift für ein optimales Erscheinungsbild drehen
          options.setRotationAngle(45);

          // Das aktualisierte Dokument am gewünschten Speicherort speichern
          const result = signature.sign('output.pdf', options);
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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "Entdecken Sie die Funktionen, die wir anbieten"
    exclude: "image"
    description: "Wir sind stolz darauf, eine breite Auswahl an Signaturmethoden und -operationen anzubieten."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Bilder zu verschiedenen Dateitypen hinzufügen"
    exclude: "PDF"
    description: "Die Node.js via Java-API ermöglicht es Ihnen, Bilder in eine breite Palette von Dokumentenformaten einzufügen. Passen Sie Größe, Platzierung und Seitenpositionierung an, um Ihren Dokumentensignaturprozess zu verbessern."
    items: 
          
        # format loop 1
        - name: "PDF mit Bild unterschreiben"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX mit Bild unterschreiben"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "JPEG mit Bild unterschreiben"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "PPTX mit Bild unterschreiben"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "XLSX mit Bild unterschreiben"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---