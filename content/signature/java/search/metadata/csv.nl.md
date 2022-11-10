---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Csv
productName: Java
lang: nl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Csv with Java

############################# Head ############################
head_title: "Zoek naar Metadata handtekeningen in Csv bestand in Java"
head_description: "Gebruik Java om te zoeken naar Metadata handtekeningen in Csv bestanden met een paar regels code."

############################# Header ############################
title: "Zoek naar Metadata handtekeningen in Csv bestand"
description: "Java native API maakt het mogelijk om te zoeken naar Metadata handtekeningen in reeds ondertekende Csv bestanden. Voer geavanceerd zoeken naar elektronische handtekeningen uit in uw Csv-documenten met een paar regels code."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Over GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) biedt Java API voor het verwerken van documenten met behulp van verschillende soorten handtekeningen, zoals teksten, afbeeldingen, digitale certificaten, streepjescodes, QR-codes, stempels of metadata. Gebruikers kunnen elektronische handtekeningen toevoegen, verwijderen, bijwerken, verifiëren of zoeken in PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsindelingen, met extra ondersteuning voor het naar behoefte aanpassen van de eigenschappen van handtekeningen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Zoeken naar handtekeningen van Metadata in Csv"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) maakt het voor Java-ontwikkelaars gemakkelijker om te zoeken naar Metadata-handtekeningen in Csv-bestanden vanuit hun applicaties door een paar eenvoudige stappen te implementeren.
        
        * Maak een nieuw exemplaar van de Signature-klasse en geef het brondocumentpad door als een constructorparameter.
        * Instantieer het SearchOptions-object volgens uw vereisten en specificeer zoekopties.
        * Roep de zoekmethode van de instantie van de Signature-klasse aan en geef er SearchOptions aan.
        * Verwerk zoekresultaten overeenkomstig uw eisen.

    title_right: "systeem vereisten"
    content_right: |
        GroupDocs.Signature for Java worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download de nieuwste versie van GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Csv file
        String filePath = "input.csv";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Csv document
        List<SpreadsheetMetadataSignature> signatures = signature.search(SpreadsheetMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "Zoeken naar Metadata elektronische handtekeningen Live demo"
    content: |
       Zoek nu in het document naar verschillende elektronische handtekeningen voor Csv-bestanden door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Zoek naar andere Metadata handtekeningen met Java"
    content: |
        "Elektronische handtekeningen zoeken in verschillende documenten. Vind handtekeningen van een van de populaire bestandsindelingen, zoals hieronder weergegeven."
    format: 
           
       
back_to_top:
    enable: true
---