---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Ppt
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Ppt with C#

############################# Head ############################
head_title: "Søg efter Text signaturer i filen Ppt i C#"
head_description: "Brug .NET til at søge efter Text-signaturer i Ppt-filer ved hjælp af et par linjer kode."

############################# Header ############################
title: "Søg efter Text-signaturer i filen Ppt"
description: ".NET native API gør det muligt at søge efter Text-signaturer i allerede signerede Ppt-filer. Udfør avanceret e-signatursøgning i dine Ppt dokumenter ved hjælp af et par linjer kode."
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
    title_left: "Sådan søger du efter Text-signaturer i Ppt"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gør det nemmere for .NET-udviklere at søge efter Text-signaturer i Ppt-filer fra deres applikationer ved at implementere nogle få nemme trin.
        
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
                
        // Set up input Ppt file
        string filePath = "input.ppt";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Ppt document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Søg efter Text elektroniske signaturer Live Demo"
    content: |
       Søg i dokumentet efter forskellige elektroniske signaturer til Ppt-filer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Søg efter andre Text-signaturer ved hjælp af C#"
    content: |
        "Elektroniske signaturer søger i forskellige dokumenter. Find signaturer fra et af de populære filformater som vist nedenfor."
    format: 
           
       
back_to_top:
    enable: true
---