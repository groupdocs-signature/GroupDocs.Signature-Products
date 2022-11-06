---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Ott
productName: .NET
lang: af
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Ott with C#

############################# Head ############################
head_title: "Soek vir Qrcode handtekeninge in Ott lêer in C#"
head_description: "Gebruik .NET om na Qrcode-handtekeninge in Ott-lêers te soek deur 'n paar reëls kode te gebruik."

############################# Header ############################
title: "Soek vir Qrcode handtekeninge in Ott lêer"
description: ".NET se inheemse API laat toe om vir Qrcode handtekeninge te soek in reeds ondertekende Ott lêers. Voer gevorderde e-handtekeningsoektog binne jou {{Lêerformaat}} dokumente uit deur 'n paar reëls kode te gebruik."
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
    title: "Oor GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) verskaf .NET API vir die verwerking van dokumente met behulp van verskeie handtekeningtipes soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata. Gebruikers kan elektroniese handtekeninge byvoeg, uitvee, opdateer, verifieer of soek binne PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate, met bykomende ondersteuning vir die pasmaak van handtekeningeienskappe soos benodig.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe om te soek vir Qrcode handtekeninge in {{Lêerformaat}}"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) maak dit makliker vir .NET-ontwikkelaars om vir Qrcode-handtekeninge in Ott-lêers vanaf hul toepassings te soek deur 'n paar maklike stappe te implementeer.
        
        * Skep 'n nuwe instansie van Signature-klas en gee brondokumentpad as 'n konstruktorparameter deur.
        * Instansieer die SearchOptions-objek volgens jou vereistes en spesifiseer soekopsies.
        * Bel Soekmetode van Signature-klasinstansie en gee SearchOptions daaraan.
        * Verwerk soekresultate volgens jou vereistes.

    title_right: "Stelselvereistes"
    content_right: |
        GroupDocs.Signature for .NET word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laai die nuutste weergawe van GroupDocs.Signature for .NET af vanaf [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ott file
        string filePath = "input.ott";

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

                // search for Qrcode signatures in Ott document
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
    title: "Soek vir Qrcode elektroniese handtekeninge Live Demo"
    content: |
       Deursoek die dokument vir verskeie elektroniese handtekeninge vir Ott lêers op die oomblik deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Soek vir ander Qrcode handtekeninge deur C# te gebruik"
    content: |
        "Elektroniese handtekeninge soek in verskeie dokumente. Soek handtekeninge van die een van die gewilde lêerformate soos hieronder getoon."
    format: 
           
       
back_to_top:
    enable: true
---