---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Ppsm
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Ppsm for Java

############################# Head ############################
head_title: "Afegint Image signatures al fitxer Ppsm amb Java"
head_description: "Poseu la signatura Image al fitxer Ppsm per a Java utilitzant unes quantes línies de codi. Utilitzeu l'API de signatura de documents de GroupDocs per signar desenes de formats de fitxer."

############################# Header ############################
title: "Signa fitxers Ppsm amb signatures Image a Java"
description: "Com afegir la signatura Image amb unes poques línies de codi Java"
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
    title: "Sobre l'API de signatures d'imatge de GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) és una API popular per a la signatura electrònica de documents digitals. Hi ha signatures com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Les signatures es poden col·locar en PDF, documents MS Word, llibres de treball de MS Excel, presentacions de MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Els clients poden signar el seu document i actualitzar, cercar, verificar, suprimir o previsualitzar les signatures electròniques que es van posar en aquests documents. A més, es proporcionen moltes capacitats per a la personalització de signatures.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passos per signar Ppsm amb Image a Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ofereix la possibilitat de signar documents Ppsm amb signatures Image de manera ràpida i senzilla.
        
        * Creeu una instància de la classe Signature que proporcioni el fitxer Ppsm que s'ha de signar com a camí o flux de memòria
        * Instancieu la classe SignOptions i configureu totes les dades sol·licitades.
        * Invoqueu el mètode Signature.Sign() passant el fitxer de sortida Ppsm o el flux de memòria

    title_right: " Requisits del sistema"
    content_right: |
        GroupDocs.Signature for Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obteniu l'últim GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ppsm file
        String filePath = "input.ppsm";
        // Set up output file
        String outputFilePath = "output.ppsm";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ppsm document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant documents de Ppsm amb Image Demostració en directe"
    content: |
       Signa el fitxer Ppsm amb diverses signatures ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostració gratuïta en línia esperant-te.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altres signatures admeses de Image per a Java"
    content: |
        "També podeu signar Ppsm amb altres tipus de signatura. Si us plau, consulteu la llista a continuació."
    format: 
       
       
back_to_top:
    enable: true
---