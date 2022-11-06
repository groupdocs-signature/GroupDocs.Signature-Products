---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Doc
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Doc for C#

############################# Head ############################
head_title: "Opdater Image signaturer placeret på Doc filer med C#"
head_description: "Brug enkel og nem at forstå .NET-koden til opdatering af Image-signaturer i signerede {{Filformat}}-dokumenter."

############################# Header ############################
title: "Rediger og opdater Image signaturer placeret på {{Filformat}} filer"
description: "API for .NET giver funktionalitet til Image signaturer, der opdateres i {{Filformat}} dokumenter. Opdater e-signaturer i dine {{Filformat}} dokumenter med et par linjer med C# kode hurtigt og nemt."
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
    title: "Lær om GroupDocs.Signature for .NET API-funktioner"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API-funktionalitet indeholder et stort udvalg af metoder til at behandle efterspurgte dokumentformater ved at bruge elektroniske signaturer. Bredt spektrum af e-signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata understøttes. Kunder kan tilføje, fjerne, redigere, validere eller søge i digitale signaturer i PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Adskillige nyttige funktioner og indstillinger er tilgængelige.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Sådan ændrer du Image-signaturer i dit {{Filformat}}-dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inkluderer nyttige funktioner som f.eks. opdatering af Image signaturer placeret på Doc dokumenter. Det gør det muligt at ændre signaturfunktioner uden ekstra kode.
        
        * Til at starte med skal du oprette signaturobjekt, der passerer som en konstruktørparametersti til et dokument, som formodes at blive opdateret.
        * Instantiér derefter et passende bestemt signaturobjekt og opsæt dets identifikator og egenskaber, som skal ændres.
        * Til sidst skal du kalde Signatures opdateringsmetode, der sender et bestemt signaturobjekt.
        * Behandle opdatering af resultater til din meddelelse.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download den seneste version af GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Opdatering af Image-signaturerne på dokumentsiderne - Live Demo"
    content: |
       Rediger forskellige elektroniske signaturer af Doc-dokumentet lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Opdater forskellige Image-signaturer via C#"
    content: |
        "Redigering af digitale signaturer, som er placeret i forskellige dokumentformater. Opdater signaturdata uden ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---