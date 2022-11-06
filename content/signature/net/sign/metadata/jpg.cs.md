---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Jpg
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Jpg for C#

############################# Head ############################
head_title: "Připojte elektronické podpisy metadat k dokumentům Jpg prostřednictvím C#"
head_description: "Použijte metadata jako skryté elektronické podpisy ve svých dokumentech Jpg pomocí několika řádků kódu C#. Použijte GroupDocs Document Signature API k elektronickému podepisování obchodních dokumentů a souborů pomocí metadat."

############################# Header ############################
title: "Elektronické podpisy metadat pro dokument Jpg prostřednictvím .NET jsou jednoduché a snadno se používají!"
description: "ePodepište své dokumenty a smlouvy Jpg se skrytými položkami metadat. Vytvářejte metadata pro soubory PDF, dokumenty MS Word, sešity MS Excel, prezentace MS PowerPoint a různé formáty obrázků bez problémů a navíc s kódováním."
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
    title: "O rozhraní API pro podpisy metadat GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je oblíbené rozhraní API pro elektronické podepisování digitálních dokumentů. K dispozici jsou podpisy jako texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Podpisy lze umístit do souborů PDF, dokumentů MS Word, sešitů MS Excel, prezentací MS PowerPoint, souborů Adobe Photoshop a různých obrazových formátů. Zákazníci mohou podepsat svůj dokument a aktualizovat, vyhledávat, ověřovat, mazat nebo zobrazovat elektronické podpisy, které byly na tyto dokumenty vloženy. Navíc je k dispozici mnoho schopností pro přizpůsobení podpisů.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky k podepsání Jpg pomocí Metadata v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) umožňuje rychle a snadno podepisovat dokumenty Jpg pomocí podpisů Metadata.
        
        * Vytvořte instanci třídy Signature poskytující soubor Jpg, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Jpg nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získejte nejnovější GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Jpg file
        string filePath = "input.jpg";
        // Set up output file
        string outputFilePath = "output.jpg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Jpg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Jpg pomocí živé ukázky Metadata"
    content: |
       Podepište soubor Jpg pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Metadata pro C#"
    content: |
        "Můžete také podepsat Jpg pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
       
       
back_to_top:
    enable: true
---