---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Ods
productName: Java
lang: de
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Ods with Java

############################# Head ############################
head_title: "Suche nach Text-Signaturen in der Datei Ods in Java"
head_description: "Verwenden Sie Java für die Suche nach Text-Signaturen in Ods-Dateien mit ein paar Zeilen Code."

############################# Header ############################
title: "Suchen Sie nach Text-Signaturen in der Datei Ods"
description: "Die native API von Java ermöglicht die Suche nach Text-Signaturen in bereits signierten Ods-Dateien. Führen Sie mit wenigen Codezeilen eine erweiterte E-Signatur-Suche in Ihren Ods-Dokumenten durch."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Über die GroupDocs.Signature for Java-API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bietet Java API zur Verarbeitung von Dokumenten mit verschiedenen Signaturtypen wie Texten, Bildern, digitalen Zertifikaten, Barcodes, QR-Codes, Stempeln oder Metadaten. Benutzer können elektronische Signaturen in PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten hinzufügen, löschen, aktualisieren, überprüfen oder suchen, mit zusätzlicher Unterstützung für die Anpassung von Signatureigenschaften nach Bedarf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "So suchen Sie nach Text-Signaturen in Ods"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) erleichtert Entwicklern von Java die Suche nach Text-Signaturen in Ods-Dateien aus ihren Anwendungen, indem einige einfache Schritte implementiert werden.
        
        * Erstellen Sie eine neue Instanz der Signature-Klasse und übergeben Sie den Pfad des Quelldokuments als Konstruktorparameter.
        * Instanziieren Sie das SearchOptions-Objekt gemäß Ihren Anforderungen und geben Sie Suchoptionen an.
        * Rufen Sie die Search-Methode der Signature-Klasseninstanz auf und übergeben Sie ihr SearchOptions.
        * Suchergebnisse entsprechend Ihren Anforderungen aufbereiten.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laden Sie die neueste Version von GroupDocs.Signature for Java von [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) herunter
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        TextSearchOptions options = new TextSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
                            
        // search for Text signatures in Ods document
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren mit Text-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zu Ods-Dateien hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Suchen Sie mit Java nach anderen Text-Signaturen"
    content: |
        "Elektronische Signaturen suchen in verschiedenen Dokumenten. Finden Sie Signaturen in einem der gängigen Dateiformate, wie unten gezeigt."
    format: 
           
       
back_to_top:
    enable: true
---