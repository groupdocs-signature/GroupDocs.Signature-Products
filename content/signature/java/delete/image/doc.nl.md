---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Doc
productName: Java
lang: nl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Doc for Java

############################# Head ############################
head_title: "Verwijder Image handtekeningen uit Doc bestanden via Java"
head_description: "Het verwijderen van specifieke Image handtekeningen uit ondertekende Doc documenten kan gemakkelijk worden uitgevoerd met korte Java code."

############################# Header ############################
title: "Verwijder Image handtekeningen die in Doc bestanden zijn geplaatst"
description: "Verwijder verschillende Image handtekeningen uit Doc documenten. Voor het verwijderen van Image-handtekeningen is een eenvoudige Java-code vereist."
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
    title_left: "Hoe Image handtekeningen te verwijderen uit uw Doc document"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) biedt een handige functie voor het wissen van Doc documenten van Image handtekeningen met een paar regels code.
        
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
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";

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
    title: "Ondertekenen met Image handtekeningen Live demo"
    content: |
       Voeg nu verschillende elektronische handtekeningen toe aan het Doc-bestand door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verwijder uw Image handtekeningen met Java"
    content: |
        "Verwijdering van elektronische handtekeningen die aan verschillende documentformaten zijn toegevoegd. Snel handtekeningen verwijderen zonder extra code."
    format: 
       
       
back_to_top:
    enable: true
---