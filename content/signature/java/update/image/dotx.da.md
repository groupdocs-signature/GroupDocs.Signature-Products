---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Dotx
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dotx for Java

############################# Head ############################
head_title: "Opdater Image signaturer placeret på Dotx filer med Java"
head_description: "Brug enkel og nem at forstå Java-koden til opdatering af Image-signaturer i signerede Dotx-dokumenter."

############################# Header ############################
title: "Rediger og opdater Image signaturer placeret på Dotx filer"
description: "API for Java giver funktionalitet til Image signaturer, der opdateres i Dotx dokumenter. Opdater e-signaturer i dine Dotx dokumenter med et par linjer med Java kode hurtigt og nemt."
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
    title: "Lær om GroupDocs.Signature for Java API-funktioner"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-funktionalitet indeholder et stort udvalg af metoder til at behandle efterspurgte dokumentformater ved at bruge elektroniske signaturer. Bredt spektrum af e-signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata understøttes. Kunder kan tilføje, fjerne, redigere, validere eller søge i digitale signaturer i PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Adskillige nyttige funktioner og indstillinger er tilgængelige.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Sådan ændrer du Image-signaturer i dit Dotx-dokument"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inkluderer nyttige funktioner som f.eks. opdatering af Image signaturer placeret på Dotx dokumenter. Det gør det muligt at ændre signaturfunktioner uden ekstra kode.
        
        * Til at starte med skal du oprette signaturobjekt, der passerer som en konstruktørparametersti til et dokument, som formodes at blive opdateret.
        * Instantiér derefter et passende bestemt signaturobjekt og opsæt dets identifikator og egenskaber, som skal ændres.
        * Til sidst skal du kalde Signatures opdateringsmetode, der sender et bestemt signaturobjekt.
        * Behandle opdatering af resultater til din meddelelse.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download den seneste version af GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Opdatering af Image-signaturerne på dokumentsiderne - Live Demo"
    content: |
       Rediger forskellige elektroniske signaturer af Dotx-dokumentet lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Opdater forskellige Image-signaturer via Java"
    content: |
        "Redigering af digitale signaturer, som er placeret i forskellige dokumentformater. Opdater signaturdata uden ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---