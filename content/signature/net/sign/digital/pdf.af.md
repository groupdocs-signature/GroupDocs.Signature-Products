---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pdf
productName: .NET
lang: af
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pdf for C#

############################# Head ############################
head_title: "Voeg digitale elektroniese handtekeninge by Pdf-lêer met C#"
head_description: "Plaas digitale handtekening op Pdf-lêer vir .NET deur 'n paar reëls kode te gebruik. Gebruik die GroupDocs Document Signature API om dosyne lêerformate te onderteken."

############################# Header ############################
title: "eSign Pdf lêers met Digital handtekeninge in C#"
description: "Hoe om Digital handtekening by te voeg met 'n paar reëls van .NET kode"
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
    title: "Meer oor GroupDocs.Signature for .NET Digitale handtekening-API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is 'n gewilde API om dokumente te ontwerp met die digitale elektroniese handtekeninge, met digitale sertifikate. Vir die Digitale handtekeninge gebruik API PFX-sertifikaatlêers om dokumente met wagwoordbeskermde private en publieke sleutels te ontwerp. Die digitale handtekeninge kan gebruik word om besigheidsdokumente met eSign PDF-spesifieke bladsy te sertifiseer, hele Microsoft Office-dokumente soos Words, Excel, Powerpoint-lêers en Open Office-dokumente te sertifiseer. Kliënte kan die handtekeninge maklik manipuleer, soos om dit te redigeer, te verwyder of aan te pas. Die API bied 'n manier om handtekeninge te soek en te verifieer. Boonop word baie vermoëns vir handtekeningaanpassing verskaf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappe om {{Lêerformaat}} met Digital in C# te onderteken"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bied die vermoë om {{Lêerformaat}} dokumente met Digital handtekeninge vinnig en maklik te onderteken.
        
        * Skep 'n instansie van Signature-klas wat Pdf-lêer verskaf wat veronderstel is om te onderteken as pad of geheuestroom
        * Instansieer SignOptions-klas en stel alle verlangde data in.
        * Roep die Signature.Sign()-metode deur die uitvoer Pdf-lêer of geheuestroom deur te gee

    title_right: " Stelselvereistes"
    content_right: |
        GroupDocs.Signature for .NET word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Kry die nuutste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pdf file
        string filePath = "input.pdf";
        // Set up output file
        string outputFilePath = "output.pdf";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Pdf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Teken {{Lêerformaat}} dokumente met Digital Regstreekse Demo"
    content: |
       Teken nou die Pdf-lêer met verskeie handtekeninge deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek. Gratis aanlyn demo wag vir jou.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ander ondersteunde Digital handtekeninge vir C#"
    content: |
        "Jy kan ook {{Lêerformaat}} met ander handtekeningtipes onderteken. Sien asseblief die lys hieronder."
    format: 
       
       
back_to_top:
    enable: true
---