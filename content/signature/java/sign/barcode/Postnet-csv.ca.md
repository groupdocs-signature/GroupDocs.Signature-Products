---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Postnet
fileformat: Csv
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Csv for Java

############################# Head ############################
head_title: "Document electrònic Csv amb codi de barres Postnet a Java"
head_description: "Creeu la signatura de codi de barres Postnet i poseu-la al document Csv amb Java utilitzant un parell de línies de codi. Utilitzeu l'API de signatura de documents de GroupDocs per signar diversos formats de fitxer."

############################# Header ############################
title: "Genereu Postnet signatura de codi de barres per al document Csv a Java"
description: "eSigne els vostres documents comercials de Csv amb el codi de barres Postnet. Genereu la signatura de codi de barres de manera ràpida i senzilla amb unes poques línies de codi per configurar les opcions de signatura."
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
    title: "Sobre l'API de signatures de codi de barres de GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) és una API ràpida i senzilla per gestionar la signatura electrònica de documents digitals mitjançant tipus de codi de barres com UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 i molts altres. Els clients poden crear fàcilment codis de barres que proporcionen el text necessari i posar-los en PDF, documents de Microsoft Office Words, llibres de treball de Microsoft Office Excel, presentacions de MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Els codis de barres col·locats als documents es poden actualitzar, cercar, verificar, suprimir o visualitzar prèviament. A més, s'admet la personalització de codis de barres.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passos per signar Csv amb Barcode a Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ofereix la possibilitat de signar documents Csv amb signatures Barcode de manera ràpida i senzilla.
        
        * Creeu una instància de la classe Signature que proporcioni el fitxer Csv que s'ha de signar com a camí o flux de memòria
        * Instancieu la classe SignOptions i configureu totes les dades sol·licitades.
        * Invoqueu el mètode Signature.Sign() passant el fitxer de sortida Csv o el flux de memòria

    title_right: " Requisits del sistema"
    content_right: |
        GroupDocs.Signature for Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obteniu l'últim GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Csv file
        String filePath = "input.csv";
        // Set up output file
        String outputFilePath = "output.csv";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Postnet);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Csv document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant documents de Csv amb Barcode Demostració en directe"
    content: |
       Signa el fitxer Csv amb diverses signatures ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostració gratuïta en línia esperant-te.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Postnet Barcode"
          content: |
            POSTNET (Tècnica de codificació numèrica postal) és una simbologia de codi de barres utilitzada pel servei postal dels Estats Units per ajudar a dirigir el correu.
          characterset: |
             Dígits numèrics (0-9).
          textcapacity: |
             Fins a 11 caràcters.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAACcAAAAjCAYAAAAXMhMjAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACeSURBVFhH7c7BCkMxEELR/P9Pp1LoRrCXpi4Cbw5kIRKZtS82x52a407Ncae+HrfWer8Pyr+i/3NcQv/nuIT+z3EJ/X/Ocf9mlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2ubnAHHdqjjt18XF7vwDevzbHqsQWPwAAAABJRU5ErkJggg==

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altres signatures admeses de Barcode per a Java"
    content: |
        "També podeu signar Csv amb altres tipus de signatura. Si us plau, consulteu la llista a continuació."
    format: 
        
       
back_to_top:
    enable: true
---