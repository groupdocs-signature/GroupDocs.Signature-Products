---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Svg
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Svg with C#

############################# Head ############################
head_title: "Vyhledejte podpisy Barcode v souboru Svg v C#"
head_description: "Použijte .NET k vyhledávání podpisů Barcode v souborech Svg pomocí několika řádků kódu."

############################# Header ############################
title: "Vyhledejte podpisy Barcode v souboru Svg"
description: "Nativní API .NET umožňuje vyhledávat podpisy Barcode v již podepsaných souborech Svg. Proveďte pokročilé vyhledávání elektronických podpisů ve svých dokumentech Svg pomocí několika řádků kódu."
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
    title: "O GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje .NET API pro zpracování dokumentů pomocí různých typů podpisů, jako jsou texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Uživatelé mohou přidávat, mazat, aktualizovat, ověřovat nebo prohledávat elektronické podpisy v souborech PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých obrazových formátech s další podporou pro přizpůsobení vlastností podpisů podle potřeby.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak hledat podpisy Barcode v Svg"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) usnadňuje vývojářům .NET hledání podpisů Barcode v souborech Svg z jejich aplikací implementací několika snadných kroků.
        
        * Vytvořte novou instanci třídy Signature a předejte cestu ke zdrojovému dokumentu jako parametr konstruktoru.
        * Vytvořte instanci objektu SearchOptions podle vašich požadavků a zadejte možnosti vyhledávání.
        * Zavolejte metodu Search instance třídy Signature a předejte jí SearchOptions.
        * Zpracujte výsledky vyhledávání podle svých požadavků.

    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte ve svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Stáhněte si nejnovější verzi GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Svg file
        string filePath = "input.svg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                BarcodeSearchOptions options = new BarcodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Barcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Barcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Barcode signatures in Svg document
                List<BarcodeSignature> signatures = signature.Search<BarcodeSignature>(options);

                // process signatures which were found                
                foreach (BarcodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Vyhledejte živé ukázky elektronických podpisů Barcode"
    content: |
       Navštivte web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) a vyhledejte v dokumentu různé elektronické podpisy do souborů Svg právě teď.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Vyhledejte další podpisy Barcode pomocí C#"
    content: |
        "Vyhledávání elektronických podpisů v různých dokumentech. Najděte podpisy z jednoho z oblíbených formátů souborů, jak je uvedeno níže."
    format: 
           
       
back_to_top:
    enable: true
---