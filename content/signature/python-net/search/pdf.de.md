



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:13
draft: false
lang: de
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Elektronische Signaturen suchen in PDF mit Python"
head_description: "Nutzen Sie die GroupDocs.Signature for Python via .NET API, um elektronische Signaturen in Formaten wie PDFs, Word, Excel, Präsentationen und Bildern zu suchen."

############################# Header ############################
title: "Suche nach digitalen Signaturen in PDF" 
description: "Extrahieren Sie umfassend eine Liste elektronischer Signaturen aus verschiedenen Formaten, einschließlich PDFs, Word, Excel, Präsentationen und Bildern, mit der Leistungsfähigkeit von GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt herunterladen"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Entfesseln Sie das Potenzial von GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) bietet fortschrittliche Funktionen zur Unterzeichnung und Verwaltung digitaler Dokumente. Mit Unterstützung für über 60 Dateiformate, einschließlich PDFs, Office-Dokumenten, Bildern und ZIP-Dateien, können Sie Signaturen wie Texte, Bilder, Barcodes, QR-Codes, digitale Zertifikate und Stempel hinzufügen, suchen, verifizieren, ändern oder entfernen.

############################# Steps ############################
steps:
    enable: true
    title: "So suchen Sie nach Signaturen in PDF mit Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) bietet eine leistungsstarke Engine zum Erkennen digitaler Signaturen in PDF-Dateien. Python via .NET-Entwickler können ihre Apps problemlos um diese Funktionalität erweitern.
      
      1. Geben Sie den Dateipfad der PDF Datei für die Signatursuche an.
      2. Verwenden Sie SearchOptions, um die Suchkriterien zu verfeinern.
      3. Rufen Sie die Methode Search auf, um die Ergebnisse abzurufen.
      4. Überprüfen Sie die Liste der identifizierten Signaturen.
   
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

            # Initialisieren Sie ein Signature Objekt mit dem Dateipfad des Dokuments
            with sg.Signature('input.pdf') as signature:

                # Erstellen Sie eine Instanz von TextSearchOptions, um alle Seiten zu durchsuchen
                options = sg.TextSearchOptions()
                options.AllPages = True

                # Führen Sie eine Suche durch, um alle textbasierten Signaturen im Dokument zu finden
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # Stellen Sie eine Liste der gefundenen Signaturen für eine detaillierte Überprüfung zusammen
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Eine umfassende Plattform zum Dokumenten-signieren"
  description: "Erleben Sie eine leistungsstarke, funktionsreiche Lösung zum Signieren, die Ihre Dokumente mit mehreren Signaturtypen sichert, die über verschiedene Dateiformate hinweg reichen."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Signaturen suchen und verwalten"
  features:
    # feature loop
    - title: "Unterzeichnen und sichern Sie Geschäftsdokumente"
      content: "Fügen Sie elektronische Signaturen an beliebiger Stelle in einem Dokument hinzu. GroupDocs.Signature unterstützt verschiedene Signaturtypen, einschließlich Text, Bilder, Barcodes, Metadaten, Stempel und digitale Zertifikate, um die Authentizität und Sicherheit des Dokuments zu gewährleisten."

    # feature loop
    - title: "Umfassende Signaturverwaltung"
      content: "Sobald ein Dokument signiert ist, nutzen Sie die Suchfunktion, um alle eingebetteten Signaturen zu finden. Sie können Signaturen nach Bedarf ändern oder entfernen und haben somit die volle Kontrolle über die Integrität des Dokuments."

    # feature loop
    - title: "Sichern Sie die Integrität des Dokuments"
      content: "Nutzen Sie fortschrittliche Werkzeuge, um versteckte Metadaten in Dokumenten zu verwalten. Fügen Sie Metadaten hinzu oder entfernen Sie diese und wenden Sie digitale Zertifikate an, um Ihre Dokumente vor unautorisierten Änderungen zu schützen und deren Authentizität zu gewährleisten."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Suche nach Bildsignaturen"
      content: |
        Dieses Beispiel zeigt, wie man eine Bildsignatur innerhalb eines bestimmten Dokuments findet.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Übergeben Sie das Quell-Dokument an den Konstruktor
              with sg.Signature('input.pdf') as signature:

                    # Suchen Sie nach textbasierten Signaturen
                    signatures = signature.Search(sg.SignatureType.Image)
                    print("\nSource document contains following image signature(s).")

                    # Zeigen Sie detaillierte Eigenschaften der identifizierten Signaturen an
                    for imageSignature in signatures:
                        print("\nFound image signature at page ", imageSignature.PageNumber)
          ```
        platform: "python-net"
        copy_title: "Kopieren"
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
    title: "Kernfunktionen"
    exclude: "search"
    description: "Unsere API bietet umfangreiche Flexibilität, die es Benutzern ermöglicht, Dokumente zu signieren und nachsignierte Operationen wie Suchen, Verifizieren und Bearbeiten von Signaturen durchzuführen."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
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
    title: "Signaturen aus mehreren Dateiformaten extrahieren"
    exclude: "PDF"
    description: "Die GroupDocs.Signature for Python via .NET API ermöglicht es Ihnen, Signaturen aus einer Vielzahl von Dokumentformaten zu extrahieren und zu verwalten. Holen Sie sich problemlos eingebettete Signaturen aus gängigen Dateitypen für eine weitere Analyse oder Verarbeitung."
    items: 
          
        # format loop 1
        - name: "Unterschriften in PDF suchen"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Unterschriften in DOCX finden"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Unterschriften in PPTX finden"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Unterschriften in XLSX suchen"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---