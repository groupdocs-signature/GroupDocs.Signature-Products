---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Xltm
productName: .NET
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Xltm with C#

############################# Head ############################
head_title: "Leitaðu að Image undirskriftum í Xltm skrá í C#"
head_description: "Notaðu .NET til að leita að Image undirskriftum í Xltm skrám með því að nota nokkrar línur af kóða."

############################# Header ############################
title: "Leitaðu að Image undirskriftum í Xltm skrá"
description: "Innbyggt forritaskil .NET gerir kleift að leita að Image undirskriftum í þegar undirrituðum Xltm skrám. Framkvæmdu háþróaða leit með rafrænum undirskriftum í Xltm skjölunum þínum með því að nota nokkrar línur af kóða."
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
    title_left: "Hvernig á að leita að Image undirskriftum í Xltm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) auðveldar forriturum .NET að leita að Image undirskriftum í Xltm skrám úr forritum sínum með því að útfæra nokkur einföld skref.
        
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
                
        // Set up input Xltm file
        string filePath = "input.xltm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Xltm document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Leitaðu að Image rafrænum undirskriftum Live Demo"
    content: |
       Leitaðu í skjalinu að ýmsum rafrænum undirskriftum í Xltm skrár núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Leitaðu að öðrum Image undirskriftum með því að nota C#"
    content: |
        "Rafrænar undirskriftir leita í ýmsum skjölum. Finndu undirskriftir frá einu af vinsælustu skráarsniðunum eins og sýnt er hér að neðan."
    format: 
           
       
back_to_top:
    enable: true
---