---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Otp
productName: .NET
lang: sl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Otp with C#

############################# Head ############################
head_title: "Poiščite podpise Metadata v datoteki Otp v C#"
head_description: "Uporabite .NET za iskanje podpisov Metadata v datotekah Otp z uporabo nekaj vrstic kode."

############################# Header ############################
title: "Poiščite podpise Metadata v datoteki Otp"
description: "Izvorni API za .NET omogoča iskanje podpisov Metadata v že podpisanih datotekah Otp. Izvedite napredno iskanje e-podpisov znotraj svojih dokumentov Otp z uporabo nekaj vrstic kode."
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
    title: "O API-ju GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ponuja API za .NET za obdelavo dokumentov z uporabo različnih vrst podpisov, kot so besedila, slike, digitalna potrdila, črtne kode, kode QR, žigi ali metapodatki. Uporabniki lahko dodajajo, brišejo, posodabljajo, preverjajo ali iščejo elektronske podpise v datotekah PDF, dokumentih MS Word, delovnih zvezkih MS Excel, predstavitvah MS PowerPoint, datotekah Adobe Photoshop in različnih formatih slik, z dodatno podporo za prilagajanje lastnosti podpisov po potrebi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako poiskati podpise Metadata v Otp"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) razvijalcem za .NET olajša iskanje podpisov Metadata v datotekah Otp iz njihovih aplikacij z implementacijo nekaj preprostih korakov.
        
        * Ustvarite nov primerek razreda Signature in podajte pot izvornega dokumenta kot parameter konstruktorja.
        * Instanciirajte objekt SearchOptions v skladu z vašimi zahtevami in določite možnosti iskanja.
        * Pokličite metodo Search instance razreda Signature in ji posredujte SearchOptions.
        * Rezultate iskanja obdelajte v skladu z vašimi zahtevami.

    title_right: "Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for .NET so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Prenesite najnovejšo različico GroupDocs.Signature for .NET iz [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Otp file
        string filePath = "input.otp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Otp document
                List<PresentationMetadataSignature> signatures = signature.Search<PresentationMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (PresentationMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Iskanje elektronskih podpisov Metadata Predstavitev v živo"
    content: |
       Takoj zdaj poiščite v dokumentu različne elektronske podpise za datoteke Otp tako, da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Išči druge Metadata podpise z C#"
    content: |
        "Iskanje elektronskih podpisov v različnih dokumentih. Poiščite podpise enega od priljubljenih formatov datotek, kot je prikazano spodaj."
    format: 
           
       
back_to_top:
    enable: true
---