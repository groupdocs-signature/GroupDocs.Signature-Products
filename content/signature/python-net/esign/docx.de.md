



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:11
draft: false
lang: de
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "E-Signatur von DOCX-Dokumenten mit Python-Apps"
head_description: "Nutzen Sie die Möglichkeiten der Python-API, um DOCX-Dokumente wie PDFs, Word-Dateien, Excel-Tabellen, Präsentationen und Bilder elektronisch zu unterzeichnen und zu sichern."

############################# Header ############################
title: "Elektronische E-Signatur für DOCX" 
description: "GroupDocs.Signature for Python via .NET ermöglicht es, eine Vielzahl von elektronischen Signaturen in Ihre Dokumente einzufügen und dabei Compliance und Datenintegrität über Formate wie PDFs, Word, Excel, Präsentationen und Bilder hinweg sicherzustellen."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Überblick über die GroupDocs.Signature for Python via .NET-API"
    link: "/signature/python-net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) bietet eine umfassende Suite von Tools zum Hinzufügen elektronischer Signaturen zu Dokumenten. Ob Sie unterschreiben, suchen, verifizieren, aktualisieren oder digitale Signaturen entfernen müssen, GroupDocs.Signature for Python via .NET erleichtert dies über mehrere Formate hinweg—PDFs, Word-Dokumente, Excel-Tabellen, PowerPoint-Präsentationen und verschiedene Bildformate—ohne dass Drittanbieter-Software benötigt wird.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zur E-Signatur von DOCX mit Python"
    content: |
      Mit [GroupDocs.Signature](/signature/python-net/) können Python via .NET-Entwickler die Signaturfunktion nahtlos in DOCX-Dokumente integrieren. Fügen Sie Ihren Anwendungen benutzerdefinierte Signaturen hinzu.
      
      1. Laden Sie die DOCX-Datei in die Signature-Instanz.
      2. Verwenden Sie SignOptions, um die Signatur­einstellungen zu konfigurieren.
      3. Passen Sie Eigenschaften der Signatur wie Größe, Farbe und Inhalt an.
      4. Speichern Sie das signierte Dokument am gewünschten Speicherort.
   
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

            # Laden Sie das Dokument in eine Signature-Instanz
            with sg.Signature('input.docx') as signature:

                # Erstellen Sie ein neues QrCodeSignOptions-Objekt
                options = sg.QrCodeSignOptions("QR code text")

                # Richten Sie alle erforderlichen Optionen ein
                options.Left = 100
                options.Top = 100
                options.ForeColor = sg.Color.Red

                # Speichern Sie das signierte Dokument in Ihrem System
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte E-Signatur-Funktionen für Dokumente"
  description: "Unsere E-Signatur-API optimiert Geschäftsprozesse, indem sie effiziente Möglichkeiten bietet, elektronische Signaturen zu signieren, zu validieren, zu modifizieren und zu verwalten, mit vollständiger Unterstützung für die Automatisierung."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "E-Signatur-Funktionen"
  features:
    # feature loop
    - title: "E-Signatur für Bürodokumente"
      content: "Platzieren Sie elektronische Signaturen an beliebiger Stelle in Ihren Dokumenten. Passen Sie Ihren Inhalt mit digitalen Zertifikaten, Barcodes, Metadaten und visuellen Elementen an, während Sie die Sicherheit und Authentizität des Dokuments gewährleisten."

    # feature loop
    - title: "Vollständige Signaturverwaltung"
      content: "Sobald ein Dokument signiert ist, können Sie alle Signaturen anzeigen und verwalten. Sie können Aktualisierungen vornehmen oder Signaturen nach Bedarf entfernen, um die vollständige Kontrolle über das Dokument zu gewährleisten."

    # feature loop
    - title: "Dokumentsicherheit erhöhen"
      content: "Schützen Sie Ihre Dokumente mit digitalen Zertifikaten. Betten Sie Metadaten ein oder rufen Sie diese ab, um Nachverfolgung, Prüfung und Compliance zu verbessern und die Authentizität Ihres Inhalts zu gewährleisten."
      
  code_samples_ext:
    # code sample ext loop
    - title: "So fügen Sie einer Dokumenten-Signatur ein Bild hinzu"
      content: |
        Dieses Beispiel zeigt, wie Sie eine Bildsignatur auf einer bestimmten Seite eines Dokuments anwenden können.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg
        
          def run():

              # Laden Sie das Dokument, das Sie signieren möchten,
              with sg.Signature('input.docx') as signature:

                  # Legen Sie den Pfad zum Bild in den Signatur­optionen fest.
                  options = sg.ImageSignOptions("image.jpg")

                  # Definieren Sie die Größe und Platzierung der Signatur auf den Zielseiten.
                  options.VerticalAlignment = sg.VerticalAlignment.Bottom
                  options.HorizontalAlignment = sg.HorizontalAlignment.Right
                  options.Height = 150
                  options.Width = 200
                  options.Margin = sg.Padding(50)
                  options.AllPages = True

                  # Wenden Sie die Signatur an und speichern Sie das signierte Dokument.
                  result = signature.Sign("output.docx", options)
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
            link: "/examples/signature/formats/signature_esign.docx"
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
    title: "Entdecken Sie unser vollständiges Funktionsset"
    exclude: "esign"
    description: "Wir bieten eine Vielzahl von Signaturalternativen und -operationen für alle Ihre E-Signatur-Anforderungen."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "E-Signatur für eine Vielzahl von Datei­formaten"
    exclude: "DOCX"
    description: "Mit der Python via .NET-API können Sie über 60 branchenübliche Formate elektronisch signieren, was Ihnen unvergleichliche Flexibilität beim Sichern Ihrer Geschäftsdokumente bietet."
    items: 
          
        # format loop 1
        - name: "e-Sign PDF"
          format: "PDF"
          link: "/signature/python-net/esign/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "e-Sign DOCX"
          format: "DOCX"
          link: "/signature/python-net/esign/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "e-Sign JPEG"
          format: "JPEG"
          link: "/signature/python-net/esign/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "e-Sign PPTX"
          format: "PPTX"
          link: "/signature/python-net/esign/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "e-Sign XLSX"
          format: "XLSX"
          link: "/signature/python-net/esign/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---