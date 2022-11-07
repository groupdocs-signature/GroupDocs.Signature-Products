---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Ppsm
productName: .NET
lang: sl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Ppsm for C#

############################# Head ############################
head_title: "Preverjanje podpisov Qrcode za datoteke Ppsm prek C#"
head_description: "Uporabite samo nekaj vrstic kode .NET za preverjanje dokumentov Ppsm in njihovih podpisov Qrcode."

############################# Header ############################
title: "Preverjanje podpisov Qrcode za datoteke Ppsm"
description: "API za .NET ponuja možnost preverjanja podpisov Qrcode v dokumentih Ppsm. Preverjanje e-podpisov v vaših Ppsm dokumentih lahko izvedete hitro in enostavno."
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
    title: "Odkrijte nove funkcije API-ja GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API ponuja široko paleto načinov za obdelavo številnih formatov dokumentov z uporabo elektronskih podpisov. Podprte so številne vrste digitalnih podpisov, kot so besedila, slike, digitalna potrdila, črtne kode, kode QR, žigi ali metapodatki. Stranke lahko dodajajo, odstranjujejo, urejajo, preverjajo ali iščejo digitalne podpise v PDF-jih, dokumentih MS Word, delovnih zvezkih MS Excel, predstavitvah MS PowerPoint, datotekah Adobe Photoshop in različnih formatih slik. Na voljo je osupljivo število dodatnih funkcij in nastavitev.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako potrditi podpise Qrcode v dokumentu Ppsm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) vključuje uporabne funkcije, kot je preverjanje podpisov Qrcode v dokumentih Ppsm. Izkoristite to priložnost brez implementacije dodatne kode.
        
        * Najprej ustvarite razred Signature, ki kot parameter konstruktorja zagotovi pot do dokumenta, ki naj bi bil preverjen.
        * Drugič, ustvarite nov objekt VerifyOptions in nastavite vse zahtevane lastnosti.
        * Nazadnje pokličite metodo Verify objekta Signature, ki posreduje instanco VerifyOptions.
        * Nato obdelajte rezultate preverjanja.

    title_right: "Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for .NET so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Prenesite najnovejšo različico GroupDocs.Signature for .NET iz [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ppsm file
        string filePath = "input.ppsm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
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
    title: "Podpisovanje s podpisi Qrcode Demo v živo"
    content: |
       Takoj dodajte različne elektronske podpise v datoteko Ppsm tako, da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Preverite druge podpise Qrcode z uporabo C#"
    content: |
        "Preverjanje elektronskih podpisov v različnih dokumentih. Preverite kakovost podpisov v priljubljenih formatih datotek, kot je prikazano spodaj."
    format: 
       
       
back_to_top:
    enable: true
---