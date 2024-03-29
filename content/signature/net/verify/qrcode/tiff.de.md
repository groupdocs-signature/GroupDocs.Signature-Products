---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Tiff
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Tiff for C#

############################# Head ############################
head_title: "Überprüfung von Qrcode-Signaturen für Tiff-Dateien über C#"
head_description: "Verwenden Sie nur wenige Zeilen .NET-Code, um Tiff-Dokumente und ihre Qrcode-Signaturen zu überprüfen."

############################# Header ############################
title: "Qrcode-Signaturüberprüfung für Tiff-Dateien"
description: "Die API für .NET bietet die Möglichkeit, Qrcode-Signaturen bei Tiff-Dokumenten zu überprüfen. Die Überprüfung elektronischer Signaturen in Ihren Tiff-Dokumenten kann schnell und einfach durchgeführt werden."
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
    title: "Entdecken Sie neue API-Funktionen von GroupDocs.Signature for .NET"
    content: |
        Die [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)-API bietet eine Vielzahl von Möglichkeiten zur Verarbeitung zahlreicher Dokumentformate mithilfe elektronischer Signaturen. Viele Arten von digitalen Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten werden unterstützt. Kunden können digitale Signaturen in PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten hinzufügen, entfernen, bearbeiten, validieren oder suchen. Erstaunlich viele zusätzliche Funktionen und Einstellungen sind verfügbar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "So validieren Sie Qrcode-Signaturen in Ihrem Tiff-Dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) enthält nützliche Funktionen wie die Überprüfung von Qrcode-Signaturen, die in Tiff-Dokumenten platziert wurden. Nutzen Sie diese Gelegenheit, ohne zusätzlichen Code zu implementieren.
        
        * Instanziieren Sie zunächst die Klasse Signature, die als Konstruktorparameter den Pfad zu einem Dokument bereitstellt, das überprüft werden soll.
        * Erstellen Sie zweitens ein neues VerifyOptions-Objekt und richten Sie alle erforderlichen Eigenschaften ein.
        * Rufen Sie schließlich die Verify-Methode des Signature-Objekts auf und übergeben Sie die VerifyOptions-Instanz.
        * Verarbeiten Sie dann die Überprüfungsergebnisse.

    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Signature for .NET werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laden Sie die neueste Version von GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature) herunter
         
    code: |
        ```csharp    
                
        // Set up input Tiff file
        string filePath = "input.tiff";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren mit Qrcode-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zur Datei Tiff hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifizieren Sie andere Qrcode-Signaturen mit C#"
    content: |
        "Überprüfung elektronischer Signaturen in verschiedenen Dokumenten. Überprüfen Sie die Qualität der Unterschriften in den gängigen Dateiformaten wie unten angegeben."
    format: 
       
       
back_to_top:
    enable: true
---