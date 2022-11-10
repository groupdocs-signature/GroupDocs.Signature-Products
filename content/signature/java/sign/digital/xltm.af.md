---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xltm
productName: Java
lang: af
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltm for Java

############################# Head ############################
head_title: "Voeg digitale elektroniese handtekeninge by Xltm-lêer met Java"
head_description: "Plaas digitale handtekening op Xltm-lêer vir Java deur 'n paar reëls kode te gebruik. Gebruik die GroupDocs Document Signature API om dosyne lêerformate te onderteken."

############################# Header ############################
title: "eSign Xltm lêers met Digital handtekeninge in Java"
description: "Hoe om Digital handtekening by te voeg met 'n paar reëls van Java kode"
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
    title: "Meer oor GroupDocs.Signature for Java Digitale handtekening-API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is 'n gewilde API om dokumente te ontwerp met die digitale elektroniese handtekeninge, met digitale sertifikate. Vir die Digitale handtekeninge gebruik API PFX-sertifikaatlêers om dokumente met wagwoordbeskermde private en publieke sleutels te ontwerp. Die digitale handtekeninge kan gebruik word om besigheidsdokumente met eSign PDF-spesifieke bladsy te sertifiseer, hele Microsoft Office-dokumente soos Words, Excel, Powerpoint-lêers en Open Office-dokumente te sertifiseer. Kliënte kan die handtekeninge maklik manipuleer, soos om dit te redigeer, te verwyder of aan te pas. Die API bied 'n manier om handtekeninge te soek en te verifieer. Boonop word baie vermoëns vir handtekeningaanpassing verskaf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappe om Xltm met Digital in Java te onderteken"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bied die vermoë om Xltm dokumente met Digital handtekeninge vinnig en maklik te onderteken.
        
        * Skep 'n instansie van Signature-klas wat Xltm-lêer verskaf wat veronderstel is om te onderteken as pad of geheuestroom
        * Instansieer SignOptions-klas en stel alle verlangde data in.
        * Roep die Signature.Sign()-metode deur die uitvoer Xltm-lêer of geheuestroom deur te gee

    title_right: " Stelselvereistes"
    content_right: |
        GroupDocs.Signature for Java word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Kry die nuutste GroupDocs.Signature for Java van [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltm file
        String filePath = "input.xltm";
        // Set up output file
        String outputFilePath = "output.xltm";
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

        // sign Xltm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Teken Xltm dokumente met Digital Regstreekse Demo"
    content: |
       Teken nou die Xltm-lêer met verskeie handtekeninge deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek. Gratis aanlyn demo wag vir jou.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ander ondersteunde Digital handtekeninge vir Java"
    content: |
        "Jy kan ook Xltm met ander handtekeningtipes onderteken. Sien asseblief die lys hieronder."
    format: 
       
       
back_to_top:
    enable: true
---