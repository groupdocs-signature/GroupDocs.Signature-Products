---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Odt
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Odt with Java

############################# Head ############################
head_title: "Søg efter Digital signaturer i filen Odt i Java"
head_description: "Brug Java til at søge efter Digital-signaturer i Odt-filer ved hjælp af et par linjer kode."

############################# Header ############################
title: "Søg efter Digital-signaturer i filen Odt"
description: "Java native API gør det muligt at søge efter Digital-signaturer i allerede signerede Odt-filer. Udfør avanceret e-signatursøgning i dine Odt dokumenter ved hjælp af et par linjer kode."
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
    title_left: "Sådan søger du efter Digital-signaturer i Odt"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gør det nemmere for Java-udviklere at søge efter Digital-signaturer i Odt-filer fra deres applikationer ved at implementere nogle få nemme trin.
        
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
                
        // Set up input Odt file
        String filePath = "input.odt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Odt document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Søg efter Digital elektroniske signaturer Live Demo"
    content: |
       Søg i dokumentet efter forskellige elektroniske signaturer til Odt-filer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Søg efter andre Digital-signaturer ved hjælp af Java"
    content: |
        "Elektroniske signaturer søger i forskellige dokumenter. Find signaturer fra et af de populære filformater som vist nedenfor."
    format: 
           
       
back_to_top:
    enable: true
---