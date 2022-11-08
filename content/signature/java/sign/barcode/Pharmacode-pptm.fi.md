---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Pptm
productName: Java
lang: fi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pptm for Java

############################# Head ############################
head_title: "eSign Pptm -asiakirja Pharmacode-viivakoodilla Java"
head_description: "Luo Pharmacode Viivakoodiallekirjoitus ja laita se Pptm-asiakirjaan, jossa on Java muutamalla rivillä koodia. Käytä GroupDocs Document Signature API:ta eri tiedostomuotojen allekirjoittamiseen."

############################# Header ############################
title: "Luo Pharmacode viivakoodiallekirjoitus asiakirjalle Pptm ohjelmassa Java"
description: "eAllekirjoita Pptm yritysasiakirjasi Pharmacode-viivakoodilla. Luo viivakoodiallekirjoitus nopeasti ja helposti muutamalla koodirivillä allekirjoitusvaihtoehtojen määrittämiseksi."
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
    title: "Tietoja GroupDocs.Signature for Java Viivakoodin allekirjoitusten sovellusliittymästä."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) on nopea ja helppo sovellusliittymä digitaalisten asiakirjojen sähköiseen allekirjoittamiseen käyttämällä viivakoodityyppejä, kuten UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 ja monet muut. Asiakkaat voivat luoda helposti tarvittavan tekstin sisältäviä viivakoodeja ja laittaa ne PDF-tiedostoihin, Microsoft Office Words -asiakirjoihin, Microsoft Office Excel -työkirjoihin, MS PowerPoint -esityksiin, Adobe Photoshop -tiedostoihin ja erilaisiin kuvamuotoihin. Asiakirjoihin sijoitettuja viivakoodeja voidaan päivittää, etsiä, tarkistaa, poistaa tai esikatsella joko. Lisäksi viivakoodien räätälöintiä tuetaan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Pptm:n allekirjoittamiseen Barcode -sovelluksella Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) tarjoaa mahdollisuuden allekirjoittaa Pptm-asiakirjoja Barcode-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Pptm-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Pptm -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for Java on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Hanki uusin GroupDocs.Signature for Java käyttäjältä [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptm file
        String filePath = "input.pptm";
        // Set up output file
        String outputFilePath = "output.pptm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Pharmacode);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Pptm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Pptm asiakirjoja Barcode Live-demolla"
    content: |
       Allekirjoita Pptm-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, joka tunnetaan myös nimellä Pharmaceutical Binary Code, on viivakoodistandardi, jota käytetään lääketeollisuudessa pakkausten valvontajärjestelmänä.
          characterset: |
             Numeeriset numerot (0-9).
          textcapacity: |
             Edustaa vain yhtä kokonaislukua väliltä 3 - 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Barcode allekirjoitukset ohjelmalle Java"
    content: |
        "Voit myös allekirjoittaa Pptm muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
        
       
back_to_top:
    enable: true
---