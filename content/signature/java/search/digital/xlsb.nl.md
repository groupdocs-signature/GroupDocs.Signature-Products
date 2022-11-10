---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Xlsb
productName: Java
lang: nl
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Xlsb with Java

############################# Head ############################
head_title: "Zoek naar Digital handtekeningen in Xlsb bestand in Java"
head_description: "Gebruik Java om te zoeken naar Digital handtekeningen in Xlsb bestanden met een paar regels code."

############################# Header ############################
title: "Zoek naar Digital handtekeningen in Xlsb bestand"
description: "Java native API maakt het mogelijk om te zoeken naar Digital handtekeningen in reeds ondertekende Xlsb bestanden. Voer geavanceerd zoeken naar elektronische handtekeningen uit in uw Xlsb-documenten met een paar regels code."
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
    title_left: "Zoeken naar handtekeningen van Digital in Xlsb"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) maakt het voor Java-ontwikkelaars gemakkelijker om te zoeken naar Digital-handtekeningen in Xlsb-bestanden vanuit hun applicaties door een paar eenvoudige stappen te implementeren.
        
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
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Xlsb document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Zoeken naar Digital elektronische handtekeningen Live demo"
    content: |
       Zoek nu in het document naar verschillende elektronische handtekeningen voor Xlsb-bestanden door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Zoek naar andere Digital handtekeningen met Java"
    content: |
        "Elektronische handtekeningen zoeken in verschillende documenten. Vind handtekeningen van een van de populaire bestandsindelingen, zoals hieronder weergegeven."
    format: 
           
       
back_to_top:
    enable: true
---