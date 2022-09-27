---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Ott
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Ott with C#

############################# Head ############################
head_title: "Suche nach Image-Signaturen in der Datei Ott in C#"
head_description: "Verwenden Sie .NET für die Suche nach Image-Signaturen in Ott-Dateien mit ein paar Zeilen Code."

############################# Header ############################
title: "Suchen Sie nach Image-Signaturen in der Datei Ott"
description: "Die native API von .NET ermöglicht die Suche nach Image-Signaturen in bereits signierten Ott-Dateien. Führen Sie mit wenigen Codezeilen eine erweiterte E-Signatur-Suche in Ihren Ott-Dokumenten durch."
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
    title_left: "So suchen Sie nach Image-Signaturen in Ott"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) erleichtert Entwicklern von .NET die Suche nach Image-Signaturen in Ott-Dateien aus ihren Anwendungen, indem einige einfache Schritte implementiert werden.
        
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
                
        // Set up input Ott file
        string filePath = "input.ott";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Ott document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren mit Image-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zu Ott-Dateien hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Suchen Sie mit C# nach anderen Image-Signaturen"
    content: |
        "Elektronische Signaturen suchen in verschiedenen Dokumenten. Finden Sie Signaturen in einem der gängigen Dateiformate, wie unten gezeigt."
    format: 
           
       
back_to_top:
    enable: true
---