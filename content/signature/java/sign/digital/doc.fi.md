---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: Java
lang: fi
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for Java

############################# Head ############################
head_title: "Digitaalisten sähköisten allekirjoitusten lisääminen tiedostoon Doc ohjelmalla Java"
head_description: "Aseta digitaalinen allekirjoitus Doc-tiedostoon Java käyttämällä muutamaa koodiriviä. Käytä GroupDocs Document Signature API allekirjoittaaksesi kymmeniä tiedostomuotoja."

############################# Header ############################
title: "eSign Doc tiedostot Digital allekirjoituksella Java"
description: "Allekirjoituksen Digital lisääminen muutamalla rivillä Java-koodia"
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
    title: "Tietoja digitaalisten allekirjoitusten sovellusliittymästä GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) on suosittu sovellusliittymä asiakirjojen allekirjoittamiseen digitaalisilla sähköisillä allekirjoituksilla ja digitaalisilla varmenteilla. Digitaalisten allekirjoitusten API käyttää PFX-sertifikaattitiedostoja asiakirjan allekirjoittamiseen salasanalla suojatuilla yksityisillä ja julkisilla avaimilla. Digitaalisia allekirjoituksia voidaan käyttää sertifioimaan yritysasiakirjoja tietyllä eSign PDF -sivulla, sertifioimaan kokonaisia ​​Microsoft Office -asiakirjoja, kuten Words-, Excel-, Powerpoint-tiedostoja ja Open Office -asiakirjoja. Asiakkaat voivat helposti muokata allekirjoituksia, kuten muokata niitä, poistaa tai säätää. API tarjoaa tavan etsiä ja vahvistaa allekirjoituksia. Lisäksi tarjolla on paljon mahdollisuuksia allekirjoitusten mukauttamiseen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Doc:n allekirjoittamiseen Digital -sovelluksella Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) tarjoaa mahdollisuuden allekirjoittaa Doc-asiakirjoja Digital-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Doc-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Doc -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for Java on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Hanki uusin GroupDocs.Signature for Java käyttäjältä [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";
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

        // sign Doc document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Doc asiakirjoja Digital Live-demolla"
    content: |
       Allekirjoita Doc-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Digital allekirjoitukset ohjelmalle Java"
    content: |
        "Voit myös allekirjoittaa {{Tiedostomuoto}} muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
       
       
back_to_top:
    enable: true
---