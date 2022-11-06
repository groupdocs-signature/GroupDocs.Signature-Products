---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Qrcode
fileformat: Xlsx
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Xlsx for Java

############################# Head ############################
head_title: "Actualitza les signatures de Qrcode col·locades als fitxers Xlsx amb Java"
head_description: "Utilitzeu el codi Java senzill i fàcil d'entendre per a l'actualització de signatures de Qrcode en documents de Xlsx signats."

############################# Header ############################
title: "Editeu i actualitzeu les signatures Qrcode col·locades als fitxers Xlsx"
description: "L'API per a Java proporciona funcionalitat per a les signatures de Qrcode que s'actualitzen als documents Xlsx. Actualitzeu les signatures electròniques dins dels vostres documents Xlsx amb un parell de línies de codi Java de manera ràpida i senzilla."
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
    title: "Més informació sobre les funcions de l'API de GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) La funcionalitat de l'API conté una àmplia selecció de mitjans per processar en formats de documents de demanda mitjançant signatures electròniques. S'admet un ampli espectre de signatures electròniques com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els clients poden afegir, eliminar, editar, validar o cercar signatures digitals en PDF, documents MS Word, llibres de treball de MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Hi ha disponibles nombroses funcions i configuracions útils.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com canviar les signatures de Qrcode al vostre document Xlsx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inclou funcions útils com ara l'actualització de signatures de Qrcode col·locades als documents Xlsx. Permet canviar les funcions de signatures sense codi addicional.
        
        * Per començar, creeu un objecte Signature passant com a ruta del paràmetre del constructor a un document que se suposa que s'ha d'actualitzar.
        * A continuació, instància un objecte de signatura particular adequat i configureu-ne l'identificador i les propietats que cal canviar.
        * Finalment, truqueu al mètode d'actualització de la signatura passant un objecte de signatura particular.
        * Processa els resultats d'actualització segons el teu avís.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Baixeu la darrera versió de GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsx file
        String filePath = "input.xlsx";
        // Set up output file
        String outputFilePath = "output.xlsx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        QrCodeSignature signatureToUpdate = new QrCodeSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(200);
        // specify signature height
        signatureToUpdate.setHeight(200);
        // set left position
        signatureToUpdate.setLeft(120);
        // set top position
        signatureToUpdate.setTop(160);

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
    title: "Actualització de les signatures de Qrcode a les pàgines del document - Demostració en directe"
    content: |
       Editeu diverses signatures electròniques del document Xlsx ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Actualitzeu diverses signatures de Qrcode mitjançant Java"
    content: |
        "Edició de signatures digitals que es col·loquen en diferents formats de documents. Actualitza les dades de signatures sense codi addicional."
    format: 
       
       
back_to_top:
    enable: true
---