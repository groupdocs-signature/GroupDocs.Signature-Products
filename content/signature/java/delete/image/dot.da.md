---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Dot
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dot for Java

############################# Head ############################
head_title: "Slet Image signaturer fra Dot filer via Java"
head_description: "Sletning af specifikke Image-signaturer fra signerede Dot-dokumenter kan udføres nemt med en kort Java-kode."

############################# Header ############################
title: "Fjern Image-signaturer, der er placeret i Dot-filer"
description: "Slet forskellige Image-signaturer fra Dot-dokumenter. Fjernelse af Image signaturer kræver simpel Java kode."
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
    title: "Få oplysninger om GroupDocs.Signature for Java API-funktioner"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API giver mange måder at behandle dine dokumenter ved hjælp af elektroniske signaturer. Digitale signaturer som tekster, billeder, digitale certifikater, stregkoder, QR-koder, stempler eller metadata er tilgængelige. Kunder har mulighed for at tilføje, slette, opdatere, verificere eller søge i digitale signaturer i PDF-filer, MS Word-dokumenter, MS Excel-projektmapper, MS PowerPoint-præsentationer, Adobe Photoshop-filer og forskellige billedformater. Der er et stort antal nyttige funktioner og indstillinger.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Sådan fjerner du Image-signaturer fra dit Dot-dokument"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) giver nyttige funktioner til at rydde Dot dokumenter for Image signaturer med et par linjer kode.
        
        * For det første skal du instansiere Signatur-objektets sti til dit dokument som en konstruktørparameter.
        * Opret derefter et passende signaturobjekt og opsæt dets unikke identifikator.
        * Kald derefter Slet-metoden, der passerer signaturobjekt, som skal slettes.
        * Endelig resultat af procesdrift.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download den seneste version af GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";
        // Set up output file
        String outputFilePath = "output.dot";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

        // provide signature features to delete
        ImageSignature signatureToDelete = new ImageSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering med Image signaturer Live Demo"
    content: |
       Føj forskellige elektroniske signaturer til filen Dot lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Slet dine Image-signaturer med Java"
    content: |
        "Sletning af e-signaturer som blev tilføjet til forskellige dokumentformater. Fjern signaturer hurtigt uden ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---