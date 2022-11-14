---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Tiff
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Tiff with Java

############################# Head ############################
head_title: "Søk etter Qrcode-signaturer i filen {{Filformat}} i Java"
head_description: "Bruk Java for å søke etter Qrcode-signaturer i Tiff-filer ved å bruke noen få linjer med kode."

############################# Header ############################
title: "Søk etter Qrcode-signaturer i filen {{Filformat}}"
description: "Java native API gjør det mulig å søke etter Qrcode-signaturer i allerede signerte Tiff-filer. Utfør avansert e-signatursøk i Tiff-dokumentene dine ved å bruke noen få linjer med kode."
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir Java API for behandling av dokumenter ved hjelp av ulike signaturtyper som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, stempler eller metadata. Brukere kan legge til, slette, oppdatere, bekrefte eller søke i elektroniske signaturer i PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater, med ekstra støtte for å tilpasse signaturegenskaper etter behov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Slik søker du etter Qrcode-signaturer i {{Filformat}}"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gjør det enklere for Java-utviklere å søke etter Qrcode-signaturer i Tiff-filer fra applikasjonene deres ved å implementere noen få enkle trinn.
        
        * Opprett en ny forekomst av Signature-klassen og send kildedokumentbanen som en konstruktørparameter.
        * Instantier SearchOptions-objektet i henhold til dine krav og spesifiser søkealternativer.
        * Ring søkemetoden til Signature-klassenforekomsten og send SearchOptions til den.
        * Behandle søkeresultater i henhold til dine krav.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Last ned den nyeste versjonen av GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Tiff document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Søk etter Qrcode elektroniske signaturer Live Demo"
    content: |
       Søk i dokumentet etter ulike elektroniske signaturer til Tiff-filer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Søk etter andre Qrcode-signaturer med Java"
    content: |
        "Elektroniske signaturer søk i ulike dokumenter. Finn signaturer fra et av de populære filformatene som vist nedenfor."
    format: 
           
       
back_to_top:
    enable: true
---