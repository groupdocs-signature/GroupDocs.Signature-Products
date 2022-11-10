---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Pps
productName: .NET
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Pps for C#

############################# Head ############################
head_title: "Eyða Qrcode undirskriftum úr Pps skrám í gegnum C#"
head_description: "Auðvelt er að eyða tilteknum Qrcode undirskriftum úr undirrituðum Pps skjölum með stuttum .NET kóða."

############################# Header ############################
title: "Fjarlægðu Qrcode undirskriftir sem eru settar í Pps skrár"
description: "Eyða ýmsum Qrcode undirskriftum úr Pps skjölum. Til að fjarlægja Qrcode undirskrift þarf einfaldan C# kóða."
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
    title: "Fáðu upplýsingar um eiginleika GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API veitir margar leiðir til að vinna úr skjölum þínum með rafrænum undirskriftum. Stafrænar undirskriftir eins og textar, myndir, stafræn skilríki, strikamerki, QR-kóðar, stimplar eða lýsigögn eru tiltækar. Viðskiptavinir hafa möguleika á að bæta við, eyða, uppfæra, sannreyna eða leita í stafrænum undirskriftum á PDF skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum. Mikill fjöldi gagnlegra eiginleika og stillinga er til staðar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að fjarlægja Qrcode undirskriftir úr Pps skjalinu þínu"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) býður upp á gagnlegan eiginleika til að hreinsa Pps skjöl af Qrcode undirskriftum með nokkrum línum af kóða.
        
        * Í fyrsta lagi, staðfestu Signature hlut sem fer í gegnum slóðina í skjalið þitt sem byggingarbreytu.
        * Búðu síðan til viðeigandi undirskriftarhlut og settu upp einstakt auðkenni hans.
        * Eftir það skaltu kalla á Delete method sem sendir undirskriftarhlut sem verður að eyða.
        * Að lokum, niðurstöður vinnsluaðgerða.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for .NET eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for .NET frá [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pps file
        string filePath = "input.pps";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                // set up particular signature id
                QrCodeSignature signatureToDelete = new QrCodeSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirskrift með Qrcode undirskriftum Live Demo"
    content: |
       Bættu ýmsum rafrænum undirskriftum við Pps skrá núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Eyddu Qrcode undirskriftunum þínum með C#"
    content: |
        "Eyðing rafrænna undirskrifta sem bætt var við ýmis skjalasnið. Fjarlægðu undirskriftir fljótt án aukakóða."
    format: 
       
       
back_to_top:
    enable: true
---