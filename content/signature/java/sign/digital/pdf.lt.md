---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pdf
productName: Java
lang: lt
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pdf for Java

############################# Head ############################
head_title: "Skaitmeninių elektroninių parašų pridėjimas prie failo Pdf naudojant Java"
head_description: "Įdėkite skaitmeninį parašą į Pdf failą, skirtą Java, naudodami kelias kodo eilutes. Norėdami pasirašyti daugybę failų formatų, naudokite GroupDocs Document Signature API."

############################# Header ############################
title: "eSign Pdf failai su Digital parašais Java"
description: "Kaip pridėti Digital parašą su keliomis Java kodo eilutėmis"
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
    title: "Apie GroupDocs.Signature for Java skaitmeninių parašų API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) yra populiari API, skirta dokumentams pasirašyti su skaitmeniniais elektroniniais parašais ir skaitmeniniais sertifikatais. Skaitmeninių parašų API naudoja PFX sertifikatų failus, kad pasirašytų dokumentą su slaptažodžiu apsaugotais privačiais ir viešaisiais raktais. Skaitmeniniai parašai gali būti naudojami verslo dokumentams sertifikuoti naudojant eSign PDF konkretų puslapį, sertifikuoti visus Microsoft Office dokumentus, pvz., Words, Excel, Powerpoint failus ir Open Office dokumentus. Klientai gali lengvai manipuliuoti parašais, pavyzdžiui, juos redaguoti, pašalinti ar koreguoti. API suteikia galimybę ieškoti ir patikrinti parašus. Be to, suteikiama daug parašų pritaikymo galimybių.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Veiksmai norint pasirašyti Pdf naudojant Digital programoje Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) suteikia galimybę greitai ir lengvai pasirašyti Pdf dokumentus su Digital parašais.
        
        * Sukurkite parašo klasės egzempliorių, pateikiantį Pdf failą, kuris turėtų būti pasirašytas kaip kelias arba atminties srautas
        * Sukurkite SignOptions klasę ir nustatykite visus reikalingus duomenis.
        * Iškvieskite Signature.Sign() metodą, perduodantį išvesties Pdf failą arba atminties srautą

    title_right: " Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for Java palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Gaukite naujausią GroupDocs.Signature for Java iš [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";
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

        // sign Pdf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentų Pdf pasirašymas naudojant Digital tiesioginę demonstraciją"
    content: |
       Pasirašykite Pdf failą įvairiais parašais dabar apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje. Jūsų laukia nemokama internetinė demonstracinė versija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kiti palaikomi Digital parašai, skirti Java"
    content: |
        "Taip pat galite pasirašyti Pdf naudodami kitų tipų parašus. Žiūrėkite žemiau esantį sąrašą."
    format: 
       
       
back_to_top:
    enable: true
---