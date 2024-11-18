



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:12
draft: false
lang: de
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Suche nach digitalen Signaturen in PDF mit Java"
head_description: "Nutzen Sie die GroupDocs.Signature for Java API, um Signaturen in PDF-Dateien zu suchen. Finden Sie Signaturen in PDFs, Word-, Excel-, Präsentationsdateien und Bildern."

############################# Header ############################
title: "Suche nach digitalen Signaturen in PDF" 
description: "Erhalten Sie eine vollständige Liste von elektronischen Signaturen, die in PDF-, Word-, Excel-, Präsentations- oder Bilddateien eingebettet sind, mithilfe von GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenloser Download"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) bietet leistungsstarke Funktionen für das Signieren von Dokumenten. Es unterstützt das Hinzufügen von Texten, Bildern, Barcodes, digitalen Zertifikaten und Stempeln zu Dateien in über 60 Formaten, einschließlich PDFs, MS Office-Dokumenten, Bildern, ZIP-Dateien und anderen gängigen Geschäftsformaten. Darüber hinaus können Sie Signaturen jederzeit suchen, verifizieren, ändern oder löschen.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zur Suche nach PDF-Signaturen mit Java"
    content: |
      [GroupDocs.Signature](/signature/java/) bietet eine leistungsstarke Engine zur Suche nach digitalen Signaturen in PDF-Dateien. Java-Entwickler können ihre Anwendungen mit unserer Lösung erweitern.
      
      1. Geben Sie den PDF-Dateipfad für die Signatursuche an.
      2. Verwenden Sie SearchOptions, um die Suchergebnisse zu verfeinern.
      3. Führen Sie die Methode Search aus, um die Ergebnisse zu erhalten.
      4. Analysieren Sie die Liste der gefundenen Signaturen.
   
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

        // Erstellen Sie eine Instanz von Signature mit dem Dokumentenpfad
        final Signature signature = new Signature("input.pdf");

        // Instanziieren Sie TextSearchOptions für alle Seiten
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // Suchen Sie nach Textsignaturen im Dokument
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // Listen Sie die gefundenen Signaturen zur weiteren Analyse auf
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Umfassende Lösung für Dokumentensignaturen"
  description: "Wir freuen uns, unsere Lösung für Dokumentensignaturen vorzustellen, die mit allen gängigen Dokumentenformaten kompatibel ist. Fügen Sie eine Vielzahl von Signaturen hinzu, um Ihre Dokumente zu verbessern oder deren Inhalt abzusichern."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Suche nach Signaturen"
  features:
    # feature loop
    - title: "Geschäftsdokumente signieren"
      content: "Fügen Sie digitale Signaturen an beliebiger Stelle auf jeder Seite eines Dokuments ein. Verwenden Sie verschiedene Signaturtypen wie Text, Bilder, Barcodes, Metadaten, Stempel oder digitale Zertifikate."

    # feature loop
    - title: "Signaturen verwalten"
      content: "Nach dem Signieren müssen Dokumente möglicherweise weiter verarbeitet werden. Suchen Sie nach allen verfügbaren Signaturen und aktualisieren oder löschen Sie sie nach Bedarf."

    # feature loop
    - title: "Inhalt des Dokuments schützen"
      content: "Verwalten Sie versteckte Metadaten, die im Dokument eingebettet sind. Fügen Sie neue Metadaten hinzu oder entfernen Sie vorhandene Einträge. Verwenden Sie Unternehmenszertifikate, um den Inhalt des Dokuments vor unbefugten Änderungen zu schützen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Suche nach Bildsignaturen"
      content: |
        Dieses Beispiel zeigt, wie man eine Bildsignatur in einem bestimmten Dokument findet.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Übergeben Sie das Quelldokument als Konstruktorparameter
          final Signature signature = new Signature("input.pdf");

          // Suchen Sie nach Signaturen vom Typ Text
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // Zeigen Sie die Ergebnisse mit den Eigenschaften der gefundenen Signaturen an
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
          }
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
    title: "Unterstützte Operationen"
    exclude: "search"
    description: "Unser Produkt bietet eine flexible API zum Signieren von Dokumenten und zum Verwalten von Signaturen nach dem Signieren."
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
    title: "Signaturen in verschiedenen Dateiformaten suchen"
    exclude: "PDF"
    description: "Mit der GroupDocs.Signature for Java API können Sie die Liste der Signaturen aus jeder signierten Datei abrufen. Extrahieren Sie Signaturen aus gängigen Dateiformaten zur weiteren Verarbeitung."
    items: 
          
        # format loop 1
        - name: "Unterschriften in PDF suchen"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 2
        - name: "Unterschriften in DOCX finden"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 3
        - name: "Unterschriften in PPTX finden"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "PowerPoint Open XML-Präsentation"
          
        # format loop 4
        - name: "Unterschriften in XLSX suchen"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Microsoft Excel Open XML-Tabelle"


          

---