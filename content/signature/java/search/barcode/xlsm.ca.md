---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Xlsm
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Xlsm with Java

############################# Head ############################
head_title: "Cerqueu signatures de Barcode al fitxer Xlsm a Java"
head_description: "Utilitzeu Java per cercar signatures Barcode als fitxers Xlsm mitjançant unes poques línies de codi."

############################# Header ############################
title: "Cerqueu signatures Barcode al fitxer Xlsm"
description: "L'API nativa de Java permet cercar signatures Barcode als fitxers Xlsm ja signats. Feu una cerca avançada de signatura electrònica als vostres documents Xlsm amb unes poques línies de codi."
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
    title: "Sobre l'API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) proporciona l'API de Java per processar documents amb diversos tipus de signatura, com ara textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els usuaris poden afegir, suprimir, actualitzar, verificar o cercar signatures electròniques en PDF, documents MS Word, llibres de treball MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge, amb suport addicional per personalitzar les propietats de les signatures segons sigui necessari.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com cercar signatures de Barcode a Xlsm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) facilita que els desenvolupadors de Java cerquin signatures de Barcode als fitxers Xlsm des de les seves aplicacions implementant uns quants passos senzills.
        
        * Creeu una nova instància de la classe Signature i passeu la ruta del document font com a paràmetre de constructor.
        * Instancieu l'objecte SearchOptions segons els vostres requisits i especifiqueu les opcions de cerca.
        * Truqueu al mètode de cerca de la instància de classe Signature i passeu-li SearchOptions.
        * Processeu els resultats de la cerca segons les vostres demandes.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Baixeu la darrera versió de GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Xlsm file
        String filePath = "input.xlsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        BarcodeSearchOptions options = new BarcodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Barcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Barcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Barcode signatures in Xlsm document
        List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cerqueu Barcode signatures electròniques Demostració en directe"
    content: |
       Cerqueu al document diverses signatures electròniques als fitxers Xlsm ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cerqueu altres signatures de Barcode amb Java"
    content: |
        "Cerca de signatures electròniques en diversos documents. Cerqueu signatures d'un dels formats de fitxer més populars, tal com es mostra a continuació."
    format: 
           
       
back_to_top:
    enable: true
---