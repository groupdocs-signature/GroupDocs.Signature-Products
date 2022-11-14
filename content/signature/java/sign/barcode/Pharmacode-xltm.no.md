---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Xltm
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xltm for Java

############################# Head ############################
head_title: "eSign {{Filformat}}-dokument med Pharmacode strekkode i Java"
head_description: "Opprett Pharmacode strekkodesignatur og legg den på Xltm-dokumentet med Java ved å bruke et par linjer med kode. Bruk GroupDocs Document Signature API for å signere ulike filformater."

############################# Header ############################
title: "Generer Pharmacode strekkodesignatur for {{Filformat}} dokument i Java"
description: "eSignér Xltm-bedriftsdokumentene dine med Pharmacode strekkode. Generer strekkodesignatur raskt og enkelt med noen få linjer med kode for å sette opp signeringsalternativer."
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir mulighet til å signere Xltm-dokumenter med Barcode-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Xltm-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Xltm eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den siste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltm file
        String filePath = "input.xltm";
        // Set up output file
        String outputFilePath = "output.xltm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Pharmacode);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Xltm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av {{Filformat}} dokumenter med Barcode Live Demo"
    content: |
       Signer Xltm-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, også kjent som Pharmaceutical Binary Code, er en strekkodestandard som brukes i den farmasøytiske industrien som et pakkekontrollsystem.
          characterset: |
             Numeriske sifre (0-9).
          textcapacity: |
             Representerer bare et enkelt heltall fra 3 til 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

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