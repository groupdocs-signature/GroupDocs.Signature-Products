---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Ppt
productName: .NET
lang: lv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Ppt for C#

############################# Head ############################
head_title: "Izveidojiet teksta elektroniskos parakstus failam Ppt, izmantojot C#"
head_description: "Ievietojiet Text eParaksts Ppt failā .NET, izmantojot dažas koda rindiņas. Izmantojiet GroupDocs Document Signature API, lai parakstītu desmitiem failu formātu."

############################# Header ############################
title: "Parakstīt Ppt failus ar Text parakstiem programmā C#"
description: "Kā pievienot Text parakstu ar dažām .NET koda rindām"
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
    title: "Par GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ir populāra API digitālo dokumentu e-parakstīšanai. Ir pieejami paraksti, piemēram, teksti, attēli, digitālie sertifikāti, svītrkodi, QR kodi, zīmogi vai metadati. Parakstus var ievietot PDF failos, MS Word dokumentos, MS Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos. Klienti var parakstīt savus dokumentus un atjaunināt, meklēt, pārbaudīt, dzēst vai priekšskatīt uz šiem dokumentiem uzliktos e-parakstus. Turklāt tiek nodrošinātas daudzas parakstu pielāgošanas iespējas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Darbības, lai parakstītu Ppt ar Text programmā C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) nodrošina iespēju ātri un vienkārši parakstīt Ppt dokumentus ar Text parakstiem.
        
        * Izveidojiet paraksta klases gadījumu, kas nodrošina Ppt failu, kas paredzēts parakstīšanai kā ceļš vai atmiņas straume
        * Izveidojiet SignOptions klasi un iestatiet visus pieprasītos datus.
        * Izsauciet metodi Signature.Sign(), kas nodod izvades Ppt failu vai atmiņas straumi

    title_right: " Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for .NET tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Iegūstiet jaunāko GroupDocs.Signature for .NET no [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ppt file
        string filePath = "input.ppt";
        // Set up output file
        string outputFilePath = "output.ppt";

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

                // sign Ppt document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentu Ppt parakstīšana, izmantojot Text tiešraides demonstrāciju"
    content: |
       Parakstiet Ppt failu ar dažādiem parakstiem tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Jūs gaida bezmaksas tiešsaistes demonstrācija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Citi atbalstītie Text paraksti priekš C#"
    content: |
        "Varat arī parakstīt Ppt ar citiem paraksta veidiem. Lūdzu, skatiet sarakstu zemāk."
    format: 
       
       
back_to_top:
    enable: true
---