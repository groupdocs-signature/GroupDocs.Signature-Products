---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Dotx
productName: Java
lang: cs
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dotx for Java

############################# Head ############################
head_title: "Aktualizujte podpisy Image umístěné v souborech Dotx pomocí Java"
head_description: "Použijte jednoduchý a snadno pochopitelný kód Java pro aktualizaci podpisů Image v podepsaných dokumentech Dotx."

############################# Header ############################
title: "Upravte a aktualizujte podpisy Image umístěné v souborech Dotx"
description: "API pro Java poskytuje funkce pro aktualizaci podpisů Image v dokumentech Dotx. Aktualizujte elektronické podpisy ve svých dokumentech Dotx pomocí několika řádků kódu Java rychle a snadno."
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
    title: "Přečtěte si o funkcích API služby GroupDocs.Signature for Java"
    content: |
        Funkce API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) obsahuje široký výběr prostředků pro zpracování dokumentů ve formátech poptávky pomocí elektronických podpisů. Je podporováno široké spektrum elektronických podpisů, jako jsou texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Zákazníci mohou přidávat, odstraňovat, upravovat, ověřovat nebo prohledávat digitální podpisy v souborech PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých formátech obrázků. K dispozici je řada užitečných funkcí a nastavení.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak změnit podpisy Image ve vašem dokumentu Dotx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) obsahuje užitečné funkce, jako je aktualizace podpisů Image umístěných v dokumentech Dotx. Umožňuje měnit vlastnosti podpisů bez dalšího kódu.
        
        * Začněte tím, že vytvoříte objekt Signature, který bude předán jako cesta parametru konstruktoru k dokumentu, který má být aktualizován.
        * Poté vytvořte instanci příslušného konkrétního objektu podpisu a nastavte jeho identifikátor a vlastnosti, které je třeba změnit.
        * Nakonec zavolejte metodu Signature's Update předáním konkrétního objektu podpisu.
        * Zpracujte aktualizaci výsledků k vašemu upozornění.

    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Signature for Java jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte ve svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Stáhněte si nejnovější verzi GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

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
    title: "Aktualizace podpisů Image na stránkách dokumentu - Živá ukázka"
    content: |
       Upravte různé elektronické podpisy dokumentu Dotx právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aktualizujte různé podpisy Image prostřednictvím Java"
    content: |
        "Úpravy digitálních podpisů, které jsou umístěny v různých formátech dokumentů. Aktualizujte data podpisů bez dalšího kódu."
    format: 
       
       
back_to_top:
    enable: true
---