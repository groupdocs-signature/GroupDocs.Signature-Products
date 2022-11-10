---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Xlsb
productName: Java
lang: sk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xlsb for Java

############################# Head ############################
head_title: "Aktualizujte podpisy Image umiestnené v súboroch Xlsb pomocou Java"
head_description: "Použite jednoduchý a zrozumiteľný kód Java na aktualizáciu podpisov Image v podpísaných dokumentoch Xlsb."

############################# Header ############################
title: "Upravte a aktualizujte podpisy Image umiestnené v súboroch Xlsb"
description: "API pre Java poskytuje funkcie pre aktualizácie podpisov Image v dokumentoch Xlsb. Rýchlo a jednoducho aktualizujte elektronické podpisy vo svojich dokumentoch Xlsb pomocou niekoľkých riadkov kódu Java."
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
    title: "Prečítajte si o funkciách rozhrania API služby GroupDocs.Signature for Java"
    content: |
        Funkcia API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) obsahuje široký výber prostriedkov na spracovanie požadovaných formátov dokumentov pomocou elektronických podpisov. Podporuje široké spektrum elektronických podpisov, ako sú texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Zákazníci môžu pridávať, odstraňovať, upravovať, overovať alebo vyhľadávať digitálne podpisy v súboroch PDF, dokumentoch MS Word, zošitoch MS Excel, prezentáciách MS PowerPoint, súboroch Adobe Photoshop a rôznych obrazových formátoch. K dispozícii je množstvo užitočných funkcií a nastavení.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ako zmeniť Image podpisy vo vašom dokumente Xlsb"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) obsahuje užitočné funkcie, ako je aktualizácia podpisov Image umiestnených v dokumentoch Xlsb. Umožňuje meniť funkcie podpisov bez dodatočného kódu.
        
        * Začnite vytvorením objektu Signature, ktorý prechádza ako cesta parametra konštruktora k dokumentu, ktorý sa má aktualizovať.
        * Potom vytvorte inštanciu príslušného konkrétneho objektu podpisu a nastavte jeho identifikátor a vlastnosti, ktoré je potrebné zmeniť.
        * Nakoniec zavolajte metódu Signature's Update odovzdaním konkrétneho objektu podpisu.
        * Spracujte aktualizáciu výsledkov na vaše upozornenie.

    title_right: "Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for Java sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Stiahnite si najnovšiu verziu GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Aktualizácia podpisov Image na stránkach dokumentu - Živá ukážka"
    content: |
       Upravte rôzne elektronické podpisy dokumentu Xlsb hneď teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aktualizujte rôzne podpisy Image cez Java"
    content: |
        "Úprava digitálnych podpisov, ktoré sú umiestnené v rôznych formátoch dokumentov. Aktualizujte údaje podpisov bez dodatočného kódu."
    format: 
       
       
back_to_top:
    enable: true
---