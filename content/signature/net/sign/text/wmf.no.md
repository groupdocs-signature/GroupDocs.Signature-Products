---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Wmf
productName: .NET
lang: no
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Wmf for C#

############################# Head ############################
head_title: "Opprett elektroniske tekstsignaturer til filen Wmf med C#"
head_description: "Sett Text eSignature på Wmf-filen for .NET ved å bruke noen få linjer med kode. Bruk GroupDocs Document Signature API til å signere dusinvis av filformater."

############################# Header ############################
title: "Signer {{Filformat}}-filer med Text-signaturer i C#"
description: "Slik legger du til Text-signatur med noen få linjer med .NET-kode"
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er et populært API for e-signering av digitale dokumenter. Signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, frimerker eller metadata er tilgjengelig. Signaturer kan plasseres på PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og forskjellige bildeformater. Kunder kan signere dokumentet sitt og oppdatere, søke, bekrefte, slette eller forhåndsvise e-signaturer som ble satt på disse dokumentene. Dessuten er det gitt mange muligheter for tilpasning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trinn for å signere {{Filformat}} med Text i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gir mulighet til å signere Wmf-dokumenter med Text-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Wmf-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Wmf eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den siste GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Wmf file
        string filePath = "input.wmf";
        // Set up output file
        string outputFilePath = "output.wmf";

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

                // sign Wmf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av {{Filformat}} dokumenter med Text Live Demo"
    content: |
       Signer Wmf-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Text-signaturer for C#"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---