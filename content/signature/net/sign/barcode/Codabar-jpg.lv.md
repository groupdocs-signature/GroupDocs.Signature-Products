---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Jpg
productName: .NET
lang: lv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Jpg for C#

############################# Head ############################
head_title: "eSign Jpg dokuments ar Codabar svītrkodu programmā C#"
head_description: "Izveidojiet Codabar svītrkoda parakstu un ievietojiet to Jpg dokumentā ar .NET, izmantojot pāris koda rindiņas. Izmantojiet GroupDocs Document Signature API dažādu failu formātu parakstīšanai."

############################# Header ############################
title: "Ģenerēt Codabar svītrkoda parakstu dokumentam Jpg programmā C#"
description: "eParakstiet savus Jpg biznesa dokumentus, izmantojot Codabar svītrkodu. Ātri un vienkārši ģenerējiet svītrkoda parakstu, izmantojot dažas koda rindiņas, lai iestatītu parakstīšanas opcijas."
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
    title_left: "Darbības, lai parakstītu Jpg ar Barcode programmā C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) nodrošina iespēju ātri un vienkārši parakstīt Jpg dokumentus ar Barcode parakstiem.
        
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
                
                // sign Jpg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentu Jpg parakstīšana, izmantojot Barcode tiešraides demonstrāciju"
    content: |
       Parakstiet Jpg failu ar dažādiem parakstiem tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Jūs gaida bezmaksas tiešsaistes demonstrācija.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar ir lineāra svītrkoda simbolika, kas tika izstrādāta tā, lai to varētu precīzi nolasīt pat tad, ja tā tiek drukāta uz matricas printeriem vairāku daļu veidlapām, piemēram, FedEx aviorēķiniem un asins bankas veidlapām.
          characterset: |
             Ciparu cipari (0-9) un īpašās rakstzīmes $/-:+.
          textcapacity: |
             Nav īpašu ierobežojumu.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Citi atbalstītie Barcode paraksti priekš C#"
    content: |
        "Varat arī parakstīt Jpg ar citiem paraksta veidiem. Lūdzu, skatiet sarakstu zemāk."
    format: 
        
       
back_to_top:
    enable: true
---