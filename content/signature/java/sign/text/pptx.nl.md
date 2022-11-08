---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Pptx
productName: Java
lang: nl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Pptx for Java

############################# Head ############################
head_title: "Maak elektronische teksthandtekeningen naar een Pptx-bestand met Java"
head_description: "Zet Text eSignature op Pptx bestand voor Java met een paar regels code. Gebruik de GroupDocs Document Signature API om tientallen bestandsindelingen te ondertekenen."

############################# Header ############################
title: "Onderteken Pptx bestanden met Text handtekeningen in Java"
description: "Hoe voeg je een Text handtekening toe met een paar regels Java code"
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
    title: "Over GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is een populaire API voor het elektronisch ondertekenen van digitale documenten. Handtekeningen zoals teksten, afbeeldingen, digitale certificaten, barcodes, QR-codes, stempels of metadata zijn beschikbaar. Handtekeningen kunnen worden geplaatst op PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsformaten. Klanten kunnen hun document ondertekenen en de elektronische handtekeningen die op die documenten zijn geplaatst bijwerken, zoeken, verifiëren, verwijderen of een voorbeeld bekijken. Bovendien zijn er veel mogelijkheden voor het aanpassen van handtekeningen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappen om Pptx te ondertekenen met Text in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) biedt de mogelijkheid om Pptx documenten snel en gemakkelijk te ondertekenen met Text handtekeningen.
        
        * Maak een instantie van de Signature-klasse die een Pptx-bestand levert dat moet worden ondertekend als pad of geheugenstroom
        * Instantieer SignOptions klasse en stel alle gevraagde gegevens in.
        * Roep de Signature.Sign()-methode op en geef uitvoer Pptx-bestand of geheugenstroom

    title_right: " systeem vereisten"
    content_right: |
        GroupDocs.Signature for Java worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download de nieuwste GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";
        // Set up output file
        String outputFilePath = "output.pptx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pptx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Pptx documenten ondertekenen met Text Live Demo"
    content: |
       Onderteken het Pptx-bestand met verschillende handtekeningen op dit moment door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan. Gratis online demo voor u klaar.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere ondersteunde Text handtekeningen voor Java"
    content: |
        "U kunt Pptx ook ondertekenen met andere soorten handtekeningen. Zie de lijst hieronder."
    format: 
       
       
back_to_top:
    enable: true
---