---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Otp
productName: Java
lang: af
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Otp for Java

############################# Head ############################
head_title: "Voeg metadata elektroniese handtekeninge by Otp dokumente via Java"
head_description: "Gebruik Metadata as versteekte elektroniese handtekeninge binne jou Otp dokumente deur 'n paar reëls van Java kode te gebruik. Gebruik die GroupDocs Document Signature API om jou besigheidsdokumente en -lêers met Metadata-inligting te e-teken."

############################# Header ############################
title: "Metadata elektroniese handtekeninge vir Otp dokument via Java is eenvoudig en maklik om te gebruik!"
description: "eTeken jou Otp dokumente en kontrakte met versteekte Metadata-inskrywings. Genereer metadata vir PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings en verskeie beeldformate sonder probleme en ekstra kodering."
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
    title: "Meer oor GroupDocs.Signature for Java Metadata-handtekeninge-API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is 'n gewilde API vir die e-ondertekening van digitale dokumente. Handtekeninge soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata is beskikbaar. Handtekeninge kan op PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate geplaas word. Kliënte kan hul dokument onderteken en e-handtekeninge wat op daardie dokumente geplaas is, bywerk, deursoek, verifieer, uitvee of voorbeskou. Boonop word baie vermoëns vir handtekeningaanpassing verskaf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappe om Otp met Metadata in Java te onderteken"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bied die vermoë om Otp dokumente met Metadata handtekeninge vinnig en maklik te onderteken.
        
        * Skep 'n instansie van Signature-klas wat Otp-lêer verskaf wat veronderstel is om te onderteken as pad of geheuestroom
        * Instansieer SignOptions-klas en stel alle verlangde data in.
        * Roep die Signature.Sign()-metode deur die uitvoer Otp-lêer of geheuestroom deur te gee

    title_right: " Stelselvereistes"
    content_right: |
        GroupDocs.Signature for Java word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Kry die nuutste GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Otp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Teken Otp dokumente met Metadata Regstreekse Demo"
    content: |
       Teken nou die Otp-lêer met verskeie handtekeninge deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek. Gratis aanlyn demo wag vir jou.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ander ondersteunde Metadata handtekeninge vir Java"
    content: |
        "Jy kan ook Otp met ander handtekeningtipes onderteken. Sien asseblief die lys hieronder."
    format: 
       
       
back_to_top:
    enable: true
---