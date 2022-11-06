---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Ods
productName: .NET
lang: af
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Ods with C#

############################# Head ############################
head_title: "Soek vir Image handtekeninge in Ods lêer in C#"
head_description: "Gebruik .NET om na Image-handtekeninge in Ods-lêers te soek deur 'n paar reëls kode te gebruik."

############################# Header ############################
title: "Soek vir Image handtekeninge in Ods lêer"
description: ".NET se inheemse API laat toe om vir Image handtekeninge te soek in reeds ondertekende Ods lêers. Voer gevorderde e-handtekeningsoektog binne jou {{Lêerformaat}} dokumente uit deur 'n paar reëls kode te gebruik."
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
    title_left: "Hoe om te soek vir Image handtekeninge in {{Lêerformaat}}"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) maak dit makliker vir .NET-ontwikkelaars om vir Image-handtekeninge in Ods-lêers vanaf hul toepassings te soek deur 'n paar maklike stappe te implementeer.
        
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
                
        // Set up input Ods file
        string filePath = "input.ods";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Ods document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Soek vir Image elektroniese handtekeninge Live Demo"
    content: |
       Deursoek die dokument vir verskeie elektroniese handtekeninge vir Ods lêers op die oomblik deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Soek vir ander Image handtekeninge deur C# te gebruik"
    content: |
        "Elektroniese handtekeninge soek in verskeie dokumente. Soek handtekeninge van die een van die gewilde lêerformate soos hieronder getoon."
    format: 
           
       
back_to_top:
    enable: true
---