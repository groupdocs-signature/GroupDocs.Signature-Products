---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Docm
productName: Java
lang: cs
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docm for Java

############################# Head ############################
head_title: "Ověření podpisů Digital pro soubory Docm prostřednictvím Java"
head_description: "Použijte pouze několik řádků kódu Java k ověření dokumentů Docm a jejich podpisů Digital."

############################# Header ############################
title: "Ověření podpisů Digital pro soubory Docm"
description: "API pro Java poskytuje příležitost ověřit podpisy Digital v dokumentech Docm. Ověření elektronických podpisů ve vašich dokumentech Docm může být provedeno rychle a snadno."
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
    title: "Objevte nové funkce API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API poskytuje širokou škálu způsobů zpracování mnoha formátů dokumentů pomocí elektronických podpisů. Je podporováno mnoho typů digitálních podpisů, jako jsou texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Zákazníci mohou přidávat, odstraňovat, upravovat, ověřovat nebo prohledávat digitální podpisy v souborech PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých formátech obrázků. K dispozici je úžasný počet dalších funkcí a nastavení.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak ověřit podpisy Digital ve vašem dokumentu Docm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) obsahuje užitečné funkce, jako je ověřování podpisů Digital umístěných v dokumentech Docm. Využijte tuto příležitost bez implementace dalšího kódu.
        
        * Nejprve vytvořte instanci třídy Signature poskytující jako parametr konstruktoru cestu k dokumentu, který má být ověřen.
        * Za druhé, vytvořte nový objekt VerifyOptions a nastavte všechny požadované vlastnosti.
        * Nakonec vyvolejte metodu Verify objektu Signature předávající instanci VerifyOptions.
        * Poté zpracujte výsledky ověření.

    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Signature for Java jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte ve svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Stáhněte si nejnovější verzi GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování pomocí Digital podpisů Živá ukázka"
    content: |
       Přidejte různé elektronické podpisy do souboru Docm právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ověřte další podpisy Digital pomocí Java"
    content: |
        "Ověřování elektronických podpisů umístěných v různých dokumentech. Zkontrolujte kvalitu podpisů v oblíbených formátech souborů, jak je uvedeno níže."
    format: 
       
       
back_to_top:
    enable: true
---