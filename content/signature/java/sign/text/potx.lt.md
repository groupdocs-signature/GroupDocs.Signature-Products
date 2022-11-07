---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Potx
productName: Java
lang: lt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Potx for Java

############################# Head ############################
head_title: "Sukurkite tekstinius elektroninius parašus į failą Potx naudodami Java"
head_description: "Įdėkite Text el. parašą į Potx failą, skirtą Java, naudodami kelias kodo eilutes. Norėdami pasirašyti daugybę failų formatų, naudokite GroupDocs Document Signature API."

############################# Header ############################
title: "Pasirašykite Potx failus naudodami Text parašus Java"
description: "Kaip pridėti Text parašą su keliomis Java kodo eilutėmis"
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
    title: "Apie GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) yra populiari skaitmeninių dokumentų el. pasirašymo API. Galimi parašai, tokie kaip tekstai, vaizdai, skaitmeniniai sertifikatai, brūkšniniai kodai, QR kodai, antspaudai ar metaduomenys. Parašai gali būti dedami ant PDF, MS Word dokumentų, MS Excel darbaknygų, MS PowerPoint pristatymų, Adobe Photoshop failų ir įvairių vaizdų formatų. Klientai gali pasirašyti savo dokumentą ir atnaujinti, ieškoti, tikrinti, ištrinti ar peržiūrėti ant tų dokumentų įrašytus el. Be to, suteikiama daug parašų pritaikymo galimybių.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Veiksmai norint pasirašyti Potx naudojant Text programoje Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) suteikia galimybę greitai ir lengvai pasirašyti Potx dokumentus su Text parašais.
        
        * Sukurkite parašo klasės egzempliorių, pateikiantį Potx failą, kuris turėtų būti pasirašytas kaip kelias arba atminties srautas
        * Sukurkite SignOptions klasę ir nustatykite visus reikalingus duomenis.
        * Iškvieskite Signature.Sign() metodą, perduodantį išvesties Potx failą arba atminties srautą

    title_right: " Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for Java palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Gaukite naujausią GroupDocs.Signature for Java iš [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potx file
        String filePath = "input.potx";
        // Set up output file
        String outputFilePath = "output.potx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Potx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentų Potx pasirašymas naudojant Text tiesioginę demonstraciją"
    content: |
       Pasirašykite Potx failą įvairiais parašais dabar apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje. Jūsų laukia nemokama internetinė demonstracinė versija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kiti palaikomi Text parašai, skirti Java"
    content: |
        "Taip pat galite pasirašyti Potx naudodami kitų tipų parašus. Žiūrėkite žemiau esantį sąrašą."
    format: 
       
       
back_to_top:
    enable: true
---