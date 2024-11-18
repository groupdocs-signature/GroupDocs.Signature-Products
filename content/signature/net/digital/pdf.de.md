



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:58
draft: false
lang: de
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Hinzufügen von digitalen elektronischen Signaturen zu PDF-Dateien mit C#"
head_description: "Fügen Sie einer PDF-Datei mit C# in nur wenigen Codezeilen eine digitale Signatur hinzu. Verwenden Sie GroupDocs.Signature for .NET, um zahlreiche Dateiformate zu signieren."

############################# Header ############################
title: "eSign PDF mit digitalen Signaturen" 
description: "Schützen Sie die Integrität Ihrer Geschäftsdokumente, indem Sie sie mit digitalen Zertifikaten versiegeln, die die robusten Funktionen von GroupDocs.Signature for .NET nutzen. Wir bieten vielseitige Lösungen, um Ihre Dokumente zu kennzeichnen und zu sichern."
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
    title: "Über GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) ist eine ausgeklügelte Signierlösung, die eine breite Palette von Dokumentenverarbeitungsaufgaben erleichtert. Sie ermöglicht das Einfügen von Text, Bildern, digitalen Zertifikaten und Stempeln in Dateien in über 60 Formaten, einschließlich PDF, MS Office, Bildern, ZIP-Dateien und anderen wichtigen Geschäftsdokumenten. Außerdem können signierte Dokumente nach Bedarf mühelos durchsucht, verifiziert, bearbeitet oder entfernt werden.

############################# Steps ############################
steps:
    enable: true
    title: "Wie man PDF mit digitalen Zertifikaten in C# sichert"
    content: |
      [GroupDocs.Signature](/signature/net/) ermöglicht es .NET-Entwicklern, PDF-Dokumente gegen Veränderungen mittels digitaler Signaturen zu schützen. Bereichern Sie Ihre Geschäftsanwendungen mit robusten Datenschutzfunktionen.
      
      1. Übergeben Sie das PDF-Dokument an den Konstruktor der Signature-Klasse.
      2. Verwenden Sie ein digitales Zertifikat und dessen Passwort, um das Dokument abzusichern.
      3. Fügen Sie optional eine visuelle Darstellung der digitalen Signatur auf den Dokumentseiten hinzu.
      4. Signieren Sie das Dokument, um sicherzustellen, dass es unverändert bleibt.
   
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
        // Nutzen Sie Signature zur digitalen Signatur des Dokuments
        using (Signature signature = new Signature("input.pdf"))
        {
            // Legen Sie das digitale Zertifikat und das zugehörige Passwort bereit
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Konfigurieren Sie die visuelle Darstellung, falls erforderlich
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // Sichern Sie das Dokument mit dem digitalen Zertifikat
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Verbessern oder sichern Sie den Dokumenteninhalt mit Signaturen"
  description: "Die GroupDocs.Signature for .NET-Bibliothek wurde entwickelt, um alle gängigen Dateiformate zu signieren. Optimieren Sie Ihre Geschäftsprozesse, indem Sie eine Vielzahl von Signaturen problemlos hinzufügen, ändern, verifizieren oder entfernen."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signaturen in Dokumente einfügen"
      content: "Fügen Sie Text-, Bild-, Barcode-, QR-Code- oder Stempelsignaturen präzise auf jeder Seite eines unterstützten Dokuments ein. Sie können auch versteckte Metadaten, wie EXIF, in Bildern und den meisten Dateitypen hinzufügen oder bearbeiten. Gewährleisten Sie die Integrität Ihres Dokumenteninhalt mit digitalen Signaturen."

    # feature loop
    - title: "Signaturen suchen und verifizieren"
      content: "Die Nachverarbeitung von Signaturen bietet zahlreiche Möglichkeiten. Überprüfen Sie, ob Ihre signierten Dokumente korrekt verarbeitet wurden. Für mehr Kontrolle können Sie eine umfassende Liste aller Signaturen über die Suchfunktion abrufen."

    # feature loop
    - title: "Signaturen bearbeiten"
      content: "Die meisten Signaturtypen sind vollständig bearbeitbar. Sie haben die Flexibilität, den Text anzupassen, Elemente neu anzuordnen, Farben zu ändern, die Größe zu ändern und mehr."

    # feature loop
    - title: "Überflüssige Signaturen entfernen"
      content: "Unsere Lösung bietet vollständige CRUD-Operationen für Signaturen. Falls erforderlich, können Sie eine Vielzahl von Signaturtypen, einschließlich digitaler Zertifikate, aus Ihrem Dokument entfernen."
      
  code_samples:
    # code sample loop
    - title: "Dokumente mit digitalen Signaturen sichern"
      content: |
        Erfahren Sie, wie Sie Dokumentenänderungen mit digitalen Signaturen verhindern.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Geben Sie das Dokument an, das signiert werden soll
        using (Signature signature = new Signature("input.pdf"))
        {
            // Verwenden Sie ein gültiges digitales Zertifikat mit dem entsprechenden Passwort
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Geben Sie zusätzliche Textinformationen an
                Reason = "Security issue",
                Contact = "John Smith",
                Location = "Office D.W.",

                // Fügen Sie ein Bild und weitere Optionen für die visuelle Darstellung hinzu
                ImageFilePath = "image.png",
                AllPages = true,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Width = 60,
                Height = 80,

                Margin = new Padding() {  Bottom = 10, Right = 10 }
            };

            // Speichern Sie das gesicherte Dokument an einem gewünschten Ort
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```
        {{< /landing/code >}}


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
    title: "Entdecken Sie unsere herausragenden Funktionen"
    exclude: "digital"
    description: "Wir bieten eine reiche Vielfalt an Signaturformaten und leistungsstarken Operationen."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
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
    title: "Dokumenten in verschiedenen Formaten signieren"
    exclude: "PDF"
    description: "Die .NET-API ermöglicht es Ihnen, über 60 verschiedene Formate zu verarbeiten. Sie können nahtlos verschiedene Signaturen auf jeder Seite erstellen und einfügen, digitale Zertifikate für die Sicherheit des Inhalts anwenden und bestehende Signaturen effizient verwalten."
    items: 
          
        # format loop 1
        - name: "PDF schützen"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX schützen"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "PPTX schützen"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "XLSX schützen"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---