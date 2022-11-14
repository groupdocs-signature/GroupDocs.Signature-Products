---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: ISBN
fileformat: Gif
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Gif for Java

############################# Head ############################
head_title: "eSign {{Filformat}}-dokument med ISBN strekkode i Java"
head_description: "Opprett ISBN strekkodesignatur og legg den på Gif-dokumentet med Java ved å bruke et par linjer med kode. Bruk GroupDocs Document Signature API for å signere ulike filformater."

############################# Header ############################
title: "Generer ISBN strekkodesignatur for {{Filformat}} dokument i Java"
description: "eSignér Gif-bedriftsdokumentene dine med ISBN strekkode. Generer strekkodesignatur raskt og enkelt med noen få linjer med kode for å sette opp signeringsalternativer."
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
    title_left: "Trinn for å signere {{Filformat}} med Barcode i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir mulighet til å signere Gif-dokumenter med Barcode-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Gif-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Gif eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den siste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
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
        options.setEncodeType(BarcodeTypes.ISBN);

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
    title: "Signering av {{Filformat}} dokumenter med Barcode Live Demo"
    content: |
       Signer Gif-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About ISBN Barcode"
          content: |
            International Standard Book Number (ISBN) er en numerisk kommersiell bokidentifikator som er ment å være unik.[a][b] Utgivere kjøper ISBN-numre fra en tilknyttet organisasjon til International ISBN Agency.
          characterset: |
             Numeriske sifre (0-9).
          textcapacity: |
             Nøyaktig 9 siffer + 1 kontrollsiffer.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Barcode-signaturer for Java"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
        
       
back_to_top:
    enable: true
---