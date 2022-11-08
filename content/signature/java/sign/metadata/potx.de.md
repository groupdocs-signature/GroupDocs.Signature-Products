---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Potx
productName: Java
lang: de
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Potx for Java

############################# Head ############################
head_title: "Elektronische Metadaten-Signaturen an Potx-Dokumente über Java anhängen"
head_description: "Verwenden Sie Metadaten als versteckte elektronische Signaturen in Ihren Potx-Dokumenten mit ein paar Zeilen Java-Code. Verwenden Sie die GroupDocs Document Signature API, um Ihre Geschäftsdokumente und Dateien mit Metadateninformationen elektronisch zu signieren."

############################# Header ############################
title: "Elektronische Metadaten-Signaturen für das Dokument Potx über Java sind einfach und benutzerfreundlich!"
description: "Unterschreiben Sie Ihre Potx-Dokumente und Verträge mit versteckten Metadateneinträgen. Generieren Sie Metadaten für PDFs, MS Word-Dokumente, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen und verschiedene Bildformate ohne Probleme und zusätzliche Codierung."
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
    title: "Über GroupDocs.Signature for Java Metadaten-Signaturen-API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ist eine beliebte API für die elektronische Unterzeichnung digitaler Dokumente. Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten sind verfügbar. Signaturen können auf PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten platziert werden. Kunden können ihr Dokument signieren und elektronische Signaturen, die auf diesen Dokumenten angebracht wurden, aktualisieren, suchen, überprüfen, löschen oder in der Vorschau anzeigen. Darüber hinaus werden viele Möglichkeiten zur Anpassung von Signaturen bereitgestellt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Schritte zum Signieren von Potx mit Metadata in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bietet die Möglichkeit, Potx-Dokumente mit Metadata-Signaturen schnell und einfach zu signieren.
        
        * Erstellen Sie eine Instanz der Signature-Klasse, die die Potx-Datei bereitstellt, die als Pfad oder Speicherstream signiert werden soll
        * Instanziieren Sie die SignOptions-Klasse und legen Sie alle erforderlichen Daten fest.
        * Rufen Sie die Signature.Sign()-Methode auf und übergeben Sie die Potx-Ausgabedatei oder den Speicherstrom

    title_right: " System Anforderungen"
    content_right: |
        GroupDocs.Signature for Java werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Holen Sie sich das neueste GroupDocs.Signature for Java von [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potx file
        String filePath = "input.potx";
        // Set up output file
        String outputFilePath = "output.potx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Potx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Potx-Dokumenten mit Metadata Live-Demo"
    content: |
       Signieren Sie die Datei Potx jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Metadata-Signaturen für Java"
    content: |
        "Sie können Potx auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
       
       
back_to_top:
    enable: true
---