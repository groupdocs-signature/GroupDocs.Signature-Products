---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Svg
productName: .NET
lang: sv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Svg for C#

############################# Head ############################
head_title: "Skapa elektroniska textsignaturer till filen Svg med C#"
head_description: "Sätt Text eSignature på filen Svg för .NET med några rader kod. Använd GroupDocs Document Signature API för att signera dussintals filformat."

############################# Header ############################
title: "Signera {{Filformat}}-filer med Text-signaturer i C#"
description: "Hur man lägger till Text-signatur med några rader med .NET-kod"
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
    title: "Om GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) är ett populärt API för e-signering av digitala dokument. Signaturer som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata finns tillgängliga. Signaturer kan placeras på PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat. Kunder kan signera sina dokument och uppdatera, söka, verifiera, ta bort eller förhandsgranska e-signaturer som satts på dessa dokument. Dessutom tillhandahålls många funktioner för anpassning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steg för att signera {{Filformat}} med Text i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ger möjlighet att signera Svg-dokument med Text-signaturer snabbt och enkelt.
        
        * Skapa en instans av Signature class som tillhandahåller Svg fil som ska signera som sökväg eller minnesström
        * Instantera SignOptions-klassen och ställ in all efterfrågad data.
        * Anropa metoden Signature.Sign() och skicka utdatafilen Svg eller minnesström

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den senaste GroupDocs.Signature for .NET från [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Svg file
        string filePath = "input.svg";
        // Set up output file
        string outputFilePath = "output.svg";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Svg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signerar {{Filformat}} dokument med Text Live Demo"
    content: |
       Signera filen Svg med olika signaturer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis onlinedemo väntar på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andra stödda Text-signaturer för C#"
    content: |
        "Du kan också signera {{Filformat}} med andra signaturtyper. Se listan nedan."
    format: 
       
       
back_to_top:
    enable: true
---