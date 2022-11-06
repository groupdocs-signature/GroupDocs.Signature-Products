---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Dot
productName: .NET
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dot for C#

############################# Head ############################
head_title: "Uppfærðu Image undirskriftir settar á Dot skrár með C#"
head_description: "Notaðu einfaldan og auðskilinn .NET kóða fyrir uppfærslu á Image undirskriftum í undirrituðum Dot skjölum."

############################# Header ############################
title: "Breyttu og uppfærðu Image undirskriftir sem settar eru á Dot skrár"
description: "API fyrir .NET veitir virkni fyrir Image undirskriftir sem uppfæra á Dot skjölum. Uppfærðu rafrænar undirskriftir í Dot skjölunum þínum með nokkrum línum af C# kóða fljótt og auðveldlega."
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
    title: "Lærðu um GroupDocs.Signature for .NET API eiginleika"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API virkni inniheldur mikið úrval af aðferðum til að vinna eftirspurn eftir skjölum með því að nota rafrænar undirskriftir. Fjölbreytt úrval rafrænna undirskrifta eins og texta, myndir, stafræn skilríki, strikamerki, QR-kóða, stimpla eða lýsigögn eru studd. Viðskiptavinir geta bætt við, fjarlægt, breytt, staðfest eða leitað í stafrænum undirskriftum á PDF skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum. Fjölmargir gagnlegir eiginleikar og stillingar eru í boði.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að breyta Image undirskriftum í Dot skjalinu þínu"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inniheldur gagnlega eiginleika eins og uppfærslu á Image undirskriftum sem settar eru á Dot skjöl. Það gerir mögulegt að breyta eiginleikum undirskrifta án aukakóða.
        
        * Til að byrja með, búðu til Signature hlut sem fer sem slóð byggingarbreytu í skjal sem á að uppfæra.
        * Settu síðan upp viðeigandi tiltekinn undirskriftarhlut og settu upp auðkenni hans og eiginleika sem þarf að breyta.
        * Að lokum skaltu kalla uppfærsluaðferð Signature sem sendir tiltekinn undirskriftarhlut.
        * Vinndu við að uppfæra niðurstöður til þín.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for .NET eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for .NET frá [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dot file
        string filePath = "input.dot";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Að uppfæra Image undirskriftirnar á skjalasíðunum - Sýning í beinni"
    content: |
       Breyttu ýmsum rafrænum undirskriftum Dot skjalsins núna með því að fara á vefsíðuna [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Uppfærðu ýmsar Image undirskriftir í gegnum C#"
    content: |
        "Breyta stafrænum undirskriftum sem eru settar á mismunandi skjalasnið. Uppfærðu undirskriftargögn án aukakóða."
    format: 
       
       
back_to_top:
    enable: true
---