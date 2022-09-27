---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Doc
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Doc with C#

############################# Head ############################
head_title: "Suche nach Qrcode-Signaturen in der Datei Doc in C#"
head_description: "Verwenden Sie .NET für die Suche nach Qrcode-Signaturen in Doc-Dateien mit ein paar Zeilen Code."

############################# Header ############################
title: "Suchen Sie nach Qrcode-Signaturen in der Datei Doc"
description: "Die native API von .NET ermöglicht die Suche nach Qrcode-Signaturen in bereits signierten Doc-Dateien. Führen Sie mit wenigen Codezeilen eine erweiterte E-Signatur-Suche in Ihren Doc-Dokumenten durch."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Über die GroupDocs.Signature for .NET-API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet .NET API zur Verarbeitung von Dokumenten mit verschiedenen Signaturtypen wie Texten, Bildern, digitalen Zertifikaten, Barcodes, QR-Codes, Stempeln oder Metadaten. Benutzer können elektronische Signaturen in PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten hinzufügen, löschen, aktualisieren, überprüfen oder suchen, mit zusätzlicher Unterstützung für die Anpassung von Signatureigenschaften nach Bedarf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "So suchen Sie nach Qrcode-Signaturen in Doc"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) erleichtert Entwicklern von .NET die Suche nach Qrcode-Signaturen in Doc-Dateien aus ihren Anwendungen, indem einige einfache Schritte implementiert werden.
        
        * Erstellen Sie eine neue Instanz der Signature-Klasse und übergeben Sie den Pfad des Quelldokuments als Konstruktorparameter.
        * Instanziieren Sie das SearchOptions-Objekt gemäß Ihren Anforderungen und geben Sie Suchoptionen an.
        * Rufen Sie die Search-Methode der Signature-Klasseninstanz auf und übergeben Sie ihr SearchOptions.
        * Suchergebnisse entsprechend Ihren Anforderungen aufbereiten.

    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Signature for .NET werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laden Sie die neueste Version von GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature) herunter
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Doc document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren mit Qrcode-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zu Doc-Dateien hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Suchen Sie mit C# nach anderen Qrcode-Signaturen"
    content: |
        "Elektronische Signaturen suchen in verschiedenen Dokumenten. Finden Sie Signaturen in einem der gängigen Dateiformate, wie unten gezeigt."
    format: 
           
       
back_to_top:
    enable: true
---