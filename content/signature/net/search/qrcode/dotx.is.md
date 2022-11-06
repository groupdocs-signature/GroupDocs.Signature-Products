---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Dotx
productName: .NET
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Dotx with C#

############################# Head ############################
head_title: "Leitaðu að Qrcode undirskriftum í Dotx skrá í C#"
head_description: "Notaðu .NET til að leita að Qrcode undirskriftum í Dotx skrám með því að nota nokkrar línur af kóða."

############################# Header ############################
title: "Leitaðu að Qrcode undirskriftum í Dotx skrá"
description: "Innbyggt forritaskil .NET gerir kleift að leita að Qrcode undirskriftum í þegar undirrituðum Dotx skrám. Framkvæmdu háþróaða leit með rafrænum undirskriftum í Dotx skjölunum þínum með því að nota nokkrar línur af kóða."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Um GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) býður upp á .NET API til að vinna úr skjölum með því að nota ýmsar undirskriftargerðir eins og texta, myndir, stafræn skilríki, strikamerki, QR-kóða, stimpla eða lýsigögn. Notendur geta bætt við, eytt, uppfært, staðfest eða leitað í rafrænum undirskriftum í PDF-skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum, með viðbótarstuðningi við að sérsníða eiginleika undirskrifta eftir þörfum.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að leita að Qrcode undirskriftum í Dotx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) auðveldar forriturum .NET að leita að Qrcode undirskriftum í Dotx skrám úr forritum sínum með því að útfæra nokkur einföld skref.
        
        * Búðu til nýtt tilvik af Signature class og sendu frumskjalsslóð sem byggingarbreytu.
        * Stofnaðu SearchOptions hlutinn í samræmi við kröfur þínar og tilgreindu leitarmöguleika.
        * Hringdu í leitaraðferð fyrir undirskriftarflokkstilvik og sendu SearchOptions til þess.
        * Vinndu leitarniðurstöður í samræmi við kröfur þínar.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for .NET eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for .NET frá [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Dotx document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Leitaðu að Qrcode rafrænum undirskriftum Live Demo"
    content: |
       Leitaðu í skjalinu að ýmsum rafrænum undirskriftum í Dotx skrár núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Leitaðu að öðrum Qrcode undirskriftum með því að nota C#"
    content: |
        "Rafrænar undirskriftir leita í ýmsum skjölum. Finndu undirskriftir frá einu af vinsælustu skráarsniðunum eins og sýnt er hér að neðan."
    format: 
           
       
back_to_top:
    enable: true
---