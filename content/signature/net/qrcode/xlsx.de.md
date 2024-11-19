



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: de
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "QR-Code für XLSX-Dateien mit C# generieren"
head_description: "Nutzen Sie die GroupDocs.Signature-API zur Generierung von QR-Codes für XLSX-Dateien. Integrieren Sie QR-Codes nahtlos auf jeder Seite für erweiterte Funktionalität."

############################# Header ############################
title: "QR-Codes für XLSX generieren" 
description: "Generieren Sie mühelos 2D-Barcodes mithilfe von Text- oder numerischen Daten und wenden Sie diese auf mehrere Seiten und Formate an, einschließlich PDFs, Word, Excel und mehr, über GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Starten Sie Ihre kostenlose Testversion"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Entdecken Sie die Möglichkeiten von GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) bietet eine breite Palette an Funktionen, die es den Benutzern ermöglichen, verschiedene Signaturtypen in führenden Dokumentformaten zu generieren und einzubetten. Egal, ob es sich um PDFs, Word-Dokumente, Excel-Tabellen, PowerPoint-Präsentationen oder Bilddateien handelt, Sie können Ihre Dokumente mit Text-, Bild-, Barcode-, QR-Code-, Metadaten-, digitalen und Stempel-Signaturen aufwerten.

############################# Steps ############################
steps:
    enable: true
    title: "So generieren und fügen Sie einen QR-Code an beliebiger Stelle innerhalb eines XLSX ein"
    content: |
      [GroupDocs.Signature](/signature/net/) erleichtert die Generierung von QR-Codes in verschiedenen gängigen Formaten und deren Platzierung auf XLSX-Seiten. Unsere Bibliothek unterstützt über 10 QR-Code-Typen und kann nahtlos in .NET-Anwendungen integriert werden. Verbessern Sie Ihre Dokumente mit QR-Code-Signaturen mithilfe unseres Produkts.
      
      1. Erwerben Sie die XLSX-Datei oder den Stream, der mit einem QR-Code signiert werden soll.
      2. Stellen Sie den erforderlichen Text für QrCodeSignOptions zur Verfügung.
      3. Passen Sie visuelle Parameter wie Farbe, Position, Größe usw. an.
      4. Speichern Sie das Dokument mit dem eingebetteten QR-Code.
   
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
        // Initialisieren Sie eine neue Signature-Instanz mit dem Dokument
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Nutzen Sie QrCodeSignOptions, um einen QR-Code in das Dokument einzufügen
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Geben Sie den Signaturtyp an und bestimmen Sie dessen Position auf der Seite
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Speichern Sie das Dokument mit dem integrierten QR-Code
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Umfassende Signaturintegration für Dokumente"
  description: "Mit der GroupDocs.Signature for .NET-API können Benutzer mühelos eine Vielzahl von Signaturtypen generieren, ändern, suchen, validieren und entfernen, sodass Dokumentenabläufe mit unvergleichlicher Präzision optimiert werden."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Signature"
  features:
    # feature loop
    - title: "Dokumentensignierung mit mehreren Signaturtypen"
      content: "GroupDocs.Signature ermöglicht die Anwendung von Text-, Bild-, Barcode-, QR-Code- und Stempelsignaturen auf jedes Dokumentformat. Signaturen können präzise auf jeder Seite platziert werden, und Metadaten können nahtlos über Metadaten-Signaturen verwaltet werden. Schützen Sie die Integrität Ihrer Dokumente, indem Sie digitale Zertifikate einfügen, die unbefugte Änderungen verhindern."

    # feature loop
    - title: "Signaturensuche und -validierung"
      content: "Überprüfen Sie die Echtheit und Genauigkeit von Dokumentensignaturen durch einen fortschrittlichen Validierungsprozess. Rufen Sie mühelos eine detaillierte Liste aller in einem Dokument eingebetteten Signaturen ab, um umfassende Einblicke zu erhalten."

    # feature loop
    - title: "Anpassbare Signaturänderung"
      content: "Aktualisieren und verfeinern Sie zuvor angewendete Signaturen, indem Sie Inhalte, Platzierung, Farbe, Größe und andere Attribute an Ihre spezifischen Anforderungen anpassen."

    # feature loop
    - title: "Effiziente Signaturentfernung"
      content: "Optimieren Sie Ihr Dokumentenmanagement, indem Sie unerwünschte Signaturen programmatisch entfernen. Ob bei digitalen Zertifikaten oder anderen Signaturtypen, die Entfernung kann schnell und effektiv erfolgen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Wie generiert man einen QR-Code mit verschiedenen Optionen?"
      content: |
        Dieses Beispiel zeigt, wie man einen benutzerdefinierten QR-Code auf einer XLSX-Seite platziert.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Rufen Sie das zu signierende Dokument ab und übergeben Sie es an Signature
          using (Signature signature = new Signature("input.xlsx"))
          {
              // Konfigurieren Sie die QR-Code-Optionen mit dem erforderlichen Text
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Bestimmen Sie die relative Position des QR-Codes auf der Seite
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Setzen Sie den Signaturabstand
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Geben Sie die Farbe des QR-Codes an
                    ForeColor = Color.Red,

                    // Definieren Sie die Schriftartenoptionen für die Nachricht
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Passen Sie die Hintergrundfarbe und den Pinsel des QR-Codes an
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Fügen Sie den QR-Code in das Dokument ein
              SignResult result = signature.Sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_qrcode.xlsx"
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
    title: "Erfahren Sie mehr über unsere Signaturlösungen"
    exclude: "qrcode"
    description: "Wir präsentieren stolz eine breite Palette an Signaturtypen und Betriebsfunktionen"
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "QR-Codes für andere Dokumentformate generieren"
    exclude: "XLSX"
    description: "Bereichern Sie alle branchenüblichen Datei-Formate mit der Möglichkeit, QR-Codes über die .NET-API einzubetten. Speichern und codieren Sie wichtige Informationen in 2D-Barcodes für nahtloses Scannen und Datenabruf."
    items: 
          
        # format loop 1
        - name: "QR-Code für PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "QR-Code für DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "QR-Code für JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "QR-Code für PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "QR-Code für XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---