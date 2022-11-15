---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Jpg
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Jpg for Java

############################# Head ############################
head_title: "Legg til metadata elektroniske signaturer til Jpg dokumenter via Java"
head_description: "Bruk Metadata som skjulte elektroniske signaturer i Jpg-dokumentene dine ved å bruke et par linjer med Java-kode. Bruk GroupDocs Document Signature API til å e-signere forretningsdokumentene og filene dine med metadatainformasjon."

############################# Header ############################
title: "Metadata elektroniske signaturer for Jpg dokument via Java er enkle og enkle å bruke!"
description: "eSigner Jpg-dokumentene og kontraktene dine med skjulte metadataoppføringer. Generer metadata for PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner og ulike bildeformater uten problemer og ekstra koding."
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
    title: "Om GroupDocs.Signature for Java API for metadatasignaturer"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er et populært API for e-signering av digitale dokumenter. Signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, frimerker eller metadata er tilgjengelig. Signaturer kan plasseres på PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og forskjellige bildeformater. Kunder kan signere dokumentet sitt og oppdatere, søke, bekrefte, slette eller forhåndsvise e-signaturer som ble satt på disse dokumentene. Dessuten er det gitt mange muligheter for tilpasning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trinn for å signere Jpg med Metadata i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir mulighet til å signere Jpg-dokumenter med Metadata-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Jpg-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Jpg eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den siste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Jpg file
        String filePath = "input.jpg";
        // Set up output file
        String outputFilePath = "output.jpg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Jpg document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av Jpg dokumenter med Metadata Live Demo"
    content: |
       Signer Jpg-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Metadata-signaturer for Java"
    content: |
        "Du kan også signere Jpg med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---