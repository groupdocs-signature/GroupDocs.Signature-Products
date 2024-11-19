



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:19
draft: false
lang: de
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "QR-Code für PDF mit Java erstellen"
head_description: "Die GroupDocs.Signature-API ermöglicht die Generierung von QR-Codes für PDF-Dateien. Erstellen Sie QR-Codes aus Ihrem Inhalt und platzieren Sie sie auf jeder Seite."

############################# Header ############################
title: "QR-Codes für PDF erstellen" 
description: "Erstellen Sie 2D-Barcode mit Text- und numerischen Daten und platzieren Sie diese auf beliebigen Seiten verschiedener Dokumente mithilfe von GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlose Testversion"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Erfahren Sie mehr über GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) bietet eine Vielzahl von Funktionen zur Erstellung und Einbettung verschiedener Arten von Unterschriften in allen gängigen Dokumentformaten. Es unterstützt PDFs, Word-Dokumente, Excel-Tabellen, PowerPoint-Präsentationen und Bilder. Verbessern Sie Ihre Dokumente mit Text-, Bild-, Barcode-, QR-Code-, Metadaten-, digitalen und Stempelunterschriften.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Erzeugen und Platzieren eines QR-Codes an beliebiger Stelle in einer PDF"
    content: |
      [GroupDocs.Signature](/signature/java/) kann QR-Codes in vielen gängigen Formaten generieren und sie auf PDF-Seiten platzieren. Über 10 QR-Code-Typen werden unterstützt und können schnell in Java-Anwendungen integriert werden. Nutzen Sie unser Produkt, um Dokumente mit generierten QR-Codes zu signieren.
      
      1. Holen Sie sich die PDF-Datei oder den Stream, der mit einem QR-Code signiert werden soll.
      2. Geben Sie den Text für QrCodeSignOptions an.
      3. Passen Sie visuelle Optionen wie Farbe, Position, Größe usw. an.
      4. Speichern Sie die Datei mit dem QR-Code.
   
    code:
      platform: "java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Beispielunterschriften"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "Klicken zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Übergeben Sie das Dokument an eine neue Signature-Instanz
        Signature signature = new Signature("input.pdf");

        // Verwenden Sie QrCodeSignOptions, um einen QR-Code zum Dokument hinzuzufügen
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Geben Sie den Unterschriftstyp und die Position auf der Seite an
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Speichern Sie die Datei mit dem hinzugefügten QR-Code
        signature.sign("output.pdf", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fügen Sie Ihren Dokumenten Unterschriften hinzu"
  description: "Die GroupDocs.Signature for Java-API unterstützt das Signieren aller gängigen Dateiformate. Generieren, ändern, suchen, überprüfen und löschen Sie verschiedene Arten von Unterschriften."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Wichtige Funktionen von GroupDocs.Signature"
  features:
    # feature loop
    - title: "Dokumente signieren"
      content: "GroupDocs.Signature unterstützt das Signieren mit Text-, Bild-, Barcode-, QR-Code- und Stempelunterschriften. Platzieren Sie sie auf beliebigen Seiten eines unterstützten Dokumentformats. Verwenden Sie Metadatenunterschriften zur Verwaltung der Dokumentenmetadaten und schützen Sie den Inhalt vor unbefugten Änderungen mit digitalen Zertifikaten."

    # feature loop
    - title: "Suche und Überprüfung"
      content: "Stellen Sie sicher, dass alle Unterschriften in einem Dokument gültig sind, indem Sie das Überwachungsverfahren anwenden. Rufen Sie eine vollständige Liste der Unterschriften in einem Dokument mit der integrierten Suchfunktion ab."

    # feature loop
    - title: "Unterschriften ändern"
      content: "Ändern Sie problemlos die Eigenschaften von Unterschriften nach der Signatur. Passen Sie den Inhalt, die Position, die Farbe, die Größe und andere Attribute nach Bedarf an."

    # feature loop
    - title: "Unterschriften entfernen"
      content: "Löschen Sie unerwünschte Unterschriften problemlos. Verschiedene Unterschriftstypen, einschließlich digitaler Zertifikate, können programmgesteuert aus Dokumenten entfernt werden."
      
  code_samples_ext:
    # code sample ext loop
    - title: "So passen Sie einen generierten QR-Code an"
      content: |
        Verwenden Sie dieses Beispiel, um zu lernen, wie Sie einen neuen QR-Code auf einer PDF-Seite platzieren.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Holen Sie sich das Dokument, das signiert werden soll, und übergeben Sie es an Signature
          Signature signature = new Signature("input.pdf");

          // Verwenden Sie die QR-Code-Optionen, um den Text mit den erforderlichen Informationen bereitzustellen
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Legen Sie die relative Position des QR-Codes auf der Seite fest
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Legen Sie die Unterschriftspolsterung fest
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Geben Sie die Farbe des QR-Codes an
          signOptions.setForeColor(Color.RED);

          // Definieren Sie die Schriftartenoptionen für die Nachricht
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Passen Sie die Hintergrundfarbe und den Pinsel des QR-Codes an
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Fügen Sie den QR-Code zum Dokument hinzu
          SignResult signResult = signature.sign("output.pdf", signOptions);
          ```
        platform: "java"
        copy_title: "Kopieren"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "Klicken zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pdf"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Maven herunterladen"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Entdecken Sie unser Hauptangebot"
    exclude: "qrcode"
    description: "Wir bieten eine vielfältige Auswahl an Signaturfunktionen und fortgeschrittenen Operationen."
    items: 
          
        # operation loop 1
        - name: "Elektronische Unterschriften"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Fügen Sie verschiedene Arten von Unterschriften zu unterstützten Dateiformaten hinzu"

        # operation loop 2
        - name: "Text zu Dokumenten hinzufügen"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Inhalt von Dokumenten mit anpassbaren Textunterschriften verbessern"

        # operation loop 3
        - name: "Bildunterschriften"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Jedes Bild an beliebiger Stelle innerhalb eines Dokuments platzieren"

        # operation loop 4
        - name: "Barcodes generieren"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Verschiedene Barcodes erstellen und in unterstützte Dokumente einfügen"

        # operation loop 5
        - name: "QR-Codes generieren"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "QR-Codes erzeugen und für die Dokumentenunterzeichnung verwenden"
          
        # operation loop 6
        - name: "Digitale Zertifikate"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Sichern Sie Geschäfte und signieren Sie Dokumente mit digitalen Zertifikaten"

        # operation loop 7
        - name: "Stempelunterschriften"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "Verwenden Sie den Stempel-Builder, um anpassbare runde oder quadratische Stempel zu erstellen"
          
        # operation loop 8
        - name: "Unterschriften suchen"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Alle zuvor hinzugefügten Unterschriften in einem Dokument lokalisieren"
          
        # operation loop 9
        - name: "Unterschrift überprüfen"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Die Authentizität von Unterschriften nach ihrer Anwendung überprüfen"
          
        # operation loop 10
        - name: "Unterschriften bearbeiten"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Verschiedene Unterschriften innerhalb eines Dokuments bearbeiten"
          
        # operation loop 11
        - name: "Unterschriften löschen"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Eine Vielzahl von zuvor angewandten Unterschriften entfernen"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "QR-Codes für zusätzliche Dateiformate generieren"
    exclude: "PDF"
    description: "Bereichern Sie alle gängigen Dateiformate mit generierten QR-Codes mithilfe der Java-API. Fügen Sie 2D-Bardaten für einfaches Scannen und Verarbeiten hinzu."
    items: 
          
        # format loop 1
        - name: "QR-Code für PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "QR-Code für DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "QR-Code für JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "JPEG-Bild"
          
        # format loop 4
        - name: "QR-Code für PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 5
        - name: "QR-Code für XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---