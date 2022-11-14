---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Csv
productName: .NET
lang: no
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Csv with C#

############################# Head ############################
head_title: "Søk etter Text-signaturer i filen {{Filformat}} i C#"
head_description: "Bruk .NET for å søke etter Text-signaturer i Csv-filer ved å bruke noen få linjer med kode."

############################# Header ############################
title: "Søk etter Text-signaturer i filen {{Filformat}}"
description: ".NET native API gjør det mulig å søke etter Text-signaturer i allerede signerte Csv-filer. Utfør avansert e-signatursøk i Csv-dokumentene dine ved å bruke noen få linjer med kode."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gir .NET API for behandling av dokumenter ved hjelp av ulike signaturtyper som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, stempler eller metadata. Brukere kan legge til, slette, oppdatere, bekrefte eller søke i elektroniske signaturer i PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater, med ekstra støtte for å tilpasse signaturegenskaper etter behov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Slik søker du etter Text-signaturer i {{Filformat}}"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gjør det enklere for .NET-utviklere å søke etter Text-signaturer i Csv-filer fra applikasjonene deres ved å implementere noen få enkle trinn.
        
        * Opprett en ny forekomst av Signature-klassen og send kildedokumentbanen som en konstruktørparameter.
        * Instantier SearchOptions-objektet i henhold til dine krav og spesifiser søkealternativer.
        * Ring søkemetoden til Signature-klassenforekomsten og send SearchOptions til den.
        * Behandle søkeresultater i henhold til dine krav.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Last ned den nyeste versjonen av GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Csv file
        string filePath = "input.csv";

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

                // search for Text signatures in Csv document
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
    title: "Søk etter Text elektroniske signaturer Live Demo"
    content: |
       Søk i dokumentet etter ulike elektroniske signaturer til Csv-filer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Søk etter andre Text-signaturer med C#"
    content: |
        "Elektroniske signaturer søk i ulike dokumenter. Finn signaturer fra et av de populære filformatene som vist nedenfor."
    format: 
           
       
back_to_top:
    enable: true
---