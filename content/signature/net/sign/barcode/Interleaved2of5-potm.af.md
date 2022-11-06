---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Potm
productName: .NET
lang: af
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Potm for C#

############################# Head ############################
head_title: "eSign {{Lêerformaat}}-dokument met Interleaved2of5 Strepiekode in C#"
head_description: "Skep Interleaved2of5 Strepiekode Handtekening en plaas dit op Potm dokument met .NET deur 'n paar reëls kode te gebruik. Gebruik die GroupDocs Document Signature API vir die ondertekening van verskeie lêerformate."

############################# Header ############################
title: "Genereer Interleaved2of5 strepieskode-handtekening vir Potm-dokument in C#"
description: "eTeken jou {{Lêerformaat}} besigheidsdokumente met Interleaved2of5 Streepkode. Genereer strepieskode-handtekening vinnig en maklik met 'n paar reëls kode om ondertekenopsies op te stel."
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
    title: "Oor GroupDocs.Signature for .NET Barcode Signatures API."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is 'n vinnige en maklike API om digitale dokumente te bestuur wat e-ondertekening gebruik deur strepieskodetipes soos UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 en vele ander. Kliënte kan maklik strepieskodes skep wat vereiste teks verskaf en dit op PDF, Microsoft Office Words-dokumente, Microsoft Office Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate plaas. Strepiekodes wat in dokumente geplaas word, kan ook opgedateer, deursoek, geverifieer, uitgevee of voorbeskou word. Boonop word die aanpassing van strepieskodes ondersteun.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappe om {{Lêerformaat}} met Barcode in C# te onderteken"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bied die vermoë om {{Lêerformaat}} dokumente met Barcode handtekeninge vinnig en maklik te onderteken.
        
        * Skep 'n instansie van Signature-klas wat Potm-lêer verskaf wat veronderstel is om te onderteken as pad of geheuestroom
        * Instansieer SignOptions-klas en stel alle verlangde data in.
        * Roep die Signature.Sign()-metode deur die uitvoer Potm-lêer of geheuestroom deur te gee

    title_right: " Stelselvereistes"
    content_right: |
        GroupDocs.Signature for .NET word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Kry die nuutste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Potm file
        string filePath = "input.potm";
        // Set up output file
        string outputFilePath = "output.potm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Interleaved2of5,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Potm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Teken {{Lêerformaat}} dokumente met Barcode Regstreekse Demo"
    content: |
       Teken nou die Potm-lêer met verskeie handtekeninge deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek. Gratis aanlyn demo wag vir jou.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) is 'n deurlopende twee-breedte strepieskode simboliek wat syfers enkodering. Dit word kommersieel gebruik op 135 film, vir ITF-14 strepieskodes, en op kartonne van sommige produkte, terwyl die produkte binne met UPC of EAN gemerk is.
          characterset: |
             Numeriese syfers (0-9).
          textcapacity: |
             Veranderlike lengte.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ander ondersteunde Barcode handtekeninge vir C#"
    content: |
        "Jy kan ook {{Lêerformaat}} met ander handtekeningtipes onderteken. Sien asseblief die lys hieronder."
    format: 
        
       
back_to_top:
    enable: true
---