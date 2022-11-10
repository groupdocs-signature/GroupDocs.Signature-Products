---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: Java
lang: nl
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for Java

############################# Head ############################
head_title: "Digitale elektronische handtekeningen toevoegen aan Dotx bestand met Java"
head_description: "Zet de digitale handtekening op het Dotx-bestand voor Java met een paar regels code. Gebruik de GroupDocs Document Signature API om tientallen bestandsindelingen te ondertekenen."

############################# Header ############################
title: "eSign Dotx bestanden met Digital handtekeningen in Java"
description: "Hoe een Digital handtekening toe te voegen met een paar regels Java code"
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
    title: "Over GroupDocs.Signature for Java API voor digitale handtekeningen"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is een populaire API om documenten te ondertekenen met de digitale elektronische handtekeningen, met digitale certificaten. Voor de API voor digitale handtekeningen gebruikt de API PFX-certificaatbestanden om documenten te ondertekenen met met een wachtwoord beveiligde privé- en openbare sleutels. De digitale handtekeningen kunnen worden gebruikt om zakelijke documenten te certificeren met een specifieke eSign PDF-pagina, en om volledige Microsoft Office-documenten zoals Words, Excel, Powerpoint-bestanden en Open Office-documenten te certificeren. Klanten kunnen de handtekeningen gemakkelijk manipuleren, zoals bewerken, verwijderen of aanpassen. De API biedt een manier om handtekeningen te zoeken en te verifiëren. Bovendien zijn er veel mogelijkheden voor het aanpassen van handtekeningen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappen om Dotx te ondertekenen met Digital in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) biedt de mogelijkheid om Dotx documenten snel en gemakkelijk te ondertekenen met Digital handtekeningen.
        
        * Maak een instantie van de Signature-klasse die een Dotx-bestand levert dat moet worden ondertekend als pad of geheugenstroom
        * Instantieer SignOptions klasse en stel alle gevraagde gegevens in.
        * Roep de Signature.Sign()-methode op en geef uitvoer Dotx-bestand of geheugenstroom

    title_right: " systeem vereisten"
    content_right: |
        GroupDocs.Signature for Java worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download de nieuwste GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";
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

        // sign Dotx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dotx documenten ondertekenen met Digital Live Demo"
    content: |
       Onderteken het Dotx-bestand met verschillende handtekeningen op dit moment door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan. Gratis online demo voor u klaar.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere ondersteunde Digital handtekeningen voor Java"
    content: |
        "U kunt Dotx ook ondertekenen met andere soorten handtekeningen. Zie de lijst hieronder."
    format: 
       
       
back_to_top:
    enable: true
---