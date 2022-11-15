---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Svg
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Svg for Java

############################# Head ############################
head_title: "eSign Svg-dokument med Codabar strekkode i Java"
head_description: "Opprett Codabar strekkodesignatur og legg den på Svg-dokumentet med Java ved å bruke et par linjer med kode. Bruk GroupDocs Document Signature API for å signere ulike filformater."

############################# Header ############################
title: "Generer Codabar strekkodesignatur for Svg dokument i Java"
description: "eSignér Svg-bedriftsdokumentene dine med Codabar strekkode. Generer strekkodesignatur raskt og enkelt med noen få linjer med kode for å sette opp signeringsalternativer."
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
    title: "Om GroupDocs.Signature for Java API for strekkodesignaturer."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er et raskt og enkelt API for å administrere digitale dokumenter e-signering ved hjelp av strekkodetyper som UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 og mange andre. Kunder kan enkelt lage strekkoder som gir nødvendig tekst og legge dem på PDF, Microsoft Office Words-dokumenter, Microsoft Office Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater. Strekkoder plassert i dokumenter kan oppdateres, søkes, bekreftes, slettes eller forhåndsvises enten. Dessuten støttes strekkodertilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trinn for å signere Svg med Barcode i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir mulighet til å signere Svg-dokumenter med Barcode-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Svg-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Svg eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den siste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Svg file
        String filePath = "input.svg";
        // Set up output file
        String outputFilePath = "output.svg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Codabar);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Svg document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av Svg dokumenter med Barcode Live Demo"
    content: |
       Signer Svg-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar er en lineær strekkodesymbologi som ble designet for å leses nøyaktig selv når den skrives ut på matriseskrivere for flerdelte skjemaer som FedEx-luftsedler og blodbankskjema.
          characterset: |
             Numeriske sifre (0-9) og spesialtegn $/-:+.
          textcapacity: |
             Ingen spesifikke restriksjoner.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Barcode-signaturer for Java"
    content: |
        "Du kan også signere Svg med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
        
       
back_to_top:
    enable: true
---