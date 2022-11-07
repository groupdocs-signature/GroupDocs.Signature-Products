---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Otp
productName: Java
lang: lv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Otp for Java

############################# Head ############################
head_title: "Atjauniniet Text parakstus, kas ievietoti failos Otp ar Java"
head_description: "Izmantojiet vienkāršu un viegli saprotamu Java kodu Text parakstu atjaunināšanai parakstītos Otp dokumentos."

############################# Header ############################
title: "Rediģējiet un atjauniniet Text parakstus, kas ievietoti Otp failos"
description: "Java API nodrošina funkcionalitāti Text parakstu atjaunināšanai Otp dokumentos. Ātri un vienkārši atjauniniet e-parakstus savos Otp dokumentos, izmantojot pāris Java koda rindiņas."
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
    title: "Uzziniet par GroupDocs.Signature for Java API funkcijām"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API funkcionalitāte ietver plašu līdzekļu izvēli, lai apstrādātu pieprasītu dokumentu formātus, izmantojot elektroniskos parakstus. Tiek atbalstīts plašs e-parakstu klāsts, piemēram, teksti, attēli, digitālie sertifikāti, svītrkodi, QR kodi, zīmogi vai metadati. Klienti var pievienot, noņemt, rediģēt, apstiprināt vai meklēt ciparparakstus PDF failos, MS Word dokumentos, MS Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos. Ir pieejamas daudzas noderīgas funkcijas un iestatījumi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kā mainīt Text parakstus savā Otp dokumentā"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ietver noderīgas funkcijas, piemēram, Text parakstu atjaunināšanu, kas ievietoti Otp dokumentos. Tas ļauj mainīt parakstu funkcijas bez papildu koda.
        
        * Lai sāktu, izveidojiet paraksta objektu, kas pāriet kā konstruktora parametra ceļš uz dokumentu, kas ir jāatjaunina.
        * Pēc tam izveidojiet atbilstošu konkrēto paraksta objektu un iestatiet tā identifikatoru un rekvizītus, kas jāmaina.
        * Visbeidzot, izsauciet Signature's Update metodi, nododot noteiktu paraksta objektu.
        * Apstrādājiet rezultātu atjaunināšanu atbilstoši jūsu paziņojumam.

    title_right: "Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for Java tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Lejupielādējiet jaunāko GroupDocs.Signature for Java versiju no [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

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
    title: "Parakstu Text atjaunināšana dokumenta lapās — tiešraides demonstrācija"
    content: |
       Rediģējiet dažādus dokumenta Otp elektroniskos parakstus tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Atjauniniet dažādus Text parakstus, izmantojot Java"
    content: |
        "Dažādos dokumentu formātos ievietoto digitālo parakstu rediģēšana. Atjauniniet parakstu datus bez papildu koda."
    format: 
       
       
back_to_top:
    enable: true
---