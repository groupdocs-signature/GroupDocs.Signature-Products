---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCE
fileformat: Pdf
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pdf for C#

############################# Head ############################
head_title: "Pdf-Dokument mit UPCE-Barcode in C# eSignieren"
head_description: "Erstellen Sie eine UPCE-Barcode-Signatur und fügen Sie sie mit ein paar Codezeilen in ein Pdf-Dokument mit .NET ein. Verwenden Sie die GroupDocs Document Signature API zum Signieren verschiedener Dateiformate."

############################# Header ############################
title: "UPCE-Barcode-Signatur für Pdf-Dokument in C# generieren"
description: "Unterzeichnen Sie Ihre Pdf-Geschäftsdokumente mit UPCE-Barcode. Generieren Sie Barcode-Signaturen schnell und einfach mit wenigen Codezeilen, um Signaturoptionen einzurichten."
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
    title_left: "Schritte zum Signieren von Pdf mit Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet die Möglichkeit, Pdf-Dokumente mit Barcode-Signaturen schnell und einfach zu signieren.
        
        * Erstellen Sie eine Instanz der Signature-Klasse, die die Pdf-Datei bereitstellt, die als Pfad oder Speicherstream signiert werden soll
        * Instanziieren Sie die SignOptions-Klasse und legen Sie alle erforderlichen Daten fest.
        * Rufen Sie die Signature.Sign()-Methode auf und übergeben Sie die Pdf-Ausgabedatei oder den Speicherstrom

    title_right: " System Anforderungen"
    content_right: |
        GroupDocs.Signature for .NET werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Holen Sie sich das neueste GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pdf file
        string filePath = "input.pdf";
        // Set up output file
        string outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.UPCE,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Pdf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Pdf-Dokumenten mit Barcode Live-Demo"
    content: |
       Signieren Sie die Datei Pdf jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCE Barcode"
          content: |
            Der Universal Product Code ist eine Strichcode-Symbologie, die weltweit zur Verfolgung von Handelsartikeln in Geschäften verwendet wird. UPCE ist eine 8-stellige Variation von UPC.
          characterset: |
             Unterstützt nur numerische Ziffern (0-9).
          textcapacity: |
             Codetextkapazität: genau 7 Ziffern + 1 Prüfziffer.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAEAAAABjCAYAAAArUQZGAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAUTSURBVHhe7ZBBqmQBCAP7/pfuMUwXyMcIkuV7BRK1wIWf78N5H/DLx/I+4JeP5X3ALx/L+oDP57/+m0I9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE548xDeB/zysbwP+OVjefgDvt9/E/iHbcwlZ5QAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Barcode-Signaturen für C#"
    content: |
        "Sie können Pdf auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
        
       
back_to_top:
    enable: true
---