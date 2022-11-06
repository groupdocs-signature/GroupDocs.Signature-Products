---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Rtf
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Rtf for C#

############################# Head ############################
head_title: "eSign {{Filformat}} dokument med Codabar stregkode i C#"
head_description: "Opret Codabar stregkodesignatur og læg den på Rtf dokument med .NET ved hjælp af et par linjer kode. Brug GroupDocs Document Signature API til at signere forskellige filformater."

############################# Header ############################
title: "Generer Codabar Stregkodesignatur for {{Filformat}} dokument i C#"
description: "eSignér dine Rtf forretningsdokumenter med Codabar stregkode. Generer stregkodesignatur hurtigt og nemt med et par linjer kode for at opsætte signeringsmuligheder."
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
    title: "Om GroupDocs.Signature for .NET stregkodesignatur-API."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er en hurtig og nem API til at administrere digitale dokumenter e-signering ved hjælp af stregkodetyper som UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 og mange andre. Kunder kan nemt oprette stregkoder, der giver den nødvendige tekst og lægge dem på PDF, Microsoft Office Words-dokumenter, Microsoft Office Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Stregkoder placeret i dokumenter kan enten opdateres, søges, verificeres, slettes eller forhåndsvises. Desuden understøttes stregkodertilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trin til at signere {{Filformat}} med Barcode i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) giver mulighed for at signere Rtf dokumenter med Barcode signaturer hurtigt og nemt.
        
        * Opret en forekomst af signaturklassen, der leverer Rtf-fil, der skal signere som sti eller hukommelsesstrøm
        * Instantiér SignOptions-klassen og indstil alle krævede data.
        * Kald Signature.Sign()-metoden ved at sende output Rtf-fil eller hukommelsesstrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den seneste GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Rtf file
        string filePath = "input.rtf";
        // Set up output file
        string outputFilePath = "output.rtf";

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
                
                // sign Rtf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering af {{Filformat}} dokumenter med Barcode Live Demo"
    content: |
       Signer Rtf-filen med forskellige signaturer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis online demo venter på dig.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar er en lineær stregkodesymbologi, der er designet til at kunne læses nøjagtigt, selv når den udskrives på matrixprintere til flerdelte formularer såsom FedEx luftsedler og blodbankformularer.
          characterset: |
             Numeriske cifre (0-9) og specialtegn $/-:+.
          textcapacity: |
             Ingen specifikke restriktioner.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre understøttede Barcode-signaturer for C#"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Se venligst listen nedenfor."
    format: 
        
       
back_to_top:
    enable: true
---