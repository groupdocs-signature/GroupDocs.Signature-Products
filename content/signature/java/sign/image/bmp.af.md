---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Bmp
productName: Java
lang: af
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Bmp for Java

############################# Head ############################
head_title: "Voeg Image handtekeninge by Bmp lêer met Java"
head_description: "Plaas Image Handtekening op Bmp lêer vir Java deur 'n paar reëls kode te gebruik. Gebruik die GroupDocs Document Signature API om dosyne lêerformate te onderteken."

############################# Header ############################
title: "Teken Bmp lêers met Image handtekeninge in Java"
description: "Hoe om Image handtekening by te voeg met 'n paar reëls van Java kode"
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
    title: "Oor GroupDocs.Signature for Java Beeldhandtekeninge-API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is 'n gewilde API vir die e-ondertekening van digitale dokumente. Handtekeninge soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata is beskikbaar. Handtekeninge kan op PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate geplaas word. Kliënte kan hul dokument onderteken en e-handtekeninge wat op daardie dokumente geplaas is, bywerk, deursoek, verifieer, uitvee of voorbeskou. Boonop word baie vermoëns vir handtekeningaanpassing verskaf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappe om Bmp met Image in Java te onderteken"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bied die vermoë om Bmp dokumente met Image handtekeninge vinnig en maklik te onderteken.
        
        * Skep 'n instansie van Signature-klas wat Bmp-lêer verskaf wat veronderstel is om te onderteken as pad of geheuestroom
        * Instansieer SignOptions-klas en stel alle verlangde data in.
        * Roep die Signature.Sign()-metode deur die uitvoer Bmp-lêer of geheuestroom deur te gee

    title_right: " Stelselvereistes"
    content_right: |
        GroupDocs.Signature for Java word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Kry die nuutste GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Bmp file
        String filePath = "input.bmp";
        // Set up output file
        String outputFilePath = "output.bmp";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Bmp document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Teken Bmp dokumente met Image Regstreekse Demo"
    content: |
       Teken nou die Bmp-lêer met verskeie handtekeninge deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek. Gratis aanlyn demo wag vir jou.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ander ondersteunde Image handtekeninge vir Java"
    content: |
        "Jy kan ook Bmp met ander handtekeningtipes onderteken. Sien asseblief die lys hieronder."
    format: 
       
       
back_to_top:
    enable: true
---