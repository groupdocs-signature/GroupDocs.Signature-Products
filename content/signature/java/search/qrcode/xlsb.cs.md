---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Xlsb
productName: Java
lang: cs
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Xlsb with Java

############################# Head ############################
head_title: "Vyhledejte podpisy Qrcode v souboru Xlsb v Java"
head_description: "Použijte Java k vyhledávání podpisů Qrcode v souborech Xlsb pomocí několika řádků kódu."

############################# Header ############################
title: "Vyhledejte podpisy Qrcode v souboru Xlsb"
description: "Nativní API Java umožňuje vyhledávat podpisy Qrcode v již podepsaných souborech Xlsb. Proveďte pokročilé vyhledávání elektronických podpisů ve svých dokumentech Xlsb pomocí několika řádků kódu."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) poskytuje Java API pro zpracování dokumentů pomocí různých typů podpisů, jako jsou texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Uživatelé mohou přidávat, mazat, aktualizovat, ověřovat nebo prohledávat elektronické podpisy v souborech PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých obrazových formátech s další podporou pro přizpůsobení vlastností podpisů podle potřeby.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak hledat podpisy Qrcode v Xlsb"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) usnadňuje vývojářům Java hledání podpisů Qrcode v souborech Xlsb z jejich aplikací implementací několika snadných kroků.
        
        * Vytvořte novou instanci třídy Signature a předejte cestu ke zdrojovému dokumentu jako parametr konstruktoru.
        * Vytvořte instanci objektu SearchOptions podle vašich požadavků a zadejte možnosti vyhledávání.
        * Zavolejte metodu Search instance třídy Signature a předejte jí SearchOptions.
        * Zpracujte výsledky vyhledávání podle svých požadavků.

    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Signature for Java jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte ve svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Stáhněte si nejnovější verzi GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Xlsb document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Vyhledejte živé ukázky elektronických podpisů Qrcode"
    content: |
       Navštivte web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) a vyhledejte v dokumentu různé elektronické podpisy do souborů Xlsb právě teď.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Vyhledejte další podpisy Qrcode pomocí Java"
    content: |
        "Vyhledávání elektronických podpisů v různých dokumentech. Najděte podpisy z jednoho z oblíbených formátů souborů, jak je uvedeno níže."
    format: 
           
       
back_to_top:
    enable: true
---