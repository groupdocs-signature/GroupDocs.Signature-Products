---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Docm
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docm for Java

############################# Head ############################
head_title: "Afegir signatures electròniques digitals al fitxer Docm amb Java"
head_description: "Col·loqueu la signatura digital al fitxer Docm per a Java utilitzant unes quantes línies de codi. Utilitzeu l'API de signatura de documents de GroupDocs per signar desenes de formats de fitxer."

############################# Header ############################
title: "eSign fitxers Docm amb signatures Digital a Java"
description: "Com afegir la signatura Digital amb unes poques línies de codi Java"
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
    title: "Sobre l'API de signatures digitals de GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) és una API popular per signar documents amb signatures electròniques digitals, amb certificats digitals. Per a l'API de signatures digitals, utilitza fitxers de certificat PFX per signar el document amb claus públiques i privades protegides amb contrasenya. Les signatures digitals es poden utilitzar per certificar documents empresarials amb eSign PDF en particular, certificar documents sencers de Microsoft Office com Words, Excel, fitxers Powerpoint i documents d'Open Office. Els clients poden manipular fàcilment les signatures com editar-les, eliminar-les o ajustar-les. L'API proporciona una manera de cercar i verificar signatures. A més, es proporcionen moltes capacitats per a la personalització de signatures.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passos per signar Docm amb Digital a Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ofereix la possibilitat de signar documents Docm amb signatures Digital de manera ràpida i senzilla.
        
        * Creeu una instància de la classe Signature que proporcioni el fitxer Docm que s'ha de signar com a camí o flux de memòria
        * Instancieu la classe SignOptions i configureu totes les dades sol·licitades.
        * Invoqueu el mètode Signature.Sign() passant el fitxer de sortida Docm o el flux de memòria

    title_right: " Requisits del sistema"
    content_right: |
        GroupDocs.Signature for Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obteniu l'últim GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Docm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant documents de Docm amb Digital Demostració en directe"
    content: |
       Signa el fitxer Docm amb diverses signatures ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostració gratuïta en línia esperant-te.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altres signatures admeses de Digital per a Java"
    content: |
        "També podeu signar Docm amb altres tipus de signatura. Si us plau, consulteu la llista a continuació."
    format: 
       
       
back_to_top:
    enable: true
---