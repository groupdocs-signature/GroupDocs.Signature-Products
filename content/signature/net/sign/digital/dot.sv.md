---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dot
productName: .NET
lang: sv
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dot for C#

############################# Head ############################
head_title: "Lägger till digitala elektroniska signaturer i filen Dot med C#"
head_description: "Lägg digital signatur på filen Dot för .NET med några rader kod. Använd GroupDocs Document Signature API för att signera dussintals filformat."

############################# Header ############################
title: "eSign Dot-filer med Digital-signaturer i C#"
description: "Hur man lägger till Digital-signatur med några rader med .NET-kod"
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
    title: "Om GroupDocs.Signature for .NET API för digitala signaturer"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) är ett populärt API för att esignera dokument med digitala elektroniska signaturer, med digitala certifikat. För digitala signaturer använder API PFX-certifikatfiler för att esignera dokument med lösenordsskyddade privata och publika nycklar. De digitala signaturerna kan användas för att certifiera affärsdokument med eSign PDF-specifik sida, certifiera hela Microsoft Office-dokument som Words, Excel, Powerpoint-filer och Open Office-dokument. Kunder kan enkelt manipulera signaturerna som att redigera dem, ta bort eller justera. API ger ett sätt att söka och verifiera signaturer. Dessutom tillhandahålls många funktioner för anpassning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steg för att signera Dot med Digital i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ger möjlighet att signera Dot-dokument med Digital-signaturer snabbt och enkelt.
        
        * Skapa en instans av Signature class som tillhandahåller Dot fil som ska signera som sökväg eller minnesström
        * Instantera SignOptions-klassen och ställ in all efterfrågad data.
        * Anropa metoden Signature.Sign() och skicka utdatafilen Dot eller minnesström

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den senaste GroupDocs.Signature for .NET från [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dot file
        string filePath = "input.dot";
        // Set up output file
        string outputFilePath = "output.dot";
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

                // sign Dot document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signerar Dot dokument med Digital Live Demo"
    content: |
       Signera filen Dot med olika signaturer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis onlinedemo väntar på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andra stödda Digital-signaturer för C#"
    content: |
        "Du kan också signera Dot med andra signaturtyper. Se listan nedan."
    format: 
       
       
back_to_top:
    enable: true
---