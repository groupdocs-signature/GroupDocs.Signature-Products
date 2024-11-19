



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:16
draft: false
lang: de
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Digitale elektronische Signaturen zu PDF-Dateien mit Java hinzufügen"
head_description: "Fügen Sie einer PDF-Datei mit Java in nur wenigen Zeilen Code eine digitale Signatur hinzu. Verwenden Sie GroupDocs.Signature for Java, um zahlreiche Dateiformate zu signieren."

############################# Header ############################
title: "PDF mit digitalen Signaturen signieren" 
description: "Schützen Sie den Inhalt Ihrer Geschäftsdokumente, indem Sie diese mit digitalen Zertifikaten versehen, die die Funktionen von GroupDocs.Signature for Java nutzen. Wir bieten zahlreiche Möglichkeiten, um Ihre Dokumente zu kennzeichnen und zu sichern."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) ist eine umfassende Signierlösung, die verschiedene Arten der Dokumentenverarbeitung unterstützt. Sie können Text, Bilder, digitale Zertifikate und Stempel zu Dateien in über 60 Formaten hinzufügen, darunter PDF, MS Office, Bilder, ZIP-Dateien und andere gängige Geschäftsformate. Darüber hinaus können signierte Dokumente auf bequeme Weise automatisch durchsucht, verifiziert, bearbeitet oder gelöscht werden.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zum Schützen von PDF mit digitalen Zertifikaten in Java"
    content: |
      [GroupDocs.Signature](/signature/java/) ermöglicht es Java-Entwicklern, Änderungen an PDF-Dokumenten mithilfe digitaler Signaturen zu verhindern. Statten Sie Ihre Unternehmensanwendungen mit der Fähigkeit aus, wichtige Daten zu sichern.
      
      1. Übergeben Sie das PDF-Dokument an den Konstruktor der Signature-Klasse.
      2. Verwenden Sie ein digitales Zertifikat und dessen Passwort, um das Dokument zu schützen.
      3. Fügen Sie optional eine visuelle Darstellung der digitalen Signatur auf den Dokumentseiten hinzu.
      4. Signieren Sie das Dokument, um zukünftige Änderungen zu verhindern.
   
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
        // Verwenden Sie Signature mit dem Dokument für die digitale Signatur
        Signature signature = new Signature("input.pdf");

        // Stellen Sie ein digitales Zertifikat und ein Passwort bereit
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Richten Sie eine visuelle Darstellung ein, falls erforderlich
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Schützen Sie das Dokument mit einem digitalen Zertifikat
        SignResult result = signature.sign("output.pdf", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweitern oder schützen Sie den Dokumenteninhalt mit Signaturen"
  description: "Die GroupDocs.Signature for Java-Bibliothek ist in der Lage, alle gängigen Dateiformate zu signieren. Fügen Sie verschiedene Arten von Signaturen automatisch hinzu, bearbeiten, verifizieren oder löschen Sie diese, um Ihre Geschäftsprozesse zu optimieren."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Funktionen von GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signaturen zu Dokumenten hinzufügen"
      content: "Text-, Bild-, Barcode-, QR-Code- oder Stempel-Signaturen können präzise auf jeder Seite eines unterstützten Dokuments hinzugefügt werden. Versteckte Metadaten wie EXIF können in Bildern und den meisten Dateitypen hinzugefügt oder bearbeitet werden. Schützen Sie den Dokumenteninhalt vor unbefugten Änderungen mithilfe digitaler Signaturen."

    # feature loop
    - title: "Signaturensuche und -verifizierung"
      content: "Dokumente können nach dem Signieren auf verschiedene Weise verarbeitet werden. Überprüfen Sie signierte Dokumente, um sicherzustellen, dass sie ordnungsgemäß verarbeitet wurden. Falls Sie mehr Kontrolle benötigen, erhalten Sie eine Liste aller Signaturen über die Suche."

    # feature loop
    - title: "Signaturen bearbeiten"
      content: "Die meisten Arten von Signaturen unterstützen weitere Anpassungen. Sie können Text korrigieren, Position, Farbe, Größe und mehr ändern."

    # feature loop
    - title: "Unnötige Signaturen entfernen"
      content: "Unsere Lösung unterstützt vollständige CRUD-Operationen für Signaturen. Viele Arten von Signaturen, einschließlich digitaler Zertifikate, können bei Bedarf aus einem Dokument gelöscht werden."
      
  code_samples:
    # code sample loop
    - title: "Dokumente mit digitalen Signaturen schützen"
      content: |
        Erfahren Sie, wie Sie ein Dokument vor Änderungen mithilfe digitaler Signaturen sichern.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Stellen Sie ein Dokument zur Signatur bereit
        Signature signature = new Signature("input.pdf");

        // Verwenden Sie ein gültiges digitales Zertifikat mit Passwort
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Geben Sie zusätzliche Textdaten an
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Verwenden Sie ein Bild und andere Optionen für die visuelle Darstellung
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Speichern Sie das geschützte Dokument an einem anderen Speicherort
        SignResult result = signature.sign("output.pdf", options);
        ```
        {{< /landing/code >}}


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
    title: "Überprüfen Sie unser umfassendes Funktionsangebot"
    exclude: "digital"
    description: "Wir sind stolz auf die umfangreiche Funktionalität und die Unterstützung von Signaturen, die unsere Plattform bietet."
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
    title: "Dokumente in anderen Formaten signieren"
    exclude: "PDF"
    description: "Die Java-API ermöglicht das Verarbeiten von mehr als 60 Formaten. Erstellen Sie verschiedene Signaturen, fügen Sie diese jeder Seite hinzu, sichern Sie Inhalte mit digitalen Zertifikaten und verwalten sowie bearbeiten Sie bestehende Signaturen innerhalb des Dokuments."
    items: 
          
        # format loop 1
        - name: "PDF schützen"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "DOCX schützen"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "PPTX schützen"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "XLSX schützen"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---