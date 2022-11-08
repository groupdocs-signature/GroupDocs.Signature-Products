---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Jpg
productName: Java
lang: fi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Jpg for Java

############################# Head ############################
head_title: "Allekirjoitusten Image lisääminen tiedostoon Jpg ohjelmalla Java"
head_description: "Aseta Image Allekirjoitus Jpg-tiedostoon Java käyttämällä muutamaa koodiriviä. Käytä GroupDocs Document Signature API allekirjoittaaksesi kymmeniä tiedostomuotoja."

############################# Header ############################
title: "Allekirjoita Jpg tiedostot Image allekirjoituksilla Java"
description: "Kuinka lisätä Image-allekirjoitus, jossa on muutama rivi Java-koodia"
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
    title: "Tietoja GroupDocs.Signature for Java Image signatures API:sta"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) on suosittu sovellusliittymä digitaalisten asiakirjojen sähköiseen allekirjoittamiseen. Saatavilla on allekirjoituksia, kuten tekstejä, kuvia, digitaalisia varmenteita, viivakoodeja, QR-koodeja, leimoja tai metatietoja. Allekirjoituksia voidaan sijoittaa PDF-tiedostoihin, MS Word -asiakirjoihin, MS Excel -työkirjoihin, MS PowerPoint -esityksiin, Adobe Photoshop -tiedostoihin ja erilaisiin kuvamuotoihin. Asiakkaat voivat allekirjoittaa asiakirjansa ja päivittää, etsiä, tarkistaa, poistaa tai esikatsella asiakirjoihin lisättyjä sähköisiä allekirjoituksia. Lisäksi tarjolla on paljon mahdollisuuksia allekirjoitusten mukauttamiseen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Jpg:n allekirjoittamiseen Image -sovelluksella Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) tarjoaa mahdollisuuden allekirjoittaa Jpg-asiakirjoja Image-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Jpg-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Jpg -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for Java on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Hanki uusin GroupDocs.Signature for Java käyttäjältä [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Jpg file
        String filePath = "input.jpg";
        // Set up output file
        String outputFilePath = "output.jpg";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Jpg document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Jpg asiakirjoja Image Live-demolla"
    content: |
       Allekirjoita Jpg-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Image allekirjoitukset ohjelmalle Java"
    content: |
        "Voit myös allekirjoittaa Jpg muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
       
       
back_to_top:
    enable: true
---