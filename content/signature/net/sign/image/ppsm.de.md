---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Ppsm
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Ppsm for C#

############################# Head ############################
head_title: "Hinzufügen von Image-Signaturen zur Ppsm-Datei mit C#"
head_description: "Fügen Sie die Image-Signatur in die Ppsm-Datei für .NET ein, indem Sie ein paar Codezeilen verwenden. Verwenden Sie die GroupDocs Document Signature API, um Dutzende von Dateiformaten zu signieren."

############################# Header ############################
title: "Signiere Ppsm-Dateien mit Image-Signaturen in C#"
description: "So fügen Sie eine Image-Signatur mit ein paar Zeilen .NET-Code hinzu"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Signature for .NET Bildsignaturen-API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ist eine beliebte API für die elektronische Unterzeichnung digitaler Dokumente. Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten sind verfügbar. Signaturen können auf PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten platziert werden. Kunden können ihr Dokument signieren und elektronische Signaturen, die auf diesen Dokumenten angebracht wurden, aktualisieren, suchen, überprüfen, löschen oder in der Vorschau anzeigen. Darüber hinaus werden viele Möglichkeiten zur Anpassung von Signaturen bereitgestellt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Schritte zum Signieren von Ppsm mit Image in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet die Möglichkeit, Ppsm-Dokumente mit Image-Signaturen schnell und einfach zu signieren.
        
        * Erstellen Sie eine Instanz der Signature-Klasse, die die Ppsm-Datei bereitstellt, die als Pfad oder Speicherstream signiert werden soll
        * Instanziieren Sie die SignOptions-Klasse und legen Sie alle erforderlichen Daten fest.
        * Rufen Sie die Signature.Sign()-Methode auf und übergeben Sie die Ppsm-Ausgabedatei oder den Speicherstrom

    title_right: " System Anforderungen"
    content_right: |
        GroupDocs.Signature for .NET werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Holen Sie sich das neueste GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ppsm file
        string filePath = "input.ppsm";
        // Set up output file
        string outputFilePath = "output.ppsm";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Ppsm document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Ppsm-Dokumenten mit Image Live-Demo"
    content: |
       Signieren Sie die Datei Ppsm jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Image-Signaturen für C#"
    content: |
        "Sie können Ppsm auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
       
       
back_to_top:
    enable: true
---