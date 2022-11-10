---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Odt
productName: Java
lang: nl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Odt for Java

############################# Head ############################
head_title: "Verwijder Qrcode handtekeningen uit Odt bestanden via Java"
head_description: "Het verwijderen van specifieke Qrcode handtekeningen uit ondertekende Odt documenten kan gemakkelijk worden uitgevoerd met korte Java code."

############################# Header ############################
title: "Verwijder Qrcode handtekeningen die in Odt bestanden zijn geplaatst"
description: "Verwijder verschillende Qrcode handtekeningen uit Odt documenten. Voor het verwijderen van Qrcode-handtekeningen is een eenvoudige Java-code vereist."
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
    title: "Krijg informatie over GroupDocs.Signature for Java API-functies"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API biedt vele manieren om uw documenten te verwerken met behulp van elektronische handtekeningen. Digitale handtekeningen zoals teksten, afbeeldingen, digitale certificaten, barcodes, QR-codes, stempels of metadata zijn beschikbaar. Klanten hebben de mogelijkheid om digitale handtekeningen toe te voegen, te verwijderen, bij te werken, te verifiëren of te zoeken in PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsformaten. Er is een groot aantal handige functies en instellingen beschikbaar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe Qrcode handtekeningen te verwijderen uit uw Odt document"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) biedt een handige functie voor het wissen van Odt documenten van Qrcode handtekeningen met een paar regels code.
        
        * Instantieer eerst het Signature-object dat het pad naar uw document doorgeeft als een constructorparameter.
        * Maak vervolgens een geschikt handtekeningobject en stel de unieke id in.
        * Roep daarna de Delete-methode aan die het handtekeningobject doorgeeft dat moet worden verwijderd.
        * Tot slot de resultaten van de proceswerking.

    title_right: "systeem vereisten"
    content_right: |
        GroupDocs.Signature for Java worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download de nieuwste versie van GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";
        // Set up output file
        String outputFilePath = "output.odt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

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
    title: "Ondertekenen met Qrcode handtekeningen Live demo"
    content: |
       Voeg nu verschillende elektronische handtekeningen toe aan het Odt-bestand door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verwijder uw Qrcode handtekeningen met Java"
    content: |
        "Verwijdering van elektronische handtekeningen die aan verschillende documentformaten zijn toegevoegd. Snel handtekeningen verwijderen zonder extra code."
    format: 
       
       
back_to_top:
    enable: true
---