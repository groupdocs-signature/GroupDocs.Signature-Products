---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pdf
productName: Java
lang: cs
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pdf for Java

############################# Head ############################
head_title: "Přidání digitálních elektronických podpisů do souboru Pdf pomocí Java"
head_description: "Vložte digitální podpis do souboru Pdf pro Java pomocí několika řádků kódu. Pomocí rozhraní GroupDocs Document Signature API podepisujte desítky formátů souborů."

############################# Header ############################
title: "Soubory eSign Pdf s podpisy Digital v Java"
description: "Jak přidat podpis Digital pomocí několika řádků kódu Java"
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
    title: "O GroupDocs.Signature for Java rozhraní API pro digitální podpisy"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je populární API pro podepisování dokumentů pomocí digitálních elektronických podpisů a digitálních certifikátů. Pro rozhraní API pro digitální podpisy používá soubory certifikátů PFX k podpisu dokumentu pomocí soukromých a veřejných klíčů chráněných heslem. Digitální podpisy lze použít k certifikaci obchodních dokumentů s konkrétní stránkou eSign PDF, k certifikaci celých dokumentů Microsoft Office, jako jsou Words, Excel, soubory Powerpoint a dokumenty Open Office. Zákazníci mohou s podpisy snadno manipulovat, například je upravovat, odstraňovat nebo upravovat. API poskytuje způsob, jak vyhledávat a ověřovat podpisy. Navíc je k dispozici mnoho schopností pro přizpůsobení podpisů.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky k podepsání Pdf pomocí Digital v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umožňuje rychle a snadno podepisovat dokumenty Pdf pomocí podpisů Digital.
        
        * Vytvořte instanci třídy Signature poskytující soubor Pdf, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Pdf nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for Java jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Získejte nejnovější GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pdf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Pdf pomocí živé ukázky Digital"
    content: |
       Podepište soubor Pdf pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Digital pro Java"
    content: |
        "Můžete také podepsat Pdf pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
       
       
back_to_top:
    enable: true
---