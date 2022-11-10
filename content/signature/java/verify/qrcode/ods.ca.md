---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Ods
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Ods for Java

############################# Head ############################
head_title: "Verificació de signatures de Qrcode per a fitxers Ods mitjançant Java"
head_description: "Utilitzeu només unes poques línies de codi Java per verificar els documents Ods i les seves signatures Qrcode."

############################# Header ############################
title: "Qrcode verificació de signatures per a fitxers Ods"
description: "L'API per a Java ofereix l'oportunitat de verificar les signatures de Qrcode als documents Ods. La verificació de les signatures electròniques dins dels vostres documents Ods es pot fer de manera ràpida i senzilla."
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
    title: "Descobriu noves funcions de l'API de GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API ofereix una àmplia gamma de maneres de processar nombrosos formats de documents mitjançant signatures electròniques. S'admeten molts tipus de signatures digitals com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els clients poden afegir, eliminar, editar, validar o cercar signatures digitals en PDF, documents MS Word, llibres de treball de MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Hi ha disponibles un nombre sorprenent de funcions i configuracions addicionals.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com validar les signatures de Qrcode al vostre document Ods"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inclou funcions útils com la verificació de les signatures de Qrcode col·locades als documents de Ods. Aprofiteu aquesta oportunitat sense implementar codi addicional.
        
        * En primer lloc, instanciïu la classe Signature proporcionant com a paràmetre de constructor la ruta d'accés a un document que se suposa que s'ha de verificar.
        * En segon lloc, creeu un nou objecte VerifyOptions i configureu totes les propietats necessàries.
        * Finalment, invoqueu el mètode Verify de l'objecte de Signature passant la instància VerifyOptions.
        * A continuació, processeu els resultats de la verificació.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Baixeu la darrera versió de GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";

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
    title: "Signant amb Qrcode signatures Demostració en directe"
    content: |
       Afegiu diverses signatures electròniques al fitxer Ods ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifiqueu altres signatures de Qrcode mitjançant Java"
    content: |
        "Verificació de signatures electròniques col·locades en diversos documents. Comproveu la qualitat de les signatures en els formats de fitxer populars, tal com es mostra a continuació."
    format: 
       
       
back_to_top:
    enable: true
---