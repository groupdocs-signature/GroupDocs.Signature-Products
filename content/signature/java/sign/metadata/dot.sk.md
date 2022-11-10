---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Dot
productName: Java
lang: sk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Dot for Java

############################# Head ############################
head_title: "Pripojte elektronické podpisy metadát k dokumentom Dot cez Java"
head_description: "Použite metadáta ako skryté elektronické podpisy vo svojich dokumentoch Dot pomocou niekoľkých riadkov kódu Java. Použite rozhranie GroupDocs Document Signature API na elektronické podpisovanie obchodných dokumentov a súborov pomocou informácií o metadátach."

############################# Header ############################
title: "Elektronické podpisy metadát pre dokument Dot prostredníctvom Java sú jednoduché a ľahko sa používajú!"
description: "ePodpíšte svoje dokumenty a zmluvy Dot so skrytými položkami metadát. Vytvárajte metadáta pre súbory PDF, dokumenty MS Word, zošity MS Excel, prezentácie MS PowerPoint a rôzne obrazové formáty bez problémov a navyše s kódovaním."
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
    title: "O rozhraní API pre podpisy metadát GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je obľúbené rozhranie API na elektronické podpisovanie digitálnych dokumentov. K dispozícii sú podpisy ako texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Podpisy možno umiestniť do súborov PDF, dokumentov MS Word, zošitov MS Excel, prezentácií MS PowerPoint, súborov Adobe Photoshop a rôznych formátov obrázkov. Zákazníci môžu podpísať svoj dokument a aktualizovať, vyhľadávať, overovať, mazať alebo zobrazovať elektronické podpisy, ktoré boli vložené do týchto dokumentov. Okrem toho je k dispozícii veľa možností na prispôsobenie podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky na podpísanie Dot pomocou Metadata v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) poskytuje možnosť rýchlo a jednoducho podpisovať dokumenty Dot pomocou podpisov Metadata.
        
        * Vytvorte inštanciu triedy Signature poskytujúcej súbor Dot, ktorý sa má podpisovať ako cesta alebo prúd pamäte
        * Instanciujte triedu SignOptions a nastavte všetky požadované údaje.
        * Vyvolajte metódu Signature.Sign() odovzdajúc výstupný súbor Dot alebo prúd pamäte

    title_right: " Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for Java sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Získajte najnovší GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";
        // Set up output file
        String outputFilePath = "output.dot";

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

        // sign Dot document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanie dokumentov Dot pomocou živej ukážky Metadata"
    content: |
       Podpíšte súbor Dot pomocou rôznych podpisov práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čaká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ďalšie podporované podpisy Metadata pre Java"
    content: |
        "Dot môžete podpísať aj inými typmi podpisov. Pozrite si zoznam nižšie."
    format: 
       
       
back_to_top:
    enable: true
---