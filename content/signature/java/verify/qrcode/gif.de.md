---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Gif
productName: Java
lang: de
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Gif for Java

############################# Head ############################
head_title: "Überprüfung von Qrcode-Signaturen für Gif-Dateien über Java"
head_description: "Verwenden Sie nur wenige Zeilen Java-Code, um Gif-Dokumente und ihre Qrcode-Signaturen zu überprüfen."

############################# Header ############################
title: "Qrcode-Signaturüberprüfung für Gif-Dateien"
description: "Die API für Java bietet die Möglichkeit, Qrcode-Signaturen bei Gif-Dokumenten zu überprüfen. Die Überprüfung elektronischer Signaturen in Ihren Gif-Dokumenten kann schnell und einfach durchgeführt werden."
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
    title: "Entdecken Sie neue API-Funktionen von GroupDocs.Signature for Java"
    content: |
        Die [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/)-API bietet eine Vielzahl von Möglichkeiten zur Verarbeitung zahlreicher Dokumentformate mithilfe elektronischer Signaturen. Viele Arten von digitalen Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten werden unterstützt. Kunden können digitale Signaturen in PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten hinzufügen, entfernen, bearbeiten, validieren oder suchen. Erstaunlich viele zusätzliche Funktionen und Einstellungen sind verfügbar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "So validieren Sie Qrcode-Signaturen in Ihrem Gif-Dokument"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) enthält nützliche Funktionen wie die Überprüfung von Qrcode-Signaturen, die in Gif-Dokumenten platziert wurden. Nutzen Sie diese Gelegenheit, ohne zusätzlichen Code zu implementieren.
        
        * Instanziieren Sie zunächst die Klasse Signature, die als Konstruktorparameter den Pfad zu einem Dokument bereitstellt, das überprüft werden soll.
        * Erstellen Sie zweitens ein neues VerifyOptions-Objekt und richten Sie alle erforderlichen Eigenschaften ein.
        * Rufen Sie schließlich die Verify-Methode des Signature-Objekts auf und übergeben Sie die VerifyOptions-Instanz.
        * Verarbeiten Sie dann die Überprüfungsergebnisse.

    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Signature for Java werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laden Sie die neueste Version von GroupDocs.Signature for Java von [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) herunter
         
    code: |
        ```java    
                
        // Set up input Gif file
        String filePath = "input.gif";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren mit Qrcode-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zur Datei Gif hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifizieren Sie andere Qrcode-Signaturen mit Java"
    content: |
        "Überprüfung elektronischer Signaturen in verschiedenen Dokumenten. Überprüfen Sie die Qualität der Signaturen in den gängigen Dateiformaten wie unten angegeben."
    format: 
       
       
back_to_top:
    enable: true
---