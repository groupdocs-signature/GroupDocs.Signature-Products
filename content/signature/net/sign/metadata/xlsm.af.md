---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xlsm
productName: .NET
lang: af
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xlsm for C#

############################# Head ############################
head_title: "Voeg metadata elektroniese handtekeninge by Xlsm dokumente via C#"
head_description: "Gebruik Metadata as versteekte elektroniese handtekeninge binne jou Xlsm dokumente deur 'n paar reëls van C# kode te gebruik. Gebruik die GroupDocs Document Signature API om jou besigheidsdokumente en -lêers met Metadata-inligting te e-teken."

############################# Header ############################
title: "Metadata elektroniese handtekeninge vir Xlsm dokument via .NET is eenvoudig en maklik om te gebruik!"
description: "eTeken jou Xlsm dokumente en kontrakte met versteekte Metadata-inskrywings. Genereer metadata vir PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings en verskeie beeldformate sonder probleme en ekstra kodering."
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
    title: "Meer oor GroupDocs.Signature for .NET Metadata-handtekeninge-API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is 'n gewilde API vir die e-ondertekening van digitale dokumente. Handtekeninge soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata is beskikbaar. Handtekeninge kan op PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate geplaas word. Kliënte kan hul dokument onderteken en e-handtekeninge wat op daardie dokumente geplaas is, bywerk, deursoek, verifieer, uitvee of voorbeskou. Boonop word baie vermoëns vir handtekeningaanpassing verskaf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappe om Xlsm met Metadata in C# te onderteken"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bied die vermoë om Xlsm dokumente met Metadata handtekeninge vinnig en maklik te onderteken.
        
        * Skep 'n instansie van Signature-klas wat Xlsm-lêer verskaf wat veronderstel is om te onderteken as pad of geheuestroom
        * Instansieer SignOptions-klas en stel alle verlangde data in.
        * Roep die Signature.Sign()-metode deur die uitvoer Xlsm-lêer of geheuestroom deur te gee

    title_right: " Stelselvereistes"
    content_right: |
        GroupDocs.Signature for .NET word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Kry die nuutste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xlsm file
        string filePath = "input.xlsm";
        // Set up output file
        string outputFilePath = "output.xlsm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Xlsm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Teken Xlsm dokumente met Metadata Regstreekse Demo"
    content: |
       Teken nou die Xlsm-lêer met verskeie handtekeninge deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek. Gratis aanlyn demo wag vir jou.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ander ondersteunde Metadata handtekeninge vir C#"
    content: |
        "Jy kan ook Xlsm met ander handtekeningtipes onderteken. Sien asseblief die lys hieronder."
    format: 
       
       
back_to_top:
    enable: true
---