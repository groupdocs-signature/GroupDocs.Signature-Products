



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: de
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Erstellen Sie runde und quadratische Stempel in JPEG mit Python"
head_description: "Generieren und fügen Sie personalisierte Stempel in JPEG-Dateien mit der GroupDocs.Signature for Python via .NET-API ein."

############################# Header ############################
title: "Stempel für JPEG erstellen" 
description: "Fügen Sie mit GroupDocs.Signature for Python via .NET benutzerdefinierte, gestaltete Stempel in jedem Teil Ihrer Dokumente hinzu und nutzen Sie die große Flexibilität für Platzierung und Konfiguration, um Ihre geschäftlichen Anforderungen zu erfüllen."
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
    title: "Überblick über GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) ist ein umfassendes Tool, mit dem Sie verschiedene Signaturtypen in Dokumente einfügen können, darunter benutzerdefinierte Stempel. Mit Unterstützung für über 60 Dateiformate – von PDFs und Word-Dokumenten bis hin zu Bildern und ZIP-Dateien – können Sie Ihre Dokumente mit Text, Bildern, Barcodes, Metadaten, digitalen Zertifikaten und Stempeln verbessern. Sie haben auch die vollständige Kontrolle, um angewendete Signaturen zu suchen, zu überprüfen, zu bearbeiten oder zu löschen.

############################# Steps ############################
steps:
    enable: true
    title: "So fügen Sie einen Stempel zu JPEG mit Python hinzu"
    content: |
      [GroupDocs.Signature](/signature/python-net/) bietet robuste Stempelerstellungstools zur Verbesserung von Python via .NET-Anwendungen. Nutzen Sie es, um benutzerdefinierte Stempel für Ihre Dokumentseiten zu gestalten und zu implementieren.
      
      1. Stellen Sie das JPEG-Dokument bereit, das Sie stempeln möchten.
      2. Verwenden Sie StampSignOptions, um alle erforderlichen Einstellungen zu konfigurieren.
      3. Fügen Sie mehrere Stempellinien hinzu, falls erforderlich.
      4. Wenden Sie den Stempel an und speichern Sie das aktualisierte Dokument.
   
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

            # Hängen Sie den Dokumentenpfad an die Signature-Instanz an
            with sg.Signature('input.jpeg') as signature:

                # Richten Sie StampSignOptions mit den erforderlichen Stempeldetails ein
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # Fügen Sie ein oder mehrere Linien zum Stempel hinzu
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # Speichern Sie das Dokument mit dem angewendeten Stempel
                result = signature.Sign("output.jpeg", options)
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Nutzen Sie Signaturen zur Sicherung und Verbesserung der Dokumentenintegrität"
  description: "Mit der GroupDocs.Signature for Python via .NET-Bibliothek können Sie nahtlos Signaturfunktionen in Ihren Dokumenten hinzufügen. Erstellen, ändern, überprüfen oder löschen Sie einfach benutzerdefinierte Stempel und andere Signaturtypen, um Ihnen Flexibilität und Sicherheit in Ihren Dokumenten Workflows zu bieten."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Stempel-Signaturen Powered by GroupDocs.Signature"
  features:
    # feature loop
    - title: "Vollständige Dokumentenunterzeichnung"
      content: "Steigern Sie Ihre Dokumente, indem Sie Signaturen wie Text, Bilder, Barcodes, QR-Codes und Stempel an beliebiger Stelle auf jeder Seite hinzufügen. Verwalten Sie eingebettete Metadaten und wenden Sie digitale Zertifikate an, um sich gegen unbefugte Änderungen zu schützen."

    # feature loop
    - title: "Effiziente Signatursuche und -verifizierung"
      content: "Nach der Unterzeichnung verwenden Sie erweiterte Suchwerkzeuge, um alle eingebetteten Signaturen zu finden. Verifizieren oder verwalten Sie die Signaturdaten problemlos, um die Integrität des Dokuments sicherzustellen."

    # feature loop
    - title: "Signaturen bearbeiten und anpassen"
      content: "Ändern Sie zuvor hinzugefügte Signaturen. Egal, ob Sie den Inhalt, die Position, die Größe oder die Farbe ändern möchten, GroupDocs.Signature for Python via .NET gibt Ihnen die volle Kontrolle, um Signaturen nach Bedarf anzupassen."

    # feature loop
    - title: "Signaturen einfach entfernen"
      content: "Wenn Sie Signaturen entfernen müssen, bietet GroupDocs.Signature for Python via .NET alle erforderlichen Werkzeuge, um jeden Typ zu löschen, einschließlich Stempeln und digitalen Zertifikaten, damit Sie Ihre Dokumente aktuell und konform halten."
      
  code_samples_ext:
    # code sample ext loop
    - title: "So fügen Sie benutzerdefinierte Stempel zu Dokumenten hinzu"
      content: |
        Dieses Beispiel zeigt, wie Sie benutzerdefinierte Stempel mit spezifischen Textdetails in ein Dokument erstellen und einfügen.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Stellen Sie das Dokument bereit, das Sie stempeln möchten
              with sg.Signature('input.jpeg') as signature:

                    # Richten Sie die Stempeloptionen mit Ihren gewünschten Einstellungen ein
                    options = sg.StampSignOptions()

                    # Definieren Sie die Größe und Platzierung des Stempels auf der Seite
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # Fügen Sie äußere kreisförmige Linien mit Text hinzu
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # Fügen Sie optional innere quadratische Linien hinzu
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # Schließen Sie ab und speichern Sie das gestempelte Dokument
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "Entdecken Sie die wichtigsten Funktionen"
    exclude: "stamp"
    description: "Finden Sie eine Vielzahl von Optionen zum Erstellen, Verwalten und Entfernen von Signaturen, die Ihnen die vollständige Kontrolle über die Dokumenten-Workflows geben."
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
    title: "Wenden Sie Stempel auf verschiedene Dokumentformate an"
    exclude: "JPEG"
    description: "Mit der GroupDocs.Signature-API können Sie benutzerdefinierte Stempel in mehr als 60 standardisierte Dateitypen einfügen. Platzieren Sie Stempel überall in Ihren Dokumenten und verbessern Sie die Personalisierung und Nachverfolgbarkeit."
    items: 
          
        # format loop 1
        - name: "PDF stempeln"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX stempeln"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "JPEG stempeln"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "PPTX stempeln"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "XLSX stempeln"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---