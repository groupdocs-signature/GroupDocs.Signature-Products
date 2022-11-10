---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Otp
productName: Java
lang: fi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Otp for Java

############################# Head ############################
head_title: "Liitä metatietojen sähköiset allekirjoitukset Otp-asiakirjoihin Java:n kautta"
head_description: "Käytä metatietoja piilotettuina sähköisinä allekirjoituksina Otp-asiakirjoissasi käyttämällä pari riviä Java-koodia. Käytä GroupDocs Document Signature API:ta yrityksesi dokumenttien ja tiedostojen sähköiseen allekirjoittamiseen metatietotiedoilla."

############################# Header ############################
title: "Metatietojen sähköiset allekirjoitukset asiakirjalle Otp tuotteen Java kautta ovat yksinkertaisia ​​ja helppokäyttöisiä!"
description: "eAllekirjoita Otp asiakirjasi ja sopimuksi piilotetuilla metatietomerkinnöillä. Luo metatietoja PDF-tiedostoille, MS Word -asiakirjoille, MS Excel -työkirjoille, MS PowerPoint -esityksille ja erilaisille kuvamuodoille ilman ongelmia ja ylimääräistä koodausta."
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
    title: "Tietoja GroupDocs.Signature for Java Metadata Signatures API:sta"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) on suosittu sovellusliittymä digitaalisten asiakirjojen sähköiseen allekirjoittamiseen. Saatavilla on allekirjoituksia, kuten tekstejä, kuvia, digitaalisia varmenteita, viivakoodeja, QR-koodeja, leimoja tai metatietoja. Allekirjoituksia voidaan sijoittaa PDF-tiedostoihin, MS Word -asiakirjoihin, MS Excel -työkirjoihin, MS PowerPoint -esityksiin, Adobe Photoshop -tiedostoihin ja erilaisiin kuvamuotoihin. Asiakkaat voivat allekirjoittaa asiakirjansa ja päivittää, etsiä, tarkistaa, poistaa tai esikatsella asiakirjoihin lisättyjä sähköisiä allekirjoituksia. Lisäksi tarjolla on paljon mahdollisuuksia allekirjoitusten mukauttamiseen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Otp:n allekirjoittamiseen Metadata -sovelluksella Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) tarjoaa mahdollisuuden allekirjoittaa Otp-asiakirjoja Metadata-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Otp-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Otp -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for Java on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Hanki uusin GroupDocs.Signature for Java käyttäjältä [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Otp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Otp asiakirjoja Metadata Live-demolla"
    content: |
       Allekirjoita Otp-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Metadata allekirjoitukset ohjelmalle Java"
    content: |
        "Voit myös allekirjoittaa Otp muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
       
       
back_to_top:
    enable: true
---