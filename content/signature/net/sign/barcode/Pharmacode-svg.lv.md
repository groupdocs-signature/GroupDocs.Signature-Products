---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Svg
productName: .NET
lang: lv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Svg for C#

############################# Head ############################
head_title: "eSign Svg dokuments ar Pharmacode svītrkodu programmā C#"
head_description: "Izveidojiet Pharmacode svītrkoda parakstu un ievietojiet to Svg dokumentā ar .NET, izmantojot pāris koda rindiņas. Izmantojiet GroupDocs Document Signature API dažādu failu formātu parakstīšanai."

############################# Header ############################
title: "Ģenerēt Pharmacode svītrkoda parakstu dokumentam Svg programmā C#"
description: "eParakstiet savus Svg biznesa dokumentus, izmantojot Pharmacode svītrkodu. Ātri un vienkārši ģenerējiet svītrkoda parakstu, izmantojot dažas koda rindiņas, lai iestatītu parakstīšanas opcijas."
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
    title: "Par GroupDocs.Signature for .NET svītrkoda parakstu API."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ir ātra un vienkārša API, lai pārvaldītu digitālo dokumentu e-parakstīšanu, izmantojot svītrkodu veidus, piemēram, UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN. , ITF14 un daudzi citi. Klienti var viegli izveidot svītrkodus ar nepieciešamo tekstu un ievietot tos PDF, Microsoft Office Words dokumentos, Microsoft Office Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos. Dokumentos ievietotos svītrkodus var atjaunināt, meklēt, pārbaudīt, dzēst vai priekšskatīt. Turklāt tiek atbalstīta svītrkodu pielāgošana.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Darbības, lai parakstītu Svg ar Barcode programmā C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) nodrošina iespēju ātri un vienkārši parakstīt Svg dokumentus ar Barcode parakstiem.
        
        * Izveidojiet paraksta klases gadījumu, kas nodrošina Svg failu, kas paredzēts parakstīšanai kā ceļš vai atmiņas straume
        * Izveidojiet SignOptions klasi un iestatiet visus pieprasītos datus.
        * Izsauciet metodi Signature.Sign(), kas nodod izvades Svg failu vai atmiņas straumi

    title_right: " Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for .NET tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Iegūstiet jaunāko GroupDocs.Signature for .NET no [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Svg file
        string filePath = "input.svg";
        // Set up output file
        string outputFilePath = "output.svg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Svg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentu Svg parakstīšana, izmantojot Barcode tiešraides demonstrāciju"
    content: |
       Parakstiet Svg failu ar dažādiem parakstiem tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Jūs gaida bezmaksas tiešsaistes demonstrācija.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Farmaceitiskais kods, kas pazīstams arī kā Pharmaceutical Binary Code, ir svītrkoda standarts, ko izmanto farmācijas rūpniecībā kā iepakojuma kontroles sistēmu.
          characterset: |
             Ciparu cipari (0-9).
          textcapacity: |
             Apzīmē tikai vienu veselu skaitli no 3 līdz 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Citi atbalstītie Barcode paraksti priekš C#"
    content: |
        "Varat arī parakstīt Svg ar citiem paraksta veidiem. Lūdzu, skatiet sarakstu zemāk."
    format: 
        
       
back_to_top:
    enable: true
---