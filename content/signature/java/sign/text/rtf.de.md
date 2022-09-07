---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Rtf
productName: Java
lang: de
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Rtf for Java

############################# Head ############################
head_title: "Hinzufügen von Text-Signaturen zur Rtf-Datei mit Java"
head_description: "Fügen Sie die Text-Signatur in die Rtf-Datei für Java ein, indem Sie ein paar Codezeilen verwenden. Verwenden Sie die GroupDocs Document Signature API, um Dutzende von Dateiformaten zu signieren."

############################# Header ############################
title: "Signiere Rtf-Dateien mit Text-Signaturen in Java"
description: "So fügen Sie eine Text-Signatur mit ein paar Zeilen Java-Code hinzu"
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
    title_left: "Schritte zum Signieren von Rtf mit Text in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bietet die Möglichkeit, Rtf-Dokumente mit Text-Signaturen schnell und einfach zu signieren.
        
        * Erstellen Sie eine Instanz der Signature-Klasse, die die Rtf-Datei bereitstellt, die als Pfad oder Speicherstream signiert werden soll
        * Instanziieren Sie die SignOptions-Klasse und legen Sie alle erforderlichen Daten fest.
        * Rufen Sie die Signature.Sign()-Methode auf und übergeben Sie die Rtf-Ausgabedatei oder den Speicherstream

    title_right: "System Requirements"
    content_right: |
        Das Signieren von Dokumenten mit GroupDocs.Signature for Java kann in nur wenigen einfachen Schritten durchgeführt werden. Unsere APIs werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Stellen Sie vor dem Ausführen des folgenden Codes sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Holen Sie sich das neueste GroupDocs.Signature for Java von [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Rtf file
        String filePath = "input.rtf";
        // Set up output file
        String outputFilePath = "output.rtf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Rtf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Rtf-Dokumenten mit Text Live-Demo"
    content: |
       Signieren Sie die Datei Rtf jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Text-Signaturen für Java"
    content: |
        "Sie können Rtf auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
       
       
back_to_top:
    enable: true
---