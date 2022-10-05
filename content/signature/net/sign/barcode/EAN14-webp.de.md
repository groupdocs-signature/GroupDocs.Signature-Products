---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N14
fileformat: Webp
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Webp for C#

############################# Head ############################
head_title: "Webp-Dokument mit E A N14-Barcode in C# eSignieren"
head_description: "Erstellen Sie eine E A N14-Barcode-Signatur und fügen Sie sie mit ein paar Codezeilen in ein Webp-Dokument mit .NET ein. Verwenden Sie die GroupDocs Document Signature API zum Signieren verschiedener Dateiformate."

############################# Header ############################
title: "E A N14-Barcode-Signatur für Webp-Dokument in C# generieren"
description: "Unterzeichnen Sie Ihre Webp-Geschäftsdokumente mit E A N14-Barcode. Generieren Sie Barcode-Signaturen schnell und einfach mit wenigen Codezeilen, um Signaturoptionen einzurichten."
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
    title: "{barcode-about.title}"
    content: |
        {barcode-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{barcode-steps.title}"
    content_left: |
        {barcode-steps.content.description}
        
        * {barcode-steps.content.step_1}
        * {barcode-steps.content.step_2}
        * {barcode-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * {system-requirements.content.step_3}
         
    code: |
        ```csharp    
        
        // Set up input Webp file
        string filePath = "input.webp";
        // Set up output file
        string outputFilePath = "output.webp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.E A N14,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Webp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Webp-Dokumenten mit Barcode Live-Demo"
    content: |
       Signieren Sie die Datei Webp jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N14 Barcode"
          content: |
            Die Europäische Artikelnummer oder EAN ist ein Standard, der eine Barcode-Symbologie und ein Nummerierungssystem beschreibt, das im globalen Handel verwendet wird, um einen bestimmten Einzelhandelsprodukttyp in einer bestimmten Verpackungskonfiguration von einem bestimmten Hersteller zu identifizieren.
          characterset: |
             Numerische Ziffern (0-9) und Sonderzeichen.
          textcapacity: |
             Genau 14 Ziffern.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Barcode-Signaturen für C#"
    content: |
        "Sie können Webp auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
        
       
back_to_top:
    enable: true
---