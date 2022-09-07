---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Dot
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Dot for C#

############################# Head ############################
head_title: "Dot-Dokument mit Pharmacode-Barcode in C# eSignieren"
head_description: "Erstellen Sie eine Pharmacode-Barcode-Signatur und fügen Sie sie mit ein paar Codezeilen in ein Dot-Dokument mit .NET ein. Verwenden Sie die GroupDocs Document Signature API zum Signieren verschiedener Dateiformate."

############################# Header ############################
title: "Pharmacode-Barcode-Signatur für Dot-Dokument in C# generieren"
description: "Unterzeichnen Sie Ihre Dot-Geschäftsdokumente mit Pharmacode-Barcode. Generieren Sie Barcode-Signaturen schnell und einfach mit wenigen Codezeilen, um Signaturoptionen einzurichten."
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
    title: "Über die GroupDocs.Signature for .NET-API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ist eine beliebte API für die elektronische Unterzeichnung digitaler Dokumente mit vielen Barcode-Typen wie UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN, ITF14 und viele andere. Kunden können auf einfache Weise Barcodes erstellen, die nur den erforderlichen Text enthalten, und sie in PDFs, MS Word-Dokumente, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedene Bildformate einfügen. In Dokumenten platzierte Barcodes können entweder aktualisiert, durchsucht, verifiziert, gelöscht oder in der Vorschau angezeigt werden. Darüber hinaus wird die Anpassung von Barcodes unterstützt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Schritte zum Signieren von Dot mit Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet die Möglichkeit, Dot-Dokumente mit Barcode-Signaturen schnell und einfach zu signieren.
        
        * Erstellen Sie eine Instanz der Signature-Klasse, die die Dot-Datei bereitstellt, die als Pfad oder Speicherstream signiert werden soll
        * Instanziieren Sie die SignOptions-Klasse und legen Sie alle erforderlichen Daten fest.
        * Rufen Sie die Signature.Sign()-Methode auf und übergeben Sie die Dot-Ausgabedatei oder den Speicherstream

    title_right: "System Requirements"
    content_right: |
        Das Signieren von Dokumenten mit GroupDocs.Signature for .NET kann in nur wenigen einfachen Schritten durchgeführt werden. Unsere APIs werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Stellen Sie vor dem Ausführen des folgenden Codes sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Holen Sie sich das neueste GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dot file
        string filePath = "input.dot";
        // Set up output file
        string outputFilePath = "output.dot";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Dot document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Dot-Dokumenten mit Barcode Live-Demo"
    content: |
       Signieren Sie die Datei Dot jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, auch bekannt als Pharmaceutical Binary Code, ist ein Barcode-Standard, der in der pharmazeutischen Industrie als Verpackungskontrollsystem verwendet wird.
          characterset: |
             Numerische Ziffern (0-9).
          textcapacity: |
             Stellt nur eine einzelne Ganzzahl von 3 bis 131070 dar.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Barcode-Signaturen für C#"
    content: |
        "Sie können Dot auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
           
       
back_to_top:
    enable: true
---