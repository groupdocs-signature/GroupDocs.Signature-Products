---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Bmp
productName: Java
lang: sk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Bmp with Java

############################# Head ############################
head_title: "Vyhľadajte podpisy Barcode v súbore Bmp v Java"
head_description: "Použite Java na vyhľadávanie Barcode podpisov v súboroch Bmp pomocou niekoľkých riadkov kódu."

############################# Header ############################
title: "Vyhľadajte podpisy Barcode v súbore Bmp"
description: "Natívne API Java umožňuje vyhľadávať podpisy Barcode v už podpísaných súboroch Bmp. Vykonajte rozšírené vyhľadávanie elektronických podpisov vo svojich dokumentoch Bmp pomocou niekoľkých riadkov kódu."
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) poskytuje Java API na spracovanie dokumentov pomocou rôznych typov podpisov, ako sú texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Používatelia môžu pridávať, mazať, aktualizovať, overovať alebo vyhľadávať elektronické podpisy v súboroch PDF, dokumentoch MS Word, zošitoch MS Excel, prezentáciách MS PowerPoint, súboroch Adobe Photoshop a rôznych obrazových formátoch s ďalšou podporou prispôsobenia vlastností podpisov podľa potreby.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ako vyhľadať podpisy Barcode v Bmp"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) uľahčuje vývojárom Java vyhľadávanie podpisov Barcode v súboroch Bmp z ich aplikácií implementáciou niekoľkých jednoduchých krokov.
        
        * Vytvorte novú inštanciu triedy Signature a odovzdajte cestu zdrojového dokumentu ako parameter konštruktora.
        * Vytvorte inštanciu objektu SearchOptions podľa svojich požiadaviek a zadajte možnosti vyhľadávania.
        * Zavolajte metódu vyhľadávania inštancie triedy Signature a odovzdajte jej SearchOptions.
        * Spracujte výsledky vyhľadávania podľa vašich požiadaviek.

    title_right: "Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for Java sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Stiahnite si najnovšiu verziu GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Bmp file
        String filePath = "input.bmp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        BarcodeSearchOptions options = new BarcodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Barcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Barcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Barcode signatures in Bmp document
        List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Vyhľadajte živé ukážky elektronických podpisov Barcode"
    content: |
       Vyhľadajte v dokumente rôzne elektronické podpisy do súborov Bmp práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Vyhľadajte ďalšie podpisy Barcode pomocou Java"
    content: |
        "Elektronické podpisy vyhľadávajú v rôznych dokumentoch. Nájdite podpisy z jedného z populárnych formátov súborov, ako je uvedené nižšie."
    format: 
           
       
back_to_top:
    enable: true
---