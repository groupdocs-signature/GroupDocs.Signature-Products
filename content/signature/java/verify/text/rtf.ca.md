---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Rtf
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Rtf for Java

############################# Head ############################
head_title: "Verificació de signatures de Text per a fitxers Rtf mitjançant Java"
head_description: "Utilitzeu només unes poques línies de codi Java per verificar els documents Rtf i les seves signatures Text."

############################# Header ############################
title: "Text verificació de signatures per a fitxers Rtf"
description: "L'API per a Java ofereix l'oportunitat de verificar les signatures de Text als documents Rtf. La verificació de les signatures electròniques dins dels vostres documents Rtf es pot fer de manera ràpida i senzilla."
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
    title_left: "Com validar les signatures de Text al vostre document Rtf"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inclou funcions útils com la verificació de les signatures de Text col·locades als documents de Rtf. Aprofiteu aquesta oportunitat sense implementar codi addicional.
        
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
                
        // Set up input Rtf file
        String filePath = "input.rtf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        TextVerifyOptions options = new TextVerifyOptions();

        // Process all pages
        options.setAllPages(true);
        // specify text match type
        options.setMatchType(TextMatchType.Exact);
        // specify text pattern to search
        options.setText("Very important signature");
                            
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
    title: "Signant amb Text signatures Demostració en directe"
    content: |
       Afegiu diverses signatures electròniques al fitxer Rtf ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifiqueu altres signatures de Text mitjançant Java"
    content: |
        "Verificació de signatures electròniques col·locades en diversos documents. Comproveu la qualitat de les signatures en els formats de fitxer populars, tal com es mostra a continuació."
    format: 
       
       
back_to_top:
    enable: true
---