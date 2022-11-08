---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Tiff
productName: .NET
lang: sv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Tiff with C#

############################# Head ############################
head_title: "Sök efter Qrcode-signaturer i filen Tiff i C#"
head_description: "Använd .NET för att söka efter Qrcode-signaturer i Tiff-filer med några rader kod."

############################# Header ############################
title: "Sök efter Qrcode-signaturer i filen Tiff"
description: "Inbyggt API för .NET gör det möjligt att söka efter Qrcode-signaturer i redan signerade Tiff-filer. Utför avancerad e-signatursökning i dina Tiff-dokument med några rader kod."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tillhandahåller .NET API för att bearbeta dokument med olika signaturtyper som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata. Användare kan lägga till, ta bort, uppdatera, verifiera eller söka efter elektroniska signaturer i PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat, med ytterligare stöd för att anpassa signaturegenskaper efter behov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hur man söker efter Qrcode-signaturer i Tiff"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gör det enklare för .NET-utvecklare att söka efter Qrcode-signaturer i Tiff-filer från sina applikationer genom att implementera några enkla steg.
        
        * Skapa en ny instans av Signature-klassen och skicka källdokumentsökvägen som en konstruktorparameter.
        * Instantiera SearchOptions-objektet enligt dina krav och ange sökalternativ.
        * Anrop sökmetoden för Signature-klassinstansen och skicka SearchOptions till den.
        * Bearbeta sökresultaten efter dina krav.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ladda ner den senaste versionen av GroupDocs.Signature for .NET från [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Tiff file
        string filePath = "input.tiff";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Tiff document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Sök efter Qrcode elektroniska signaturer Live Demo"
    content: |
       Sök i dokumentet efter olika elektroniska signaturer till Tiff-filer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Sök efter andra Qrcode-signaturer med C#"
    content: |
        "Sök efter elektroniska signaturer i olika dokument. Hitta signaturer från ett av de populära filformaten som visas nedan."
    format: 
           
       
back_to_top:
    enable: true
---