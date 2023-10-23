---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Zip
productName: Java
lang: lt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Zip for Java

############################# Head ############################
head_title: "Qrcode failų Zip parašų patvirtinimas naudojant Java"
head_description: "Naudokite tik kelias Java kodo eilutes, kad patikrintumėte Zip dokumentus ir jų Qrcode parašus."

############################# Header ############################
title: "Qrcode parašų patvirtinimas Zip failams"
description: "API, skirta Java, suteikia galimybę patvirtinti Qrcode parašus Zip dokumentuose. El. parašų patvirtinimas jūsų Zip dokumentuose gali būti atliktas greitai ir paprastai."
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
    title: "Atraskite naujas GroupDocs.Signature for Java API funkcijas"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API suteikia daug įvairių būdų, kaip apdoroti įvairių formatų dokumentus naudojant elektroninius parašus. Palaikomi daugelio tipų skaitmeniniai parašai, tokie kaip tekstai, vaizdai, skaitmeniniai sertifikatai, brūkšniniai kodai, QR kodai, antspaudai ar metaduomenys. Klientai gali pridėti, pašalinti, redaguoti, patvirtinti arba ieškoti skaitmeninių parašų PDF, MS Word dokumentuose, MS Excel darbaknygėse, MS PowerPoint pristatymuose, Adobe Photoshop failuose ir įvairiuose vaizdo formatuose. Galimas stulbinantis papildomų funkcijų ir nustatymų skaičius.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kaip patvirtinti Qrcode parašus Zip dokumente"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) apima naudingas funkcijas, pvz., Qrcode parašų, pateiktų Zip dokumentuose, patvirtinimą. Pasinaudokite šia galimybe neįdiegę papildomo kodo.
        
        * Pirma, sukurkite parašo klasę, kaip konstruktoriaus parametro kelią į dokumentą, kuris turėtų būti patikrintas.
        * Antra, sukurkite naują VerifyOptions objektą ir nustatykite visas reikalingas ypatybes.
        * Galiausiai iškvieskite Signature objekto Verify metodą, perduodantį VerifyOptions egzempliorių.
        * Tada apdorokite patikrinimo rezultatus.

    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for Java palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Atsisiųskite naujausią GroupDocs.Signature for Java versiją iš [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
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
    title: "Pasirašymas naudojant Qrcode parašus Tiesioginė demonstracija"
    content: |
       Pridėkite įvairių elektroninių parašų prie Zip failo dabar, apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Patikrinkite kitus Qrcode parašus naudodami Java"
    content: |
        "Įvairiuose dokumentuose dedamų elektroninių parašų tikrinimas. Patikrinkite parašų kokybę populiariuose failų formatuose, kaip parodyta toliau."
    format: 
       
       
back_to_top:
    enable: true
---