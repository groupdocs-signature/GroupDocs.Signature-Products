---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Pps
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Pps for Java

############################# Head ############################
head_title: "Opret elektroniske tekstsignaturer til filen Pps med Java"
head_description: "Sæt Text eSignature på filen Pps for Java ved hjælp af et par linjer kode. Brug GroupDocs Document Signature API til at signere snesevis af filformater."

############################# Header ############################
title: "Signer Pps-filer med Text-signaturer i Java"
description: "Sådan tilføjer du Text-signatur med et par linjer med Java-kode"
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
    title: "Om GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er en populær API til e-signering af digitale dokumenter. Signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata er tilgængelige. Signaturer kan placeres på PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Kunder kan underskrive deres dokument og opdatere, søge, verificere, slette eller forhåndsvise e-signaturer, der blev sat på disse dokumenter. Desuden er der en masse muligheder for signaturtilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trin til at signere Pps med Text i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) giver mulighed for at signere Pps dokumenter med Text signaturer hurtigt og nemt.
        
        * Opret en forekomst af signaturklassen, der leverer Pps-fil, der skal signere som sti eller hukommelsesstrøm
        * Instantiér SignOptions-klassen og indstil alle krævede data.
        * Kald Signature.Sign()-metoden ved at sende output Pps-fil eller hukommelsesstrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den seneste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pps file
        String filePath = "input.pps";
        // Set up output file
        String outputFilePath = "output.pps";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pps document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering af Pps dokumenter med Text Live Demo"
    content: |
       Signer Pps-filen med forskellige signaturer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis online demo venter på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre understøttede Text-signaturer for Java"
    content: |
        "Du kan også signere Pps med andre signaturtyper. Se venligst listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---