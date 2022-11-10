---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Ods
productName: Java
lang: et
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ods for Java

############################# Head ############################
head_title: "Digital allkirjade kontrollimine failide Ods jaoks läbi Java"
head_description: "Kasutage Ods dokumentide ja nende allkirjade Digital kontrollimiseks ainult mõnda rida Java koodi."

############################# Header ############################
title: "Digital allkirjade kontrollimine faili Ods jaoks"
description: "API for Java annab võimaluse kontrollida Digital allkirju Ods dokumentides. Teie Ods dokumentides olevate e-allkirjade kontrollimine võib toimuda kiiresti ja lihtsalt."
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
    title: "Avastage GroupDocs.Signature for Java API uusi funktsioone"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API pakub laias valikus viise mitmesuguste dokumendivormingute töötlemiseks elektrooniliste allkirjade abil. Toetatakse mitut tüüpi digitaalallkirju, nagu tekstid, pildid, digitaalsed sertifikaadid, vöötkoodid, QR-koodid, templid või metaandmed. Kliendid saavad lisada, eemaldada, redigeerida, kinnitada või otsida digitaalallkirju PDF-ides, MS Wordi dokumentides, MS Exceli töövihikutes, MS PowerPointi esitlustes, Adobe Photoshopi failides ja erinevates pildivormingutes. Saadaval on hämmastav hulk lisafunktsioone ja seadeid.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kuidas kontrollida allkirja Digital oma dokumendis Ods"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) sisaldab kasulikke funktsioone, nagu Digital allkirjade kontrollimine, mis on pandud dokumentidele Ods. Kasutage seda võimalust lisakoodi rakendamata.
        
        * Esiteks instantseerige Signature klass, mis annab konstruktori parameetri tee dokumendile, mis peaks olema kontrollitud.
        * Teiseks looge uus VerifyOptions objekt ja seadistage kõik vajalikud atribuudid.
        * Lõpuks käivitage Signature'i objekti Verify meetod, mis läbib VerifyOptions eksemplari.
        * Seejärel töödelge kinnitustulemusi.

    title_right: "Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for Java toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laadige alla toote GroupDocs.Signature for Java uusim versioon saidilt [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
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
    title: "Allkirjastamine Digital allkirjaga Live Demo"
    content: |
       Lisage kohe failile Ods erinevad elektroonilised allkirjad, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kontrollige teisi Digital allkirju, kasutades Java"
    content: |
        "Erinevatesse dokumentidesse pandud elektrooniliste allkirjade kontrollimine. Kontrollige allkirjade kvaliteeti populaarsetes failivormingutes, nagu on näidatud allpool."
    format: 
       
       
back_to_top:
    enable: true
---