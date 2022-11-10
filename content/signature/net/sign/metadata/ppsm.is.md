---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ppsm
productName: .NET
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ppsm for C#

############################# Head ############################
head_title: "Bættu rafrænum undirskriftum lýsigagna við Ppsm skjöl í gegnum C#"
head_description: "Notaðu Lýsigögn sem falin rafræn undirskrift í Ppsm skjölunum þínum með því að nota nokkrar línur af C# kóða. Notaðu GroupDocs Document Signature API til að rafrænt undirrita viðskiptaskjölin þín og skrár með upplýsingum um lýsigögn."

############################# Header ############################
title: "Rafrænar undirskriftir með lýsigögnum fyrir Ppsm skjal í gegnum .NET eru einfaldar og auðveldar í notkun!"
description: "eSignaðu Ppsm skjölin þín og samninga með földum lýsigagnafærslum. Búðu til lýsigögn fyrir PDF skjöl, MS Word skjöl, MS Excel vinnubækur, MS PowerPoint kynningar og ýmis myndsnið án vandræða og aukakóðun."
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
    title: "Um GroupDocs.Signature for .NET Lýsigögn undirskriftarforritaskil"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er vinsælt forritaskil fyrir rafræn undirskrift stafrænna skjala. Undirskriftir eins og textar, myndir, stafræn skilríki, strikamerki, QR-kóðar, stimplar eða lýsigögn eru tiltækar. Undirskriftir gætu verið settar á PDF skjöl, MS Word skjöl, MS Excel vinnubækur, MS PowerPoint kynningar, Adobe Photoshop skrár og ýmis myndsnið. Viðskiptavinir geta skrifað undir skjalið sitt og uppfært, leitað, staðfest, eytt eða forskoðað rafrænar undirskriftir sem settar voru á þau skjöl. Þar að auki er mikið af hæfileikum til að sérsníða undirskriftir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Skref til að undirrita Ppsm með Metadata í C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) veitir möguleika á að undirrita Ppsm skjöl með Metadata undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Ppsm skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Ppsm skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for .NET eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Fáðu nýjasta GroupDocs.Signature for .NET frá [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ppsm file
        string filePath = "input.ppsm";
        // Set up output file
        string outputFilePath = "output.ppsm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Ppsm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Ppsm skjöl með Metadata lifandi kynningu"
    content: |
       Skrifaðu undir Ppsm skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Metadata undirskriftir fyrir C#"
    content: |
        "Þú getur líka skrifað undir Ppsm með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
       
       
back_to_top:
    enable: true
---