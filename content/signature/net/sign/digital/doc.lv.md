---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: lv
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "Digitālo elektronisko parakstu pievienošana failam Doc, izmantojot C#"
head_description: "Ievietojiet digitālo parakstu Doc failā .NET, izmantojot dažas koda rindiņas. Izmantojiet GroupDocs Document Signature API, lai parakstītu desmitiem failu formātu."

############################# Header ############################
title: "eSign Doc faili ar Digital parakstiem programmā C#"
description: "Kā pievienot Digital parakstu ar dažām .NET koda rindām"
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
    title: "Par GroupDocs.Signature for .NET digitālo parakstu API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ir populāra API dokumentu parakstīšanai ar digitālajiem elektroniskajiem parakstiem un digitālajiem sertifikātiem. Digitālo parakstu API izmanto PFX sertifikātu failus, lai parakstītu dokumentu ar paroli aizsargātām privātajām un publiskajām atslēgām. Ciparparakstus var izmantot, lai sertificētu biznesa dokumentus ar eSign PDF konkrētu lapu, sertificētu visus Microsoft Office dokumentus, piemēram, Words, Excel, Powerpoint failus un Open Office dokumentus. Klienti var viegli manipulēt ar parakstiem, piemēram, tos rediģēt, noņemt vai pielāgot. API nodrošina veidu, kā meklēt un pārbaudīt parakstus. Turklāt tiek nodrošinātas daudzas parakstu pielāgošanas iespējas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Darbības, lai parakstītu Doc ar Digital programmā C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) nodrošina iespēju ātri un vienkārši parakstīt Doc dokumentus ar Digital parakstiem.
        
        * Izveidojiet paraksta klases gadījumu, kas nodrošina Doc failu, kas paredzēts parakstīšanai kā ceļš vai atmiņas straume
        * Izveidojiet SignOptions klasi un iestatiet visus pieprasītos datus.
        * Izsauciet metodi Signature.Sign(), kas nodod izvades Doc failu vai atmiņas straumi

    title_right: " Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for .NET tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Iegūstiet jaunāko GroupDocs.Signature for .NET no [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";
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

                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentu Doc parakstīšana, izmantojot Digital tiešraides demonstrāciju"
    content: |
       Parakstiet Doc failu ar dažādiem parakstiem tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Jūs gaida bezmaksas tiešsaistes demonstrācija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Citi atbalstītie Digital paraksti priekš C#"
    content: |
        "Varat arī parakstīt Doc ar citiem paraksta veidiem. Lūdzu, skatiet sarakstu zemāk."
    format: 
       
       
back_to_top:
    enable: true
---