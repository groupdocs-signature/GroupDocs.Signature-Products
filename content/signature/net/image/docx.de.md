



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:09
draft: false
lang: de
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Bildunterschriften zu DOCX-Dateien mit C# hinzufügen"
head_description: "DOCX-Datei für .NET mit wenigen Codezeilen signieren. Nutzen Sie die GroupDocs.Signature for .NET-API, um Bilder hinzuzufügen."

############################# Header ############################
title: "Bildunterschrift zu DOCX-Dateien hinzufügen" 
description: "Nutzen Sie GroupDocs.Signature for .NET, um Bilder nahtlos in eine Vielzahl von Office-Dokumentformaten zu integrieren, einschließlich PDFs, Word, Excel und Bilddateien. Die Einbindung eines Bildes der Unterschrift Ihres Vorgesetzten kann einen beeindruckenden professionellen Eindruck hinterlassen und die visuelle Anziehungskraft sowie die Authentizität Ihrer Dokumente erhöhen."
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
    title: "GroupDocs.Signature for .NET entdecken"
    link: "/signature/net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) bietet umfassende Möglichkeiten zum Einbetten von Bildunterschriften an beliebiger Stelle auf jeder Seite innerhalb Ihrer Geschäftsdokumente. Optimieren Sie Ihre Arbeitsabläufe, indem Sie Bilder nahtlos in PDFs, Word-Dokumente, Excel-Tabellen, PowerPoint-Präsentationen und verschiedene gängige Bildformate über unsere robuste Bibliothek integrieren.

############################# Steps ############################
steps:
    enable: true
    title: "So fügen Sie ein Bild an einer beliebigen Stelle eines DOCX mit C# hinzu"
    content: |
      Nutzen Sie [GroupDocs.Signature](/signature/net/), um .NET-Anwendungen mit der Fähigkeit auszustatten, Unterschriften präzise in jede Seite von DOCX-Dokumenten einzufügen. Erweitern Sie nahtlos die Fähigkeiten Ihres Produkts durch die Integration unserer Lösung.
      
      1. Instanziieren Sie die Signature-Klasse mit dem DOCX-Dokument.
      2. Nutzen Sie ImageSignOptions, um das Unterschriftsbild festzulegen.
      3. Positionieren Sie das Bild präzise an der gewünschten Stelle auf einer beliebigen Seite.
      4. Speichern Sie das neu signierte Dokument an einem festgelegten Ort.
   
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
        // Initialisieren Sie Signature mit dem Pfad zum Dokument
        using (Signature signature = new Signature("input.docx"))
        {
            // Konfigurieren Sie ImageSignOptions mit einem Bild für die Unterschrift
            ImageSignOptions options = new ImageSignOptions("company_logo.jpg")
            {
                // Positionieren Sie das Bild in der oberen linken Ecke aller Seiten
                AllPages = true,
                Left = 100,
                Top = 200
            };

            // Speichern Sie das signierte Dokument
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Umfassende Lösungen zur Dokumentenunterzeichnung"
  description: "Wir freuen uns, Ihnen eine breite Palette von Signaturfunktionen vorzustellen, die von unserer API unterstützt werden. Fügen Sie problemlos verschiedene Signaturtypen hinzu, ändern, löschen, suchen und verifizieren Sie diese, einschließlich bildbasierter Unterschriften."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Bildunterzeichnung"
  features:
    # feature loop
    - title: "Bilder in Office-Dokumente einbetten"
      content: "Fügen Sie elektronische Unterschriften und Bilder nahtlos an beliebiger Stelle auf jeder Seite eines Dokuments ein. Verbessern Sie den Inhalt Ihres Dokuments mit Text, Bildern, Barcodes, Metadaten oder digitalen Zertifikaten, um die Funktionalität und Sicherheit zu erhöhen."

    # feature loop
    - title: "Signatursuche und -verifikation"
      content: "Verwalten Sie unterschriebene Dokumente, indem Sie die Authentizität und Integrität der Unterschriften überprüfen. Rufen Sie eine umfassende Liste aller Unterschriften innerhalb eines Dokuments ab und prüfen Sie deren spezifische Attribute."

    # feature loop
    - title: "Unterschriften ändern"
      content: "Gelegentlich müssen Unterschriften in Dokumenten aktualisiert werden. Passen Sie den Inhalt, das Aussehen, die Größe oder die Position vorhandener Unterschriften an, um den sich ändernden Anforderungen gerecht zu werden."

    # feature loop
    - title: "Überflüssige Unterschriften entfernen"
      content: "Unsere API ermöglicht vollständige CRUD-Operationen für die meisten Signaturtypen. Sie können nach Bedarf Unterschriften aus nahezu allen unterstützten Dokumentformaten effizient entfernen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Dokumenteninhalt mit Bildunterschriften sichern"
      content: |
        Erfahren Sie, wie Sie Geschäftsdokumente durch das Einbetten von Bildern anreichern und zusätzliche Informationen bereitstellen.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Wählen Sie das zu signierende Dokument aus
          using (Signature signature = new Signature("input.docx"))
          {
              // Erstellen Sie Bildoptionen mit dem angegebenen Bildpfad
              ImageSignOptions options = new ImageSignOptions("manager_signature.jpg")
              {
                    // Definieren Sie die Abmessungen der Bildunterschrift
                    Width = 100,
                    Height = 100,

                    // Positionieren Sie das Bild in der unteren rechten Ecke
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,

                    // Wenden Sie bei Bedarf den erforderlichen Abstand zu den Seitenrändern an
                    Margin = new Padding() { Bottom = 120, Right = 120 },

                    // Optional: Fügen Sie der Abbildung einen individuellen Rahmen hinzu
                    Border = new Border()
                    {
                        Visible = true,
                        Color = Color.Red,
                        DashStyle = DashStyle.DashDotDot,
                        Weight = 5
                    },

                    // Drehen Sie die Unterschrift zur optimalen Ausrichtung
                    RotationAngle = 45
              };

              // Speichern Sie das aktualisierte Dokument an dem gewünschten Ort
              SignResult result = signature.Sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_image.docx"
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
    title: "Verstehen Sie unser Leistungsangebot"
    exclude: "image"
    description: "Entdecken Sie eine Vielzahl von Signaturtypen und robusten Operationen, die von unserer Plattform bereitgestellt werden."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Bilder in verschiedene Dateiformate integrieren"
    exclude: "DOCX"
    description: "Nutzen Sie die .NET-API, um unterstützte Bildformate an eine breite Palette von Dokumenten anzuhängen. Passen Sie die Größe an, positionieren Sie die Bilder, wählen Sie spezifische Seiten aus und fügen Sie bildbasierte Unterschriften in Ihre Dokumente ein."
    items: 
          
        # format loop 1
        - name: "PDF mit Bild unterschreiben"
          format: "PDF"
          link: "/signature/net/image/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX mit Bild unterschreiben"
          format: "DOCX"
          link: "/signature/net/image/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "JPEG mit Bild unterschreiben"
          format: "JPEG"
          link: "/signature/net/image/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "PPTX mit Bild unterschreiben"
          format: "PPTX"
          link: "/signature/net/image/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "XLSX mit Bild unterschreiben"
          format: "XLSX"
          link: "/signature/net/image/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---