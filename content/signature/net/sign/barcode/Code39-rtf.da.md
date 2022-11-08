---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Code39
fileformat: Rtf
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Rtf for C#

############################# Head ############################
head_title: "eSign Rtf dokument med Code39 stregkode i C#"
head_description: "Opret Code39 stregkodesignatur og læg den på Rtf dokument med .NET ved hjælp af et par linjer kode. Brug GroupDocs Document Signature API til at signere forskellige filformater."

############################# Header ############################
title: "Generer Code39 Stregkodesignatur for Rtf dokument i C#"
description: "eSignér dine Rtf forretningsdokumenter med Code39 stregkode. Generer stregkodesignatur hurtigt og nemt med et par linjer kode for at opsætte signeringsmuligheder."
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
    title: "Om GroupDocs.Signature for .NET stregkodesignatur-API."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er en hurtig og nem API til at administrere digitale dokumenter e-signering ved hjælp af stregkodetyper som UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 og mange andre. Kunder kan nemt oprette stregkoder, der giver den nødvendige tekst og lægge dem på PDF, Microsoft Office Words-dokumenter, Microsoft Office Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Stregkoder placeret i dokumenter kan enten opdateres, søges, verificeres, slettes eller forhåndsvises. Desuden understøttes stregkodertilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trin til at signere Rtf med Barcode i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) giver mulighed for at signere Rtf dokumenter med Barcode signaturer hurtigt og nemt.
        
        * Opret en forekomst af signaturklassen, der leverer Rtf-fil, der skal signere som sti eller hukommelsesstrøm
        * Instantiér SignOptions-klassen og indstil alle krævede data.
        * Kald Signature.Sign()-metoden ved at sende output Rtf-fil eller hukommelsesstrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den seneste GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Rtf file
        string filePath = "input.rtf";
        // Set up output file
        string outputFilePath = "output.rtf";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Code39,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Rtf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering af Rtf dokumenter med Barcode Live Demo"
    content: |
       Signer Rtf-filen med forskellige signaturer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis online demo venter på dig.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Code39 Barcode"
          content: |
            Kode 39 (også kendt som Alpha39, Kode 3 af 9, Kode 3/9, Type 39, USS Kode 39 eller USD-3) er en diskret stregkodesymbolologi med variabel længde.
          characterset: |
             Numeriske cifre (0-9) og store bogstaver (A-Z) og et antal specialtegn (-, ., $, /, +, % og mellemrum).
          textcapacity: |
             Ingen specifikke restriktioner.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre understøttede Barcode-signaturer for C#"
    content: |
        "Du kan også signere Rtf med andre signaturtyper. Se venligst listen nedenfor."
    format: 
        
       
back_to_top:
    enable: true
---