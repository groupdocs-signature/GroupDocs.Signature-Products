---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Docx
productName: .NET
lang: sl
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docx for C#

############################# Head ############################
head_title: "Preverjanje podpisov Digital za datoteke Docx prek C#"
head_description: "Uporabite samo nekaj vrstic kode .NET za preverjanje dokumentov Docx in njihovih podpisov Digital."

############################# Header ############################
title: "Preverjanje podpisov Digital za datoteke Docx"
description: "API za .NET ponuja možnost preverjanja podpisov Digital v dokumentih Docx. Preverjanje e-podpisov v vaših Docx dokumentih lahko izvedete hitro in enostavno."
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
    title_left: "Kako potrditi podpise Digital v dokumentu Docx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) vključuje uporabne funkcije, kot je preverjanje podpisov Digital v dokumentih Docx. Izkoristite to priložnost brez implementacije dodatne kode.
        
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
                
        // Set up input Docx file
        string filePath = "input.docx";

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
    title: "Podpisovanje s podpisi Digital Demo v živo"
    content: |
       Takoj dodajte različne elektronske podpise v datoteko Docx tako, da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Preverite druge podpise Digital z uporabo C#"
    content: |
        "Preverjanje elektronskih podpisov v različnih dokumentih. Preverite kakovost podpisov v priljubljenih formatih datotek, kot je prikazano spodaj."
    format: 
       
       
back_to_top:
    enable: true
---