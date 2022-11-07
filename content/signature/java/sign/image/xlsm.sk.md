---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Xlsm
productName: Java
lang: sk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Xlsm for Java

############################# Head ############################
head_title: "Pridanie podpisov Image do súboru Xlsm pomocou Java"
head_description: "Vložte podpis Image do súboru Xlsm pre Java pomocou niekoľkých riadkov kódu. Použite rozhranie GroupDocs Document Signature API na podpisovanie desiatok formátov súborov."

############################# Header ############################
title: "Podpíšte súbory Xlsm pomocou podpisov Image v Java"
description: "Ako pridať podpis Image pomocou niekoľkých riadkov kódu Java"
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
    title: "O rozhraní API pre podpisy obrázkov GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je obľúbené rozhranie API na elektronické podpisovanie digitálnych dokumentov. K dispozícii sú podpisy ako texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Podpisy možno umiestniť do súborov PDF, dokumentov MS Word, zošitov MS Excel, prezentácií MS PowerPoint, súborov Adobe Photoshop a rôznych formátov obrázkov. Zákazníci môžu podpísať svoj dokument a aktualizovať, vyhľadávať, overovať, mazať alebo zobrazovať elektronické podpisy, ktoré boli vložené do týchto dokumentov. Okrem toho je k dispozícii veľa možností na prispôsobenie podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky na podpísanie Xlsm pomocou Image v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) poskytuje možnosť rýchlo a jednoducho podpisovať dokumenty Xlsm pomocou podpisov Image.
        
        * Vytvorte inštanciu triedy Signature poskytujúcej súbor Xlsm, ktorý sa má podpisovať ako cesta alebo prúd pamäte
        * Instanciujte triedu SignOptions a nastavte všetky požadované údaje.
        * Vyvolajte metódu Signature.Sign() odovzdajúc výstupný súbor Xlsm alebo prúd pamäte

    title_right: " Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for Java sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Získajte najnovší GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsm file
        String filePath = "input.xlsm";
        // Set up output file
        String outputFilePath = "output.xlsm";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xlsm document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanie dokumentov Xlsm pomocou živej ukážky Image"
    content: |
       Podpíšte súbor Xlsm pomocou rôznych podpisov práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čaká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ďalšie podporované podpisy Image pre Java"
    content: |
        "Xlsm môžete podpísať aj inými typmi podpisov. Pozrite si zoznam nižšie."
    format: 
       
       
back_to_top:
    enable: true
---