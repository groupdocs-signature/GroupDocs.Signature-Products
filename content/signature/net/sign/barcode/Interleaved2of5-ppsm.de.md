---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Ppsm
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ppsm for C#

############################# Head ############################
head_title: "Ppsm-Dokument mit Interleaved2of5-Barcode in C# eSignieren"
head_description: "Erstellen Sie eine Interleaved2of5-Barcode-Signatur und fügen Sie sie mit ein paar Codezeilen in ein Ppsm-Dokument mit .NET ein. Verwenden Sie die GroupDocs Document Signature API zum Signieren verschiedener Dateiformate."

############################# Header ############################
title: "Interleaved2of5-Barcode-Signatur für Ppsm-Dokument in C# generieren"
description: "Unterzeichnen Sie Ihre Ppsm-Geschäftsdokumente mit Interleaved2of5-Barcode. Generieren Sie Barcode-Signaturen schnell und einfach mit wenigen Codezeilen, um Signaturoptionen einzurichten."
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
    title: "Über GroupDocs.Signature for .NET Strichcode-Signaturen-API."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ist eine schnelle und einfache API zur Verwaltung digitaler Dokumente mit elektronischen Signaturen unter Verwendung von Barcode-Typen wie UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 und viele andere. Kunden können auf einfache Weise Barcodes mit dem erforderlichen Text erstellen und diese in PDF-Dateien, Microsoft Office Words-Dokumente, Microsoft Office Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedene Bildformate einfügen. In Dokumenten platzierte Barcodes können entweder aktualisiert, durchsucht, verifiziert, gelöscht oder in der Vorschau angezeigt werden. Darüber hinaus wird die Anpassung von Barcodes unterstützt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Schritte zum Signieren von Ppsm mit Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet die Möglichkeit, Ppsm-Dokumente mit Barcode-Signaturen schnell und einfach zu signieren.
        
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

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Interleaved2of5,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ppsm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Ppsm-Dokumenten mit Barcode Live-Demo"
    content: |
       Signieren Sie die Datei Ppsm jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) ist eine kontinuierliche Barcode-Symbologie mit zwei Breiten, die Ziffern codiert. Es wird kommerziell auf 135-Folie, für ITF-14-Barcodes und auf Kartons einiger Produkte verwendet, während die Produkte darin mit UPC oder EAN gekennzeichnet sind.
          characterset: |
             Numerische Ziffern (0-9).
          textcapacity: |
             Variable Länge.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Barcode-Signaturen für C#"
    content: |
        "Sie können Ppsm auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
        
       
back_to_top:
    enable: true
---