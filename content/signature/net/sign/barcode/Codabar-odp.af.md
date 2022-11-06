---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Odp
productName: .NET
lang: af
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Odp for C#

############################# Head ############################
head_title: "eSign {{Lêerformaat}}-dokument met Codabar Strepiekode in C#"
head_description: "Skep Codabar Strepiekode Handtekening en plaas dit op Odp dokument met .NET deur 'n paar reëls kode te gebruik. Gebruik die GroupDocs Document Signature API vir die ondertekening van verskeie lêerformate."

############################# Header ############################
title: "Genereer Codabar strepieskode-handtekening vir Odp-dokument in C#"
description: "eTeken jou {{Lêerformaat}} besigheidsdokumente met Codabar Streepkode. Genereer strepieskode-handtekening vinnig en maklik met 'n paar reëls kode om ondertekenopsies op te stel."
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
        
        * Skep 'n instansie van Signature-klas wat Odp-lêer verskaf wat veronderstel is om te onderteken as pad of geheuestroom
        * Instansieer SignOptions-klas en stel alle verlangde data in.
        * Roep die Signature.Sign()-metode deur die uitvoer Odp-lêer of geheuestroom deur te gee

    title_right: " Stelselvereistes"
    content_right: |
        GroupDocs.Signature for .NET word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Kry die nuutste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Odp file
        string filePath = "input.odp";
        // Set up output file
        string outputFilePath = "output.odp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Codabar,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Odp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Teken {{Lêerformaat}} dokumente met Barcode Regstreekse Demo"
    content: |
       Teken nou die Odp-lêer met verskeie handtekeninge deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek. Gratis aanlyn demo wag vir jou.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar is 'n liniêre strepieskode-simbool wat ontwerp is om akkuraat gelees te word, selfs wanneer dit op puntmatriksdrukkers gedruk word vir meervoudige vorms soos FedEx-lugbille en bloedbankvorm.
          characterset: |
             Numeriese syfers (0-9) en spesiale karakters $/-:+.
          textcapacity: |
             Geen spesifieke beperkings nie.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

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