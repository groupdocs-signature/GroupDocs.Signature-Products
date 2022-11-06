---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Rtf
productName: Java
lang: cs
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Rtf for Java

############################# Head ############################
head_title: "Připojte elektronické podpisy metadat k dokumentům Rtf prostřednictvím Java"
head_description: "Použijte metadata jako skryté elektronické podpisy ve svých dokumentech Rtf pomocí několika řádků kódu Java. Použijte GroupDocs Document Signature API k elektronickému podepisování obchodních dokumentů a souborů pomocí metadat."

############################# Header ############################
title: "Elektronické podpisy metadat pro dokument Rtf prostřednictvím Java jsou jednoduché a snadno se používají!"
description: "ePodepište své dokumenty a smlouvy Rtf se skrytými položkami metadat. Vytvářejte metadata pro soubory PDF, dokumenty MS Word, sešity MS Excel, prezentace MS PowerPoint a různé formáty obrázků bez problémů a navíc s kódováním."
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
    title_left: "Kroky k podepsání Rtf pomocí Metadata v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umožňuje rychle a snadno podepisovat dokumenty Rtf pomocí podpisů Metadata.
        
        * Vytvořte instanci třídy Signature poskytující soubor Rtf, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Rtf nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for Java jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Získejte nejnovější GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Rtf file
        String filePath = "input.rtf";
        // Set up output file
        String outputFilePath = "output.rtf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Rtf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Rtf pomocí živé ukázky Metadata"
    content: |
       Podepište soubor Rtf pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Metadata pro Java"
    content: |
        "Můžete také podepsat Rtf pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
       
       
back_to_top:
    enable: true
---