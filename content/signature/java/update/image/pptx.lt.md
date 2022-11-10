---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Pptx
productName: Java
lang: lt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Pptx for Java

############################# Head ############################
head_title: "Atnaujinkite Image parašus, pateiktus Pptx failuose naudodami Java"
head_description: "Naudokite paprastą ir lengvai suprantamą Java kodą Image parašų atnaujinimui pasirašytuose Pptx dokumentuose."

############################# Header ############################
title: "Redaguoti ir atnaujinti Image parašus, esančius Pptx failuose"
description: "API, skirta Java, teikia Image parašų atnaujinimo funkciją Pptx dokumentuose. Greitai ir lengvai atnaujinkite el. parašus savo Pptx dokumentuose naudodami kelias Java kodo eilutes."
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
    title: "Sužinokite apie GroupDocs.Signature for Java API funkcijas"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API funkcija apima daugybę priemonių, skirtų apdoroti pageidaujamų formatų dokumentus naudojant elektroninius parašus. Palaikomas platus el. parašų spektras, pavyzdžiui, tekstai, vaizdai, skaitmeniniai sertifikatai, brūkšniniai kodai, QR kodai, antspaudai ar metaduomenys. Klientai gali pridėti, pašalinti, redaguoti, patvirtinti arba ieškoti skaitmeninių parašų PDF, MS Word dokumentuose, MS Excel darbaknygėse, MS PowerPoint pristatymuose, Adobe Photoshop failuose ir įvairiuose vaizdo formatuose. Yra daug naudingų funkcijų ir nustatymų.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kaip pakeisti Image parašus Pptx dokumente"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) apima naudingų funkcijų, pvz., Image parašų, esančių Pptx dokumentuose, atnaujinimas. Tai leidžia pakeisti parašo funkcijas be papildomo kodo.
        
        * Norėdami pradėti, sukurkite parašo objektą, kuris kaip konstruktoriaus parametro kelias į dokumentą, kuris turėtų būti atnaujintas.
        * Tada sukurkite atitinkamą konkretų parašo objektą ir nustatykite jo identifikatorių bei savybes, kurias reikia pakeisti.
        * Galiausiai iškvieskite parašo atnaujinimo metodą, perduodant tam tikrą parašo objektą.
        * Apdorokite rezultatų atnaujinimą pagal jūsų pranešimą.

    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for Java palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Atsisiųskite naujausią GroupDocs.Signature for Java versiją iš [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";
        // Set up output file
        String outputFilePath = "output.pptx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image parašų atnaujinimas dokumento puslapiuose – tiesioginė demonstracija"
    content: |
       Šiuo metu redaguokite įvairius elektroninius Pptx dokumento parašus apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Atnaujinkite įvairius Image parašus naudodami Java"
    content: |
        "Skaitmeninių parašų, kurie dedami į įvairius dokumentų formatus, redagavimas. Atnaujinkite parašų duomenis be papildomo kodo."
    format: 
       
       
back_to_top:
    enable: true
---