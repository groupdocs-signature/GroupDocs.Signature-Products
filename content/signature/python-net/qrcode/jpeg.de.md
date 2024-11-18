



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:04
draft: false
lang: de
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "QR-Codes für JPEG-Dateien mit Python generieren"
head_description: "Verwenden Sie die GroupDocs.Signature-API, um QR-Codes in JPEG-Dateien zu generieren und einzubetten. Platzieren Sie QR-Codes ganz einfach auf jeder Seite, um zusätzliche Funktionen hinzuzufügen."

############################# Header ############################
title: "QR-Codes für JPEG generieren" 
description: "Erstellen Sie mühelos 2D-Barcodes mit Text- oder numerischen Daten und wenden Sie sie auf verschiedene Seiten und Formate an, einschließlich PDFs, Word, Excel und mehr mit GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlose Testversion"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET-Funktionen entdecken"
    link: "/signature/python-net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) bietet eine Vielzahl von Funktionen, die es Benutzern ermöglichen, verschiedene Signaturtypen in wichtigen Dokumenten zu generieren und einzubetten. Egal, ob es sich um PDFs, Word, Excel, PowerPoint oder Bilder handelt – verbessern Sie Ihre Dokumente mit Text-, Bild-, Barcode-, QR-Code-, Metadaten-, digitalen oder Stempel-Signaturen.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Generieren und Einfügen eines QR-Codes in JPEG"
    content: |
      [GroupDocs.Signature](/signature/python-net/) ermöglicht es Ihnen, QR-Codes in gängigen Formaten zu erstellen und sie auf JPEG-Seiten zu platzieren. Mit Unterstützung für über 10 QR-Code-Typen können Sie diese Funktion nahtlos in Python via .NET-Anwendungen integrieren. Verbessern Sie Ihre Dokumente mit QR-Code-Signaturen unter Verwendung unseres Produkts.
      
      1. Erwerben Sie die JPEG-Datei oder den Stream, in den der QR-Code hinzugefügt wird.
      2. Geben Sie den erforderlichen Text an QrCodeSignOptions.
      3. Passen Sie die visuellen Einstellungen wie Farbe, Position und Größe an.
      4. Speichern Sie das Dokument mit dem eingebetteten QR-Code.
   
    code:
      platform: "python-net"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Beispielunterschriften"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "Klicken zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Initialisieren Sie eine neue Signature-Instanz mit dem Dokument
            with sg.Signature('input.jpeg') as signature:

                # Verwenden Sie QrCodeSignOptions, um einen QR-Code in das Dokument einzubetten
                options = sg.QrCodeSignOptions("Text Content")

                # Geben Sie den Signaturtyp an und setzen Sie seine Position auf der Seite
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Speichern Sie das Dokument mit dem eingebetteten QR-Code
                result = signature.Sign("output.jpeg", options)
        ```                 

############################# More features ############################
more_features:
  enable: true
  title: "Vollständige Signaturintegration für Dokumente"
  description: "Mit der GroupDocs.Signature for Python via .NET-API können Benutzer verschiedene Signaturtypen generieren, ändern, suchen, validieren und entfernen, um Dokumentenworkflows präzise zu vereinfachen."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Signature"
  features:
    # feature loop
    - title: "Anwenden mehrerer Signaturtypen"
      content: "GroupDocs.Signature ermöglicht die Anwendung von Text-, Bild-, Barcode-, QR-Code- und Stempel-Signaturen auf jedes Dokument. Sie können Signaturen präzise auf jeder Seite platzieren und Metadaten problemlos verwalten. Schützen Sie Ihre Dokumente vor unbefugten Änderungen mit digitalen Zertifikaten."

    # feature loop
    - title: "Signaturen suchen und validieren"
      content: "Überprüfen Sie die Authentizität und Genauigkeit von Dokumentensignaturen mit fortschrittlichen Validierungstools. Erhalten Sie mühelos eine detaillierte Auflistung aller in einem Dokument eingebetteten Signaturen für eine bessere Übersicht."

    # feature loop
    - title: "Vorhandene Signaturen ändern"
      content: "Sie können zuvor angewendete Signaturen aktualisieren, indem Sie Inhalt, Position, Farbe, Größe und andere Attribute an Ihre spezifischen Anforderungen anpassen."

    # feature loop
    - title: "Signaturen einfach entfernen"
      content: "Optimieren Sie das Dokumentenmanagement, indem Sie unerwünschte Signaturen schnell entfernen. Ob es sich um ein digitales Zertifikat oder einen anderen Signaturtyp handelt, die Entfernung kann effizient erfolgen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Einen generierten QR-Code anpassen"
      content: |
        Dieses Beispiel zeigt, wie man einen angepassten QR-Code auf einer JPEG-Seite platziert.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Holen Sie das zu signierende Dokument und übergeben Sie es an Signature
              with sg.Signature('input.jpeg') as signature:

                    # Konfigurieren Sie die QR-Code-Optionen mit dem erforderlichen Text
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Setzen Sie die Position des QR-Codes auf der Seite
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Legen Sie den Abstand für die Signatur fest
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Wählen Sie die Farbe des QR-Codes
                    options.ForeColor = sg.Color.Red

                    # Definieren Sie die Schriftoptionen für die Nachricht
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Legen Sie die Hintergrundfarbe und die Pinsel für den QR-Code fest
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Betten Sie den QR-Code in das Dokument ein
                    result = signature.Sign("output.jpeg", options)
          ```
        platform: "python-net"
        copy_title: "Kopieren"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "Klicken zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.jpeg"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "PyPi herunterladen"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Entdecken Sie unsere Signaturlösungen"
    exclude: "qrcode"
    description: "Wir bieten eine breite Palette von Signaturtypen und Operationen, um Ihren Dokumentenbedürfnissen gerecht zu werden."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "QR-Codes in verschiedenen Dokumentenformaten einbetten"
    exclude: "JPEG"
    description: "Verwenden Sie die Python via .NET-API, um QR-Codes in jedes branchenübliche Dokumentenformat einzubetten. Speichern und kodieren Sie wichtige Informationen in 2D-Barcodes für einfaches Scannen und Datenabruf."
    items: 
          
        # format loop 1
        - name: "QR-Code für PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "QR-Code für DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "QR-Code für JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "QR-Code für PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "QR-Code für XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---