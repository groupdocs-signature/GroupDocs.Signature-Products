---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Gif
productName: Java
lang: sk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Gif for Java

############################# Head ############################
head_title: "eSign Gif dokument s Interleaved2of5 čiarovým kódom v Java"
head_description: "Vytvorte podpis čiarového kódu Interleaved2of5 a vložte ho do dokumentu Gif s Java pomocou niekoľkých riadkov kódu. Na podpisovanie rôznych formátov súborov použite rozhranie GroupDocs Document Signature API."

############################# Header ############################
title: "Vygenerujte Interleaved2of5 podpis čiarového kódu pre dokument Gif v Java"
description: "ePodpíšte svoje obchodné dokumenty vo formáte Gif pomocou čiarového kódu Interleaved2of5. Vygenerujte podpis čiarového kódu rýchlo a jednoducho pomocou niekoľkých riadkov kódu na nastavenie možností podpisovania."
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
    title: "O rozhraní API podpisov čiarových kódov GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je rýchle a jednoduché rozhranie API na správu elektronického podpisovania digitálnych dokumentov pomocou typov čiarových kódov, ako sú UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 a mnoho ďalších. Zákazníci môžu jednoducho vytvárať čiarové kódy poskytujúce požadovaný text a vkladať ich do PDF, dokumentov Microsoft Office Words, zošitov Microsoft Office Excel, prezentácií MS PowerPoint, súborov Adobe Photoshop a rôznych obrazových formátov. Čiarové kódy umiestnené v dokumentoch je možné aktualizovať, vyhľadávať, overovať, mazať alebo prezerať. Okrem toho je podporované prispôsobenie čiarových kódov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky na podpísanie Gif pomocou Barcode v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) poskytuje možnosť rýchlo a jednoducho podpisovať dokumenty Gif pomocou podpisov Barcode.
        
        * Vytvorte inštanciu triedy Signature poskytujúcej súbor Gif, ktorý sa má podpisovať ako cesta alebo prúd pamäte
        * Instanciujte triedu SignOptions a nastavte všetky požadované údaje.
        * Vyvolajte metódu Signature.Sign() odovzdajúc výstupný súbor Gif alebo prúd pamäte

    title_right: " Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for Java sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Získajte najnovší GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Gif file
        String filePath = "input.gif";
        // Set up output file
        String outputFilePath = "output.gif";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Gif document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanie dokumentov Gif pomocou živej ukážky Barcode"
    content: |
       Podpíšte súbor Gif pomocou rôznych podpisov práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čaká.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) je súvislý čiarový kód s dvojitou šírkou, ktorý kóduje číslice symboliky. Komerčne sa používa na fólii 135, na čiarové kódy ITF-14 a na kartónoch niektorých produktov, pričom produkty vo vnútri sú označené UPC alebo EAN.
          characterset: |
             Číslice (0-9).
          textcapacity: |
             Variabilná dĺžka.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ďalšie podporované podpisy Barcode pre Java"
    content: |
        "Gif môžete podpísať aj inými typmi podpisov. Pozrite si zoznam nižšie."
    format: 
        
       
back_to_top:
    enable: true
---