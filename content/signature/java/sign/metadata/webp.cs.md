---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Webp
productName: Java
lang: cs
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Webp for Java

############################# Head ############################
head_title: "Připojte elektronické podpisy metadat k dokumentům Webp prostřednictvím Java"
head_description: "Použijte metadata jako skryté elektronické podpisy ve svých dokumentech Webp pomocí několika řádků kódu Java. Použijte GroupDocs Document Signature API k elektronickému podepisování obchodních dokumentů a souborů pomocí metadat."

############################# Header ############################
title: "Elektronické podpisy metadat pro dokument Webp prostřednictvím Java jsou jednoduché a snadno se používají!"
description: "ePodepište své dokumenty a smlouvy Webp se skrytými položkami metadat. Vytvářejte metadata pro soubory PDF, dokumenty MS Word, sešity MS Excel, prezentace MS PowerPoint a různé formáty obrázků bez problémů a navíc s kódováním."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "O rozhraní API pro podpisy metadat GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je oblíbené rozhraní API pro elektronické podepisování digitálních dokumentů. K dispozici jsou podpisy jako texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Podpisy lze umístit do souborů PDF, dokumentů MS Word, sešitů MS Excel, prezentací MS PowerPoint, souborů Adobe Photoshop a různých obrazových formátů. Zákazníci mohou podepsat svůj dokument a aktualizovat, vyhledávat, ověřovat, mazat nebo zobrazovat elektronické podpisy, které byly na tyto dokumenty vloženy. Navíc je k dispozici mnoho schopností pro přizpůsobení podpisů.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky k podepsání Webp pomocí Metadata v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umožňuje rychle a snadno podepisovat dokumenty Webp pomocí podpisů Metadata.
        
        * Vytvořte instanci třídy Signature poskytující soubor Webp, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Webp nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for Java jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Získejte nejnovější GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Webp file
        String filePath = "input.webp";
        // Set up output file
        String outputFilePath = "output.webp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Webp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Webp pomocí živé ukázky Metadata"
    content: |
       Podepište soubor Webp pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Metadata pro Java"
    content: |
        "Můžete také podepsat Webp pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
       
       
back_to_top:
    enable: true
---