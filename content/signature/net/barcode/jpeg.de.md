



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:06
draft: false
lang: de
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Barcode für JPEG mit C# API generieren"
head_description: "Erzeugen Sie eine Barcode-Signatur und sichern Sie Ihr JPEG-Dokument mit C# in nur wenigen Codezeilen. Nutzen Sie GroupDocs.Signature für die Unterzeichnung einer Vielzahl von Dateiformaten."

############################# Header ############################
title: "Barcode für JPEG-Dokumente generieren" 
description: "Verwenden Sie GroupDocs.Signature for .NET, um Barcodes an jeder Stelle innerhalb Ihrer Geschäftsdokumente zu platzieren. Unsere API bietet umfangreiche Anpassungsmöglichkeiten für Barcode-Signaturen."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Überblick über GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) ist eine leistungsstarke Dokumentensignaturlösung, die eine breite Palette von Signaturtypen unterstützt, darunter Text, Bilder, Barcodes, digitale Zertifikate und Stempel. Mit der Unterstützung von über 60 Dateiformaten – wie PDF, MS Office, Bilder, ZIP-Dateien und mehr – ermöglicht dieses Tool nicht nur das Anwenden von Signaturen, sondern auch das Suchen, Verifizieren, Modifizieren oder Entfernen von Signaturen nach Bedarf.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zur Generierung und Einbettung eines Barcodes in eine JPEG-Datei"
    content: |
      [GroupDocs.Signature](/signature/net/) ermöglicht die Generierung von Barcodes in zahlreichen gängigen Formaten und deren Platzierung auf JPEG-Seiten. Mit Unterstützung für über 60 Barcodetypen können .NET-Anwendungen mühelos mit Barcode-Signierfunktionen aufgestockt werden, indem unsere Bibliothek integriert wird.
      
      1. Liefern Sie die JPEG-Datei oder den Stream zur Verarbeitung.
      2. Übergeben Sie den Barcode-Text an die BarcodeSignOptions-Instanz.
      3. Passen Sie die Barcode-Optionen wie Position, Größe usw. an.
      4. Speichern Sie die Datei mit dem neu hinzugefügten Barcode.
   
    code:
      platform: "net"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Beispielunterschriften"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "Klicken zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Erstellen Sie ein neues Signature-Objekt mit dem Dokumentenpfad
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Verwenden Sie BarcodeSignOptions, um einen Barcode zum Dokument hinzuzufügen
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // Konfigurieren Sie den Barcodetyp und zusätzliche Eigenschaften
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // Speichern Sie die signierte Datei
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweitern und sichern Sie Ihre Dokumente mit fortschrittlichen Signaturfunktionen"
  description: "Die GroupDocs.Signature for .NET-Bibliothek wurde entwickelt, um die umfassende Dokumentensignierung und -verarbeitung in weitverbreiteten Dateiformaten zu erleichtern. Sie können mühelos verschiedene Arten von Signaturen hinzufügen, anpassen, verifizieren oder entfernen."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Signature"
  features:
    # feature loop
    - title: "Vielseitige Dokumentensignierung"
      content: "Effizient jede Seite von unterstützten Dokumenten mit Text, Bildern, Barcodes, QR-Codes oder Stempeln signieren. Außerdem können Sie versteckte Metadaten, wie EXIF-Daten in Bildern, einfügen oder den Inhalt Ihres Dokuments mit digitalen Zertifikaten gegen unbefugte Änderungen schützen."

    # feature loop
    - title: "Umfassende Signatur-Suche und -Verifizierung"
      content: "Unser Tool bietet leistungsstarke Funktionen zum Arbeiten mit signierten Dokumenten. Stellen Sie die Integrität Ihrer Dokumente durch Verifizierung der Signaturen sicher und rufen Sie mühelos eine umfassende Liste aller Signaturen in einem Dokument über unsere Suchfunktion ab."

    # feature loop
    - title: "Signaturen bequem bearbeiten"
      content: "Fast alle zuvor angewendeten Signaturen können modifiziert werden. Aktualisieren Sie Text, ändern Sie die Position oder passen Sie Farben nach Ihren Bedürfnissen an."

    # feature loop
    - title: "Effiziente Signaturentfernung"
      content: "Unser Ansatz unterstützt vollständig CRUD-Operationen für Signaturen, sodass Sie unerwünschte oder veraltete Signaturen schnell aus Ihren Dokumenten entfernen können."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Wie man eine Barcode-Signatur generiert"
      content: |
        Dieses Beispiel zeigt, wie man einen maßgeschneiderten Barcode auf JPEG-Dokumentseiten einfügt.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.jpeg"))
          {
              // Formulieren Sie die Signaturoptionen mit dem gewünschten Text
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // Bestimmen Sie die relative Barcode-Position auf der Seite
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // Definieren Sie den Abstand des Barcodes vom Seitenrand
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // Geben Sie die Farbe der Striche an
                  ForeColor = Color.Red,

                  // Wählen Sie den Schriftstil für die Nachricht
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // Geben Sie die Position der Nachricht an
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // Signieren und speichern Sie das Dokument
              SignResult result = signature.Sign("output.jpeg", options);
          }
          ```
        platform: "net"
        copy_title: "Kopieren"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "Klicken zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.jpeg"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Nuget herunterladen"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Entdecken Sie unsere Hauptfunktionen"
    exclude: "barcode"
    description: "Wir bieten eine beeindruckende Auswahl an Signaturoptionen und -operationen"
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Dokumente in verschiedenen Formaten signieren"
    exclude: "JPEG"
    description: "Unsere .NET-API unterstützt die Unterzeichnung von mehr als 60 verschiedenen Formaten. Platzieren Sie mühelos verschiedene Arten von Signaturen auf jeder Seite oder an beliebiger Stelle innerhalb Ihrer Dokumente."
    items: 
          
        # format loop 1
        - name: "Barcode zu PDF hinzufügen"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Barcode zu DOCX hinzufügen"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Barcode zu JPEG hinzufügen"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "Barcode zu PPTX hinzufügen"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "Barcode zu XLSX hinzufügen"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---