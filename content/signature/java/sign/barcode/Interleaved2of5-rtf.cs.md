---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Rtf
productName: Java
lang: cs
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Rtf for Java

############################# Head ############################
head_title: "Dokument eSign Rtf s čárovým kódem Interleaved2of5 v Java"
head_description: "Vytvořte podpis čárového kódu Interleaved2of5 a vložte jej do dokumentu Rtf s Java pomocí několika řádků kódu. K podepisování různých formátů souborů použijte rozhraní GroupDocs Document Signature API."

############################# Header ############################
title: "Vygenerujte podpis čárového kódu Interleaved2of5 pro dokument Rtf v Java"
description: "ePodepište své obchodní dokumenty ve formátu Rtf pomocí čárového kódu Interleaved2of5. Vygenerujte podpis čárového kódu rychle a snadno pomocí několika řádků kódu pro nastavení možností podepisování."
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
    title: "O rozhraní API pro podpisy čárových kódů GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je rychlé a snadné rozhraní API pro správu elektronického podepisování digitálních dokumentů pomocí typů čárových kódů, jako jsou UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 a mnoho dalších. Zákazníci mohou snadno vytvářet čárové kódy poskytující požadovaný text a vkládat je do PDF, dokumentů Microsoft Office Words, sešitů Microsoft Office Excel, prezentací MS PowerPoint, souborů Adobe Photoshop a různých obrazových formátů. Čárové kódy umístěné v dokumentech lze aktualizovat, vyhledávat, ověřovat, mazat nebo zobrazovat náhled. Navíc je podporováno přizpůsobení čárových kódů.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky k podepsání Rtf pomocí Barcode v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umožňuje rychle a snadno podepisovat dokumenty Rtf pomocí podpisů Barcode.
        
        * Vytvořte instanci třídy Signature poskytující soubor Rtf, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Rtf nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for Java jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Získejte nejnovější GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Rtf file
        String filePath = "input.rtf";
        // Set up output file
        String outputFilePath = "output.rtf";

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

        // sign Rtf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Rtf pomocí živé ukázky Barcode"
    content: |
       Podepište soubor Rtf pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) je souvislá číslice kódující symboliku čárového kódu o dvou šířkách. Komerčně se používá na fólii 135, pro čárové kódy ITF-14 a na kartonech některých produktů, přičemž produkty uvnitř jsou označeny UPC nebo EAN.
          characterset: |
             Číslice (0-9).
          textcapacity: |
             Variabilní délka.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Barcode pro Java"
    content: |
        "Můžete také podepsat Rtf pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
        
       
back_to_top:
    enable: true
---