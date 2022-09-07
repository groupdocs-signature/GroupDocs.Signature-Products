---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Tiff
productName: Java
lang: de
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Tiff for Java

############################# Head ############################
head_title: "Elektronische Metadaten-Signaturen an Tiff-Dokumente über Java anhängen"
head_description: "Verwenden Sie Metadaten als versteckte elektronische Signaturen in Ihren Tiff-Dokumenten mit ein paar Zeilen Java-Code. Verwenden Sie die GroupDocs Document Signature API, um Ihre Geschäftsdokumente und Dateien mit Metadateninformationen elektronisch zu signieren."

############################# Header ############################
title: "Elektronische Metadaten-Signaturen für das Dokument Tiff über Java sind einfach und benutzerfreundlich!"
description: "Unterschreiben Sie Ihre {{Dateiformat}}-Dokumente und Verträge mit versteckten Metadateneinträgen. Generieren Sie Metadaten für PDFs, MS Word-Dokumente, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen und verschiedene Bildformate ohne Probleme und zusätzliche Codierung."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Über die GroupDocs.Signature for Java-API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ist eine beliebte API für die elektronische Unterzeichnung digitaler Dokumente. Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten sind verfügbar. Signaturen können auf PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten platziert werden. Kunden können ihr Dokument signieren und elektronische Signaturen, die auf diesen Dokumenten angebracht wurden, aktualisieren, suchen, überprüfen, löschen oder in der Vorschau anzeigen. Darüber hinaus werden viele Möglichkeiten zur Anpassung von Signaturen bereitgestellt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Schritte zum Signieren von Tiff mit Metadata in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bietet die Möglichkeit, Tiff-Dokumente mit Metadata-Signaturen schnell und einfach zu signieren.
        
        * Erstellen Sie eine Instanz der Signature-Klasse, die die Tiff-Datei bereitstellt, die als Pfad oder Speicherstream signiert werden soll
        * Instanziieren Sie die SignOptions-Klasse und legen Sie alle erforderlichen Daten fest.
        * Rufen Sie die Signature.Sign()-Methode auf und übergeben Sie die Tiff-Ausgabedatei oder den Speicherstream

    title_right: "System Requirements"
    content_right: |
        Das Signieren von Dokumenten mit GroupDocs.Signature for Java kann in nur wenigen einfachen Schritten durchgeführt werden. Unsere APIs werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Stellen Sie vor dem Ausführen des folgenden Codes sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Holen Sie sich das neueste GroupDocs.Signature for Java von [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";
        // Set up output file
        String outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Tiff document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Tiff-Dokumenten mit Metadata Live-Demo"
    content: |
       Signieren Sie die Datei Tiff jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Metadata-Signaturen für Java"
    content: |
        "Sie können Tiff auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
       
       
back_to_top:
    enable: true
---