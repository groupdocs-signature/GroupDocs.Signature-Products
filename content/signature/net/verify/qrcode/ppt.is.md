---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Ppt
productName: .NET
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Ppt for C#

############################# Head ############################
head_title: "Staðfesting á Qrcode undirskriftum fyrir Ppt skrár í gegnum C#"
head_description: "Notaðu aðeins nokkrar línur af .NET kóða til að staðfesta Ppt skjöl og Qrcode undirskrift þeirra."

############################# Header ############################
title: "Qrcode staðfesting á undirskriftum fyrir Ppt skrár"
description: "API fyrir .NET veitir tækifæri til að staðfesta Qrcode undirskriftir á Ppt skjölum. Staðfesting á rafrænum undirskriftum inni í Ppt skjölunum þínum gæti verið framkvæmd fljótt og auðveldlega."
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
    title: "Uppgötvaðu nýja eiginleika GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API býður upp á fjölbreytt úrval leiða til að vinna úr fjölmörgum skjalasniðum með því að nota rafrænar undirskriftir. Margar tegundir stafrænna undirskrifta eins og texta, myndir, stafræn skilríki, strikamerki, QR-kóða, stimpla eða lýsigögn eru studdar. Viðskiptavinir geta bætt við, fjarlægt, breytt, staðfest eða leitað í stafrænum undirskriftum á PDF skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum. Ótrúlegur fjöldi viðbótareiginleika og stillinga er í boði.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að staðfesta Qrcode undirskriftir í Ppt skjalinu þínu"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inniheldur gagnlega eiginleika eins og staðfestingu á Qrcode undirskriftum sem settar eru á Ppt skjöl. Notaðu þetta tækifæri án þess að innleiða aukakóða.
        
        * Í fyrsta lagi, staðfestu undirskriftarflokk sem veitir slóð fyrir breytu byggingaraðila að skjali sem á að vera staðfest.
        * Í öðru lagi, búðu til nýjan VerifyOptions hlut og settu upp alla nauðsynlega eiginleika.
        * Að lokum skaltu kalla á hlut Staðfestingaraðferð Signature sem framhjá VerifyOptions tilviki.
        * Vinndu síðan úr sannprófunarniðurstöðum.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for .NET eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for .NET frá [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ppt file
        string filePath = "input.ppt";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirskrift með Qrcode undirskriftum Live Demo"
    content: |
       Bættu ýmsum rafrænum undirskriftum við Ppt skrá núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Staðfestu aðrar Qrcode undirskriftir með C#"
    content: |
        "Staðfesting rafrænna undirskrifta sem settar eru í ýmis skjöl. Athugaðu gæði undirskrifta í vinsælu skráarsniðunum eins og sýnt er hér að neðan."
    format: 
       
       
back_to_top:
    enable: true
---