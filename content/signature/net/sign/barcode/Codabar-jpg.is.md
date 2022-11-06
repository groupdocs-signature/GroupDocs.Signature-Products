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
lang: is
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Jpg for C#

############################# Head ############################
head_title: "eSign Jpg skjal með Codabar Strikamerki í C#"
head_description: "Búðu til Codabar Strikamerki undirskrift og settu hana á Jpg skjal með .NET með því að nota nokkrar línur af kóða. Notaðu GroupDocs Document Signature API til að undirrita ýmis skráarsnið."

############################# Header ############################
title: "Búðu til Codabar Strikamerki undirskrift fyrir Jpg skjal í C#"
description: "eSignaðu Jpg viðskiptaskjölin þín með Codabar Strikamerki. Búðu til Strikamerki undirskrift fljótt og auðveldlega með nokkrum línum af kóða til að setja upp undirskriftarmöguleika."
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
    title: "Um GroupDocs.Signature for .NET Strikamerki undirskriftarforritaskil."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er fljótlegt og auðvelt forritaskil til að stjórna rafrænni undirskrift skjala með því að nota Strikamerki eins og UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 og margir aðrir. Viðskiptavinir geta auðveldlega búið til Strikamerki með nauðsynlegum texta og sett þá á PDF, Microsoft Office Words Documents, Microsoft Office Excel vinnubækur, MS PowerPoint kynningar, Adobe Photoshop skrár og ýmis myndsnið. Strikamerki sem sett eru í skjöl er hægt að uppfæra, leita, staðfesta, eyða eða forskoða annað hvort. Þar að auki er aðlögun strikamerkja studd.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Skref til að undirrita Jpg með Barcode í C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) veitir möguleika á að undirrita Jpg skjöl með Barcode undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Jpg skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Jpg skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for .NET eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Fáðu nýjasta GroupDocs.Signature for .NET frá [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
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
    title: "Undirritar Jpg skjöl með Barcode lifandi kynningu"
    content: |
       Skrifaðu undir Jpg skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar er línuleg strikamerki táknfræði sem var hönnuð til að vera nákvæmlega lesin, jafnvel þegar þau eru prentuð á punktafylkisprentara fyrir fjölþætt eyðublöð eins og FedEx flugseðla og blóðbankaform.
          characterset: |
             Tölustafir (0-9) og sérstafir $/-:+.
          textcapacity: |
             Engar sérstakar takmarkanir.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Barcode undirskriftir fyrir C#"
    content: |
        "Þú getur líka skrifað undir Jpg með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
        
       
back_to_top:
    enable: true
---