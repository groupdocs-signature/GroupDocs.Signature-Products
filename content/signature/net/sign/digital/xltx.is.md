---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xltx
productName: .NET
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltx for C#

############################# Head ############################
head_title: "Bætir stafrænum rafrænum undirskriftum við Xltx skrá með C#"
head_description: "Settu stafræna undirskrift á Xltx skrá fyrir .NET með því að nota nokkrar línur af kóða. Notaðu GroupDocs Document Signature API til að undirrita heilmikið af skráarsniðum."

############################# Header ############################
title: "eSign Xltx skrár með Digital undirskriftum í C#"
description: "Hvernig á að bæta við Digital undirskrift með nokkrum línum af .NET kóða"
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
    title: "Um GroupDocs.Signature for .NET API fyrir stafrænar undirskriftir"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er vinsælt API til að útskrifa skjöl með stafrænum rafrænum undirskriftum, með stafrænum skilríkjum. Fyrir stafrænar undirskriftir notar API PFX vottorðsskrár til að útskrifa skjal með lykilorðavörðum einka- og opinberum lyklum. Stafrænu undirskriftirnar gætu verið notaðar til að votta viðskiptaskjöl með eSign PDF tiltekinni síðu, votta heil Microsoft Office skjöl eins og Words, Excel, Powerpoint skrár og Open Office skjöl. Viðskiptavinir geta auðveldlega unnið með undirskriftirnar eins og að breyta þeim, fjarlægja eða stilla. API veitir leið til að leita og staðfesta undirskriftir. Þar að auki er mikið af hæfileikum til að sérsníða undirskriftir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Skref til að undirrita Xltx með Digital í C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) veitir möguleika á að undirrita Xltx skjöl með Digital undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Xltx skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Xltx skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for .NET eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Fáðu nýjasta GroupDocs.Signature for .NET frá [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltx file
        string filePath = "input.xltx";
        // Set up output file
        string outputFilePath = "output.xltx";
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

                // sign Xltx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Xltx skjöl með Digital lifandi kynningu"
    content: |
       Skrifaðu undir Xltx skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Digital undirskriftir fyrir C#"
    content: |
        "Þú getur líka skrifað undir Xltx með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
       
       
back_to_top:
    enable: true
---