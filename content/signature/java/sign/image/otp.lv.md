---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Otp
productName: Java
lang: lv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Otp for Java

############################# Head ############################
head_title: "Parakstu Image pievienošana failam Otp, izmantojot Java"
head_description: "Ievietojiet Image parakstu Otp failā Java, izmantojot dažas koda rindiņas. Izmantojiet GroupDocs Document Signature API, lai parakstītu desmitiem failu formātu."

############################# Header ############################
title: "Parakstīt Otp failus ar Image parakstiem programmā Java"
description: "Kā pievienot Image parakstu ar dažām Java koda rindām"
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
    title: "Par GroupDocs.Signature for Java attēla parakstu API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ir populāra API digitālo dokumentu e-parakstīšanai. Ir pieejami paraksti, piemēram, teksti, attēli, digitālie sertifikāti, svītrkodi, QR kodi, zīmogi vai metadati. Parakstus var ievietot PDF failos, MS Word dokumentos, MS Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos. Klienti var parakstīt savus dokumentus un atjaunināt, meklēt, pārbaudīt, dzēst vai priekšskatīt uz šiem dokumentiem uzliktos e-parakstus. Turklāt tiek nodrošinātas daudzas parakstu pielāgošanas iespējas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Darbības, lai parakstītu Otp ar Image programmā Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) nodrošina iespēju ātri un vienkārši parakstīt Otp dokumentus ar Image parakstiem.
        
        * Izveidojiet paraksta klases gadījumu, kas nodrošina Otp failu, kas paredzēts parakstīšanai kā ceļš vai atmiņas straume
        * Izveidojiet SignOptions klasi un iestatiet visus pieprasītos datus.
        * Izsauciet metodi Signature.Sign(), kas nodod izvades Otp failu vai atmiņas straumi

    title_right: " Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for Java tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Iegūstiet jaunāko GroupDocs.Signature for Java no [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Otp document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentu Otp parakstīšana, izmantojot Image tiešraides demonstrāciju"
    content: |
       Parakstiet Otp failu ar dažādiem parakstiem tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Jūs gaida bezmaksas tiešsaistes demonstrācija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Citi atbalstītie Image paraksti priekš Java"
    content: |
        "Varat arī parakstīt Otp ar citiem paraksta veidiem. Lūdzu, skatiet sarakstu zemāk."
    format: 
       
       
back_to_top:
    enable: true
---