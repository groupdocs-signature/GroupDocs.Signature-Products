---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xltm
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltm for C#

############################# Head ############################
head_title: "Slet Digital signaturer fra Xltm filer via C#"
head_description: "Sletning af specifikke Digital-signaturer fra signerede Xltm-dokumenter kan udføres nemt med en kort .NET-kode."

############################# Header ############################
title: "Fjern Digital-signaturer, der er placeret i Xltm-filer"
description: "Slet forskellige Digital-signaturer fra Xltm-dokumenter. Fjernelse af Digital signaturer kræver simpel C# kode."
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
    title: "Få oplysninger om GroupDocs.Signature for .NET API-funktioner"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API giver mange måder at behandle dine dokumenter ved hjælp af elektroniske signaturer. Digitale signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata er tilgængelige. Kunder har mulighed for at tilføje, slette, opdatere, verificere eller søge i digitale signaturer i PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Der er et stort antal nyttige funktioner og indstillinger.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Sådan fjerner du Digital-signaturer fra dit Xltm-dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) giver nyttige funktioner til at rydde Xltm dokumenter for Digital signaturer med et par linjer kode.
        
        * For det første skal du instansiere Signatur-objektets sti til dit dokument som en konstruktørparameter.
        * Opret derefter et passende signaturobjekt og opsæt dets unikke identifikator.
        * Kald derefter Slet-metoden, der passerer signaturobjekt, som skal slettes.
        * Endelig resultat af procesdrift.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download den seneste version af GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltm file
        string filePath = "input.xltm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering med Digital signaturer Live Demo"
    content: |
       Føj forskellige elektroniske signaturer til filen Xltm lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Slet dine Digital-signaturer med C#"
    content: |
        "Sletning af e-signaturer som blev tilføjet til forskellige dokumentformater. Fjern signaturer hurtigt uden ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---