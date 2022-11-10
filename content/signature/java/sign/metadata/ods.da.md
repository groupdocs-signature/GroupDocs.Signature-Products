---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ods
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ods for Java

############################# Head ############################
head_title: "Tilføj metadata elektroniske signaturer til Ods dokumenter via Java"
head_description: "Brug Metadata som skjulte elektroniske signaturer i dine Ods-dokumenter ved at bruge et par linjer med Java-kode. Brug GroupDocs Document Signature API til at e-signere dine forretningsdokumenter og filer med metadataoplysninger."

############################# Header ############################
title: "Metadata elektroniske signaturer for Ods dokument via Java er enkle og nemme at bruge!"
description: "eSignér dine Ods dokumenter og kontrakter med skjulte metadataposter. Generer metadata til PDF'er, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer og forskellige billedformater uden problemer og ekstra kodning."
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
    title: "Om GroupDocs.Signature for Java Metadata Signatures API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er en populær API til e-signering af digitale dokumenter. Signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata er tilgængelige. Signaturer kan placeres på PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Kunder kan underskrive deres dokument og opdatere, søge, verificere, slette eller forhåndsvise e-signaturer, der blev sat på disse dokumenter. Desuden er der en masse muligheder for signaturtilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trin til at signere Ods med Metadata i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) giver mulighed for at signere Ods dokumenter med Metadata signaturer hurtigt og nemt.
        
        * Opret en forekomst af signaturklassen, der leverer Ods-fil, der skal signere som sti eller hukommelsesstrøm
        * Instantiér SignOptions-klassen og indstil alle krævede data.
        * Kald Signature.Sign()-metoden ved at sende output Ods-fil eller hukommelsesstrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den seneste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Ods document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering af Ods dokumenter med Metadata Live Demo"
    content: |
       Signer Ods-filen med forskellige signaturer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis online demo venter på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre understøttede Metadata-signaturer for Java"
    content: |
        "Du kan også signere Ods med andre signaturtyper. Se venligst listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---