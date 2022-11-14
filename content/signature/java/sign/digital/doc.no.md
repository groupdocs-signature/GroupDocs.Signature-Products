---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: Java
lang: no
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for Java

############################# Head ############################
head_title: "Legger til digitale elektroniske signaturer i filen Doc med Java"
head_description: "Sett digital signatur på Doc-filen for Java ved å bruke noen få linjer med kode. Bruk GroupDocs Document Signature API til å signere dusinvis av filformater."

############################# Header ############################
title: "eSign Doc-filer med Digital-signaturer i Java"
description: "Slik legger du til Digital-signatur med noen få linjer med Java-kode"
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
    title: "Om GroupDocs.Signature for Java API for digitale signaturer"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er et populært API for å esignere dokumenter med digitale elektroniske signaturer, med digitale sertifikater. For Digitale signaturer bruker API PFX-sertifikatfiler for å esignere dokumenter med passordbeskyttede private og offentlige nøkler. De digitale signaturene kan brukes til å sertifisere forretningsdokumenter med eSign PDF-spesifikk side, sertifisere hele Microsoft Office-dokumenter som Words, Excel, Powerpoint-filer og Open Office-dokumenter. Kunder kan enkelt manipulere signaturene som å redigere dem, fjerne eller justere. API-en gir en måte å søke og bekrefte signaturer på. Dessuten er det gitt mange muligheter for tilpasning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trinn for å signere {{Filformat}} med Digital i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gir mulighet til å signere Doc-dokumenter med Digital-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Doc-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Doc eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den siste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Doc document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av {{Filformat}} dokumenter med Digital Live Demo"
    content: |
       Signer Doc-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Digital-signaturer for Java"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---