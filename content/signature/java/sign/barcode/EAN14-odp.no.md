---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N14
fileformat: Odp
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Odp for Java

############################# Head ############################
head_title: "eSign {{Filformat}}-dokument med E A N14 strekkode i Java"
head_description: "Opprett E A N14 strekkodesignatur og legg den på Odp-dokumentet med Java ved å bruke et par linjer med kode. Bruk GroupDocs Document Signature API for å signere ulike filformater."

############################# Header ############################
title: "Generer E A N14 strekkodesignatur for {{Filformat}} dokument i Java"
description: "eSignér Odp-bedriftsdokumentene dine med E A N14 strekkode. Generer strekkodesignatur raskt og enkelt med noen få linjer med kode for å sette opp signeringsalternativer."
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir mulighet til å signere Odp-dokumenter med Barcode-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Odp-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Odp eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den siste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odp file
        String filePath = "input.odp";
        // Set up output file
        String outputFilePath = "output.odp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.E A N14);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Odp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av {{Filformat}} dokumenter med Barcode Live Demo"
    content: |
       Signer Odp-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N14 Barcode"
          content: |
            Europeisk artikkelnummer eller EAN er en standard som beskriver en strekkodesymbologi og nummereringssystem som brukes i global handel for å identifisere en spesifikk detaljhandelsprodukttype, i en spesifikk emballasjekonfigurasjon, fra en spesifikk produsent.
          characterset: |
             Numeriske sifre (0-9) og spesialtegn.
          textcapacity: |
             Nøyaktig 14 numeriske sifre.
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