---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Xltx
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltx for C#

############################# Head ############################
head_title: "Bekræftelse af Digital signaturer for Xltx filer via C#"
head_description: "Brug kun et par linjer med .NET-kode til at bekræfte Xltx-dokumenter og deres Digital-signaturer."

############################# Header ############################
title: "Digital signaturbekræftelse for {{Filformat}} filer"
description: "API for .NET giver mulighed for at bekræfte Digital-signaturer på Xltx-dokumenter. Bekræftelse af e-signaturer i dine {{Filformat}}-dokumenter kan udføres hurtigt og nemt."
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
    title: "Oplev nye GroupDocs.Signature for .NET API-funktioner"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API giver en bred vifte af måder at behandle adskillige dokumentformater ved at bruge elektroniske signaturer. Mange typer digitale signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata understøttes. Kunder kan tilføje, fjerne, redigere, validere eller søge i digitale signaturer i PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Et forbløffende antal ekstra funktioner og indstillinger er tilgængelige.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Sådan validerer du Digital-signaturer i dit {{Filformat}}-dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inkluderer nyttige funktioner såsom bekræftelse af Digital signaturer placeret på Xltx dokumenter. Brug denne mulighed uden at implementere ekstra kode.
        
        * For det første instansierer Signature-klassen, der som en konstruktørparametersti til et dokument, der formodes at være verificeret.
        * For det andet skal du oprette et nyt VerifyOptions-objekt og opsætte alle nødvendige egenskaber.
        * Til sidst påkalder du Signatures objekt Verify-metode, der passerer VerifyOptions-instansen.
        * Behandl derefter verifikationsresultaterne.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download den seneste version af GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltx file
        string filePath = "input.xltx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
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
    title: "Signering med Digital signaturer Live Demo"
    content: |
       Føj forskellige elektroniske signaturer til filen Xltx lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bekræft andre Digital-signaturer ved hjælp af C#"
    content: |
        "Verifikation af elektroniske signaturer placeret i forskellige dokumenter. Tjek kvaliteten af ​​signaturer i de populære filformater som vist nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---