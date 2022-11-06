---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Xlsx
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Xlsx with C#

############################# Head ############################
head_title: "Søg efter Metadata signaturer i filen {{Filformat}} i C#"
head_description: "Brug .NET til at søge efter Metadata-signaturer i Xlsx-filer ved hjælp af et par linjer kode."

############################# Header ############################
title: "Søg efter Metadata-signaturer i filen {{Filformat}}"
description: ".NET native API gør det muligt at søge efter Metadata-signaturer i allerede signerede Xlsx-filer. Udfør avanceret e-signatursøgning i dine {{Filformat}} dokumenter ved hjælp af et par linjer kode."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Om GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) giver .NET API til behandling af dokumenter ved hjælp af forskellige signaturtyper såsom tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata. Brugere kan tilføje, slette, opdatere, verificere eller søge i elektroniske signaturer i PDF'er, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater, med yderligere støtte til at tilpasse signaturegenskaber efter behov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Sådan søger du efter Metadata-signaturer i {{Filformat}}"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gør det nemmere for .NET-udviklere at søge efter Metadata-signaturer i Xlsx-filer fra deres applikationer ved at implementere nogle få nemme trin.
        
        * Opret en ny forekomst af Signature-klassen og videregiv kildedokumentstien som en konstruktørparameter.
        * Instantiér SearchOptions-objektet i overensstemmelse med dine krav, og angiv søgeindstillinger.
        * Kald søgemetoden for Signature-klasseforekomsten og send SearchOptions til den.
        * Bearbejd søgeresultater i overensstemmelse med dine krav.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download den seneste version af GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xlsx file
        string filePath = "input.xlsx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Xlsx document
                List<SpreadsheetMetadataSignature> signatures = signature.Search<SpreadsheetMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (SpreadsheetMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Søg efter Metadata elektroniske signaturer Live Demo"
    content: |
       Søg i dokumentet efter forskellige elektroniske signaturer til Xlsx-filer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Søg efter andre Metadata-signaturer ved hjælp af C#"
    content: |
        "Elektroniske signaturer søger i forskellige dokumenter. Find signaturer fra et af de populære filformater som vist nedenfor."
    format: 
           
       
back_to_top:
    enable: true
---