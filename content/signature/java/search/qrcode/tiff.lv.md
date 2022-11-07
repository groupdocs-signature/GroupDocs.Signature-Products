---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Tiff
productName: Java
lang: lv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Tiff with Java

############################# Head ############################
head_title: "Meklēt Qrcode parakstus Tiff failā programmā Java"
head_description: "Izmantojiet Java, lai meklētu Qrcode parakstus Tiff failos, izmantojot dažas koda rindiņas."

############################# Header ############################
title: "Meklējiet Qrcode parakstus failā Tiff"
description: "Java vietējais API ļauj meklēt Qrcode parakstus jau parakstītos Tiff failos. Veiciet izvērsto e-paraksta meklēšanu savos Tiff dokumentos, izmantojot dažas koda rindiņas."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Par GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) nodrošina Java API dokumentu apstrādei, izmantojot dažādus parakstu veidus, piemēram, tekstus, attēlus, digitālos sertifikātus, svītrkodus, QR kodus, zīmogus vai metadatus. Lietotāji var pievienot, dzēst, atjaunināt, pārbaudīt vai meklēt elektroniskos parakstus PDF failos, MS Word dokumentos, MS Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos ar papildu atbalstu parakstu rekvizītu pielāgošanai pēc vajadzības.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kā meklēt Qrcode parakstus Tiff"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ļauj Java izstrādātājiem vieglāk meklēt Qrcode parakstus Tiff failos no savām lietojumprogrammām, veicot dažas vienkāršas darbības.
        
        * Izveidojiet jaunu Signature klases gadījumu un norādiet avota dokumenta ceļu kā konstruktora parametru.
        * Izveidojiet SearchOptions objektu atbilstoši savām prasībām un norādiet meklēšanas opcijas.
        * Izsauciet Signature klases instances meklēšanas metodi un nosūtiet tai SearchOptions.
        * Apstrādājiet meklēšanas rezultātus atbilstoši savām prasībām.

    title_right: "Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for Java tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Lejupielādējiet jaunāko GroupDocs.Signature for Java versiju no [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Tiff document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Meklēt Qrcode elektronisko parakstu tiešraides demonstrāciju"
    content: |
       Meklējiet dokumentā dažādus Tiff failu elektroniskos parakstus tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Meklēt citus Qrcode parakstus, izmantojot Java"
    content: |
        "Elektronisko parakstu meklēšana dažādos dokumentos. Atrodiet parakstus no viena no populārajiem failu formātiem, kā parādīts tālāk."
    format: 
           
       
back_to_top:
    enable: true
---