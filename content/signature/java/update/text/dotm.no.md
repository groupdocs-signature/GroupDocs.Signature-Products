---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Dotm
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Dotm for Java

############################# Head ############################
head_title: "Oppdater Text-signaturer plassert på Dotm-filer med Java"
head_description: "Bruk enkel og enkel for å forstå Java-koden for Text-signaturoppdatering i signerte {{Filformat}}-dokumenter."

############################# Header ############################
title: "Rediger og oppdater Text-signaturer plassert i {{Filformat}}-filer"
description: "API for Java gir funksjonalitet for Text-signaturer som oppdateres i {{Filformat}}-dokumenter. Oppdater e-signaturer i {{Filformat}}-dokumentene dine med et par linjer med Java-kode raskt og enkelt."
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
    title: "Lær om GroupDocs.Signature for Java API-funksjoner"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-funksjonalitet inneholder et stort utvalg måter å behandle etterspurte dokumentformater ved å bruke elektroniske signaturer. Et bredt spekter av e-signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, stempler eller metadata støttes. Kunder kan legge til, fjerne, redigere, validere eller søke i digitale signaturer i PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater. Mange nyttige funksjoner og innstillinger er tilgjengelige.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvordan endre Text-signaturer i {{Filformat}}-dokumentet ditt"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inkluderer nyttige funksjoner som oppdatering av Text-signaturer plassert i {{Filformat}}-dokumenter. Det gjør det mulig å endre signaturfunksjoner uten ekstra kode.
        
        * Til å begynne med, lag signaturobjekt som passerer som en konstruktørparameterbane til et dokument som skal oppdateres.
        * Deretter instansierer du et passende bestemt signaturobjekt og setter opp identifikatoren og egenskapene som må endres.
        * Til slutt kaller du Signatures oppdateringsmetode som sender et bestemt signaturobjekt.
        * Behandle oppdatering av resultater til din varsel.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Last ned den nyeste versjonen av GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotm file
        String filePath = "input.dotm";
        // Set up output file
        String outputFilePath = "output.dotm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

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
    title: "Oppdatering av Text-signaturene på dokumentsidene - Live Demo"
    content: |
       Rediger ulike elektroniske signaturer til Dotm-dokumentet akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Oppdater forskjellige Text-signaturer via Java"
    content: |
        "Redigering av digitale signaturer som er plassert i ulike dokumentformater. Oppdater signaturdata uten ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---