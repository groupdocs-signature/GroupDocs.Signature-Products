---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Ott
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Ott for C#

############################# Head ############################
head_title: "Opret elektroniske tekstsignaturer til filen Ott med C#"
head_description: "Sæt Text eSignature på filen Ott for .NET ved hjælp af et par linjer kode. Brug GroupDocs Document Signature API til at signere snesevis af filformater."

############################# Header ############################
title: "Signer {{Filformat}}-filer med Text-signaturer i C#"
description: "Sådan tilføjer du Text-signatur med et par linjer med .NET-kode"
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
    title: "Om GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er en populær API til e-signering af digitale dokumenter. Signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata er tilgængelige. Signaturer kan placeres på PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Kunder kan underskrive deres dokument og opdatere, søge, verificere, slette eller forhåndsvise e-signaturer, der blev sat på disse dokumenter. Desuden er der en masse muligheder for signaturtilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trin til at signere {{Filformat}} med Text i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) giver mulighed for at signere Ott dokumenter med Text signaturer hurtigt og nemt.
        
        * Opret en forekomst af signaturklassen, der leverer Ott-fil, der skal signere som sti eller hukommelsesstrøm
        * Instantiér SignOptions-klassen og indstil alle krævede data.
        * Kald Signature.Sign()-metoden ved at sende output Ott-fil eller hukommelsesstrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den seneste GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ott file
        string filePath = "input.ott";
        // Set up output file
        string outputFilePath = "output.ott";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Ott document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering af {{Filformat}} dokumenter med Text Live Demo"
    content: |
       Signer Ott-filen med forskellige signaturer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis online demo venter på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre understøttede Text-signaturer for C#"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Se venligst listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---