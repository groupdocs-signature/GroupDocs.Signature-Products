---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Odp
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Odp with Java

############################# Head ############################
head_title: "Søg efter Image signaturer i filen {{Filformat}} i Java"
head_description: "Brug Java til at søge efter Image-signaturer i Odp-filer ved hjælp af et par linjer kode."

############################# Header ############################
title: "Søg efter Image-signaturer i filen {{Filformat}}"
description: "Java native API gør det muligt at søge efter Image-signaturer i allerede signerede Odp-filer. Udfør avanceret e-signatursøgning i dine {{Filformat}} dokumenter ved hjælp af et par linjer kode."
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
    title_left: "Sådan søger du efter Image-signaturer i {{Filformat}}"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gør det nemmere for Java-udviklere at søge efter Image-signaturer i Odp-filer fra deres applikationer ved at implementere nogle få nemme trin.
        
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
                
        // Set up input Odp file
        String filePath = "input.odp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Odp document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Søg efter Image elektroniske signaturer Live Demo"
    content: |
       Søg i dokumentet efter forskellige elektroniske signaturer til Odp-filer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Søg efter andre Image-signaturer ved hjælp af Java"
    content: |
        "Elektroniske signaturer søger i forskellige dokumenter. Find signaturer fra et af de populære filformater som vist nedenfor."
    format: 
           
       
back_to_top:
    enable: true
---