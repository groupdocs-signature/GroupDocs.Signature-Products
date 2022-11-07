---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Jpg
productName: .NET
lang: lv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Jpg for C#

############################# Head ############################
head_title: "Pievienojiet metadatu elektroniskos parakstus Jpg dokumentiem, izmantojot C#"
head_description: "Izmantojiet metadatus kā slēptos elektroniskos parakstus savos Jpg dokumentos, izmantojot dažas C# koda rindiņas. Izmantojiet GroupDocs Document Signature API, lai e-parakstītu savus biznesa dokumentus un failus ar metadatu informāciju."

############################# Header ############################
title: "Metadatu elektroniskie paraksti dokumentam Jpg, izmantojot .NET, ir vienkārši un ērti lietojami!"
description: "eParakstiet savus Jpg dokumentus un līgumus ar slēptiem metadatu ierakstiem. Ģenerējiet metadatus PDF failiem, MS Word dokumentiem, MS Excel darbgrāmatām, MS PowerPoint prezentācijām un dažādiem attēlu formātiem bez problēmām un papildu kodēšanas."
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
    title: "Par GroupDocs.Signature for .NET metadatu parakstu API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ir populāra API digitālo dokumentu e-parakstīšanai. Ir pieejami paraksti, piemēram, teksti, attēli, digitālie sertifikāti, svītrkodi, QR kodi, zīmogi vai metadati. Parakstus var ievietot PDF failos, MS Word dokumentos, MS Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos. Klienti var parakstīt savus dokumentus un atjaunināt, meklēt, pārbaudīt, dzēst vai priekšskatīt uz šiem dokumentiem uzliktos e-parakstus. Turklāt tiek nodrošinātas daudzas parakstu pielāgošanas iespējas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Darbības, lai parakstītu Jpg ar Metadata programmā C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) nodrošina iespēju ātri un vienkārši parakstīt Jpg dokumentus ar Metadata parakstiem.
        
        * Izveidojiet paraksta klases gadījumu, kas nodrošina Jpg failu, kas paredzēts parakstīšanai kā ceļš vai atmiņas straume
        * Izveidojiet SignOptions klasi un iestatiet visus pieprasītos datus.
        * Izsauciet metodi Signature.Sign(), kas nodod izvades Jpg failu vai atmiņas straumi

    title_right: " Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for .NET tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Iegūstiet jaunāko GroupDocs.Signature for .NET no [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Jpg file
        string filePath = "input.jpg";
        // Set up output file
        string outputFilePath = "output.jpg";

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

                // sign Jpg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentu Jpg parakstīšana, izmantojot Metadata tiešraides demonstrāciju"
    content: |
       Parakstiet Jpg failu ar dažādiem parakstiem tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Jūs gaida bezmaksas tiešsaistes demonstrācija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Citi atbalstītie Metadata paraksti priekš C#"
    content: |
        "Varat arī parakstīt Jpg ar citiem paraksta veidiem. Lūdzu, skatiet sarakstu zemāk."
    format: 
       
       
back_to_top:
    enable: true
---