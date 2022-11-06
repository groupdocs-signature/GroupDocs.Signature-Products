---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Webp
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Webp with Java

############################# Head ############################
head_title: "Søg efter Barcode signaturer i filen {{Filformat}} i Java"
head_description: "Brug Java til at søge efter Barcode-signaturer i Webp-filer ved hjælp af et par linjer kode."

############################# Header ############################
title: "Søg efter Barcode-signaturer i filen {{Filformat}}"
description: "Java native API gør det muligt at søge efter Barcode-signaturer i allerede signerede Webp-filer. Udfør avanceret e-signatursøgning i dine {{Filformat}} dokumenter ved hjælp af et par linjer kode."
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
    title: "Om GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) giver Java API til behandling af dokumenter ved hjælp af forskellige signaturtyper såsom tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata. Brugere kan tilføje, slette, opdatere, verificere eller søge i elektroniske signaturer i PDF'er, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater, med yderligere støtte til at tilpasse signaturegenskaber efter behov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Sådan søger du efter Barcode-signaturer i {{Filformat}}"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gør det nemmere for Java-udviklere at søge efter Barcode-signaturer i Webp-filer fra deres applikationer ved at implementere nogle få nemme trin.
        
        * Opret en ny forekomst af Signature-klassen og videregiv kildedokumentstien som en konstruktørparameter.
        * Instantiér SearchOptions-objektet i overensstemmelse med dine krav, og angiv søgeindstillinger.
        * Kald søgemetoden for Signature-klasseforekomsten og send SearchOptions til den.
        * Bearbejd søgeresultater i overensstemmelse med dine krav.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download den seneste version af GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Webp file
        String filePath = "input.webp";

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
                            
        // search for Barcode signatures in Webp document
        List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Søg efter Barcode elektroniske signaturer Live Demo"
    content: |
       Søg i dokumentet efter forskellige elektroniske signaturer til Webp-filer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Søg efter andre Barcode-signaturer ved hjælp af Java"
    content: |
        "Elektroniske signaturer søger i forskellige dokumenter. Find signaturer fra et af de populære filformater som vist nedenfor."
    format: 
           
       
back_to_top:
    enable: true
---