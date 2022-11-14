---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Ods
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Ods for Java

############################# Head ############################
head_title: "Legger til Image-signaturer til Ods-filen med Java"
head_description: "Sett Image-signatur på Ods-filen for Java ved å bruke noen få linjer med kode. Bruk GroupDocs Document Signature API til å signere dusinvis av filformater."

############################# Header ############################
title: "Signer {{Filformat}}-filer med Image-signaturer i Java"
description: "Slik legger du til Image-signatur med noen få linjer med Java-kode"
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
    title: "Om GroupDocs.Signature for Java API for bildesignaturer"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er et populært API for e-signering av digitale dokumenter. Signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, frimerker eller metadata er tilgjengelig. Signaturer kan plasseres på PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og forskjellige bildeformater. Kunder kan signere dokumentet sitt og oppdatere, søke, bekrefte, slette eller forhåndsvise e-signaturer som ble satt på disse dokumentene. Dessuten er det gitt mange muligheter for tilpasning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trinn for å signere {{Filformat}} med Image i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir mulighet til å signere Ods-dokumenter med Image-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Ods-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Ods eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den siste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ods document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av {{Filformat}} dokumenter med Image Live Demo"
    content: |
       Signer Ods-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Image-signaturer for Java"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---