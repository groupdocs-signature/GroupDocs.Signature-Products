---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Zip
productName: Java
lang: fi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Zip for Java

############################# Head ############################
head_title: "Allekirjoitusten Qrcode vahvistaminen tiedostoille Zip Java:n kautta"
head_description: "Käytä vain muutamaa riviä Java-koodia Zip-asiakirjojen ja niiden allekirjoitusten Qrcode vahvistamiseen."

############################# Header ############################
title: "Qrcode allekirjoitusten vahvistus tiedostoille Zip"
description: "API for Java tarjoaa mahdollisuuden tarkistaa Qrcode allekirjoitukset Zip asiakirjoissa. Zip-asiakirjojen sisällä olevien sähköisten allekirjoitusten varmennus voidaan suorittaa nopeasti ja helposti."
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
    title: "Tutustu uusiin GroupDocs.Signature for Java API -ominaisuuksiin"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API tarjoaa laajan valikoiman tapoja käsitellä useita dokumenttimuotoja käyttämällä sähköisiä allekirjoituksia. Monen tyyppisiä digitaalisia allekirjoituksia, kuten tekstejä, kuvia, digitaalisia varmenteita, viivakoodeja, QR-koodeja, leimoja tai metatietoja, tuetaan. Asiakkaat voivat lisätä, poistaa, muokata, vahvistaa tai etsiä digitaalisia allekirjoituksia PDF-tiedostoista, MS Word -asiakirjoista, MS Excel -työkirjoista, MS PowerPoint -esityksistä, Adobe Photoshop -tiedostoista ja erilaisista kuvaformaateista. Saatavilla on hämmästyttävä määrä lisäominaisuuksia ja asetuksia.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Allekirjoitusten Qrcode vahvistaminen asiakirjassasi Zip"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) sisältää hyödyllisiä ominaisuuksia, kuten Qrcode-allekirjoituksia, jotka on sijoitettu Zip-asiakirjoihin. Käytä tätä mahdollisuutta ilman ylimääräistä koodia.
        
        * Ensinnäkin ilmennä Signature-luokka, joka tarjoaa konstruktoriparametripolun dokumenttiin, joka on tarkoitus varmentaa.
        * Toiseksi luo uusi VerifyOptions-objekti ja määritä kaikki tarvittavat ominaisuudet.
        * Lopuksi kutsu Signaturen objektin Verify-menetelmä, joka välittää VerifyOptions-ilmentymän.
        * Käsittele sitten vahvistustulokset.

    title_right: "Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for Java on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Lataa tuotteen GroupDocs.Signature for Java uusin versio osoitteesta [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Zip file
        String filePath = "input.zip";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitus Qrcode allekirjoituksilla Live-demo"
    content: |
       Lisää erilaisia ​​sähköisiä allekirjoituksia Zip-tiedostoon heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Vahvista muut Qrcode allekirjoitukset käyttämällä Java"
    content: |
        "Eri asiakirjoihin asetettujen sähköisten allekirjoitusten todentaminen. Tarkista suosituimpien tiedostomuotojen allekirjoitusten laatu, kuten alla on kerrottu."
    format: 
       
       
back_to_top:
    enable: true
---