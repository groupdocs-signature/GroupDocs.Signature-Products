---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Potm
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Potm for Java

############################# Head ############################
head_title: "Slett Image-signaturer fra Potm-filer via Java"
head_description: "Sletting av spesifikke Image-signaturer fra signerte Potm-dokumenter kan enkelt utføres med kort Java-kode."

############################# Header ############################
title: "Fjern Image-signaturer som er plassert i Potm-filer"
description: "Slett forskjellige Image-signaturer fra Potm-dokumenter. Fjerning av Image-signaturer krever enkel Java-kode."
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
    title: "Få informasjon om GroupDocs.Signature for Java API-funksjoner"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API gir mange måter å behandle dokumentene dine på ved hjelp av elektroniske signaturer. Digitale signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, frimerker eller metadata er tilgjengelig. Kunder har mulighet til å legge til, slette, oppdatere, verifisere eller søke i digitale signaturer på PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater. Et stort antall nyttige funksjoner og innstillinger er gitt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Slik fjerner du Image-signaturer fra Potm-dokumentet"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir nyttig funksjon for å tømme Potm dokumenter for Image signaturer med noen få linjer med kode.
        
        * For det første, instansierer Signatur-objektets bane til dokumentet som en konstruktørparameter.
        * Deretter oppretter du et passende signaturobjekt og setter opp dets unike identifikator.
        * Deretter påkaller du Slett-metoden som sender signaturobjekt som må slettes.
        * Til slutt resultat av prosessdrift.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Last ned den nyeste versjonen av GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";
        // Set up output file
        String outputFilePath = "output.potm";

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
       Legg til ulike elektroniske signaturer i Potm-filen akkurat nå ved å gå til nettstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Slett Image-signaturene dine med Java"
    content: |
        "Sletting av e-signaturer som ble lagt til ulike dokumentformater. Fjern signaturer raskt uten ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---