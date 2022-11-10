---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Ots
productName: Java
lang: sk
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ots for Java

############################# Head ############################
head_title: "Overenie Digital podpisov pre súbory Ots cez Java"
head_description: "Na overenie dokumentov Ots a ich podpisov Digital použite iba niekoľko riadkov kódu Java."

############################# Header ############################
title: "Overenie podpisov Digital pre súbory Ots"
description: "API pre Java poskytuje možnosť overiť podpisy Digital v dokumentoch Ots. Overenie elektronických podpisov vo vašich dokumentoch Ots môže byť vykonané rýchlo a jednoducho."
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
    title: "Objavte nové funkcie rozhrania API služby GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API poskytuje širokú škálu spôsobov spracovania mnohých formátov dokumentov pomocou elektronických podpisov. Podporované sú mnohé typy digitálnych podpisov, ako sú texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Zákazníci môžu pridávať, odstraňovať, upravovať, overovať alebo vyhľadávať digitálne podpisy v súboroch PDF, dokumentoch MS Word, zošitoch MS Excel, prezentáciách MS PowerPoint, súboroch Adobe Photoshop a rôznych obrazových formátoch. K dispozícii je úžasný počet ďalších funkcií a nastavení.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ako overiť podpisy Digital vo vašom dokumente Ots"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) obsahuje užitočné funkcie, ako je overenie podpisov Digital umiestnených v dokumentoch Ots. Využite túto príležitosť bez implementácie dodatočného kódu.
        
        * Najprv vytvorte inštanciu triedy Signature poskytujúcej ako cestu parametra konštruktora k dokumentu, ktorý sa má overiť.
        * Po druhé, vytvorte nový objekt VerifyOptions a nastavte všetky požadované vlastnosti.
        * Nakoniec vyvolajte metódu Verify objektu Signature odovzdávajúcu inštanciu VerifyOptions.
        * Potom spracujte výsledky overenia.

    title_right: "Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for Java sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Stiahnite si najnovšiu verziu GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ots file
        String filePath = "input.ots";

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
    title: "Podpisovanie pomocou Digital podpisov Živá ukážka"
    content: |
       Pridajte rôzne elektronické podpisy do súboru Ots hneď teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Overte ďalšie podpisy Digital pomocou Java"
    content: |
        "Overovanie elektronických podpisov umiestnených v rôznych dokumentoch. Skontrolujte kvalitu podpisov v populárnych formátoch súborov, ako je uvedené nižšie."
    format: 
       
       
back_to_top:
    enable: true
---