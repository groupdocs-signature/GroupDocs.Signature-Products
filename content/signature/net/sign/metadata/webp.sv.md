---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Webp
productName: .NET
lang: sv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Webp for C#

############################# Head ############################
head_title: "Bifoga metadata elektroniska signaturer till Webp dokument via C#"
head_description: "Använd metadata som dolda elektroniska signaturer i dina Webp-dokument med ett par rader med C#-kod. Använd GroupDocs Document Signature API för att e-signera dina affärsdokument och filer med metadatainformation."

############################# Header ############################
title: "Metadata elektroniska signaturer för Webp dokument via .NET är enkla och lätta att använda!"
description: "esignera dina Webp dokument och kontrakt med dolda metadataposter. Generera metadata för PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer och olika bildformat utan problem och extra kodning."
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
    title: "Om GroupDocs.Signature for .NET API för metadatasignaturer"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) är ett populärt API för e-signering av digitala dokument. Signaturer som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata finns tillgängliga. Signaturer kan placeras på PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat. Kunder kan signera sina dokument och uppdatera, söka, verifiera, ta bort eller förhandsgranska e-signaturer som satts på dessa dokument. Dessutom tillhandahålls många funktioner för anpassning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steg för att signera Webp med Metadata i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ger möjlighet att signera Webp-dokument med Metadata-signaturer snabbt och enkelt.
        
        * Skapa en instans av Signature class som tillhandahåller Webp fil som ska signera som sökväg eller minnesström
        * Instantera SignOptions-klassen och ställ in all efterfrågad data.
        * Anropa metoden Signature.Sign() och skicka utdatafilen Webp eller minnesström

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den senaste GroupDocs.Signature for .NET från [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Webp file
        string filePath = "input.webp";
        // Set up output file
        string outputFilePath = "output.webp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Webp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signerar Webp dokument med Metadata Live Demo"
    content: |
       Signera filen Webp med olika signaturer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis onlinedemo väntar på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andra stödda Metadata-signaturer för C#"
    content: |
        "Du kan också signera Webp med andra signaturtyper. Se listan nedan."
    format: 
       
       
back_to_top:
    enable: true
---