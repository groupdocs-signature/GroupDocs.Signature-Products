---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xlsb
productName: Java
lang: nl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xlsb for Java

############################# Head ############################
head_title: "Voeg elektronische handtekeningen met metagegevens toe aan Xlsb documenten via Java"
head_description: "Gebruik metadata als verborgen elektronische handtekeningen in uw Xlsb-documenten met een paar regels Java-code. Gebruik de GroupDocs Document Signature API om uw zakelijke documenten en bestanden elektronisch te ondertekenen met metadata-informatie."

############################# Header ############################
title: "Metadata elektronische handtekeningen voor Xlsb document via Java zijn eenvoudig en gemakkelijk te gebruiken!"
description: "Onderteken uw Xlsb documenten en contracten met verborgen metadata-items. Genereer probleemloos metadata voor PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties en verschillende afbeeldingsformaten."
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
    title: "Over GroupDocs.Signature for Java API voor handtekeningen met metagegevens"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is een populaire API voor het elektronisch ondertekenen van digitale documenten. Handtekeningen zoals teksten, afbeeldingen, digitale certificaten, barcodes, QR-codes, stempels of metadata zijn beschikbaar. Handtekeningen kunnen worden geplaatst op PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsformaten. Klanten kunnen hun document ondertekenen en de elektronische handtekeningen die op die documenten zijn geplaatst bijwerken, zoeken, verifiëren, verwijderen of een voorbeeld bekijken. Bovendien zijn er veel mogelijkheden voor het aanpassen van handtekeningen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappen om Xlsb te ondertekenen met Metadata in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) biedt de mogelijkheid om Xlsb documenten snel en gemakkelijk te ondertekenen met Metadata handtekeningen.
        
        * Maak een instantie van de Signature-klasse die een Xlsb-bestand levert dat moet worden ondertekend als pad of geheugenstroom
        * Instantieer SignOptions klasse en stel alle gevraagde gegevens in.
        * Roep de Signature.Sign()-methode op en geef uitvoer Xlsb-bestand of geheugenstroom

    title_right: " systeem vereisten"
    content_right: |
        GroupDocs.Signature for Java worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download de nieuwste GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";

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

        // sign Xlsb document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Xlsb documenten ondertekenen met Metadata Live Demo"
    content: |
       Onderteken het Xlsb-bestand met verschillende handtekeningen op dit moment door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan. Gratis online demo voor u klaar.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere ondersteunde Metadata handtekeningen voor Java"
    content: |
        "U kunt Xlsb ook ondertekenen met andere soorten handtekeningen. Zie de lijst hieronder."
    format: 
       
       
back_to_top:
    enable: true
---