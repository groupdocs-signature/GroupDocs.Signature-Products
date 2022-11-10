---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Docm
productName: Java
lang: hu
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Docm for Java

############################# Head ############################
head_title: "Metaadat elektronikus aláírások csatolása a Docm dokumentumokhoz a Java segítségével"
head_description: "Használja a metaadatokat rejtett elektronikus aláírásként a Docm dokumentumaiban néhány soros Java kód használatával. A GroupDocs Document Signature API használatával elektronikusan aláírhatja üzleti dokumentumait és fájljait metaadat-információkkal."

############################# Header ############################
title: "A Docm dokumentum metaadat-elektronikus aláírása a Java-on keresztül egyszerű és könnyen használható!"
description: "eAláírja Docm dokumentumait és szerződéseit rejtett metaadat-bejegyzésekkel. Metaadatok generálása PDF-ekhez, MS Word dokumentumokhoz, MS Excel munkafüzetekhez, MS PowerPoint prezentációkhoz és különféle képformátumokhoz probléma és extra kódolás nélkül."
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
    title: "A GroupDocs.Signature for Java metaadat-aláírások API-járól"
    content: |
        A [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) egy népszerű API a digitális dokumentumok elektronikus aláírására. Aláírások, például szövegek, képek, digitális tanúsítványok, vonalkódok, QR-kódok, bélyegzők vagy metaadatok állnak rendelkezésre. Az aláírások elhelyezhetők PDF-eken, MS Word dokumentumokon, MS Excel munkafüzeteken, MS PowerPoint prezentációkban, Adobe Photoshop fájlokon és különféle képformátumokban. Az ügyfelek aláírhatják dokumentumaikat, és frissíthetik, kereshetik, ellenőrizhetik, törölhetik vagy megtekinthetik a dokumentumokon elhelyezett e-aláírásokat. Ezenkívül számos lehetőség áll rendelkezésre az aláírások testreszabásához.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "A Docm aláírásának lépései a Metadata segítségével a Java programban"
    content_left: |
        A [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) lehetővé teszi a Docm dokumentumok gyors és egyszerű aláírását Metadata aláírással.
        
        * Hozzon létre egy példányt a Signature osztályból, amely Docm fájlt tartalmaz, amelyet elérési útként vagy memóriafolyamként kell aláírni
        * Példányosítsa a SignOptions osztályt, és állítsa be az összes kért adatot.
        * Hívja meg a Signature.Sign() metódust, amely átadja a kimeneti Docm fájlt vagy memóriafolyamot

    title_right: " rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for Java minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Szerezze meg a legújabb GroupDocs.Signature for Java terméket a következőtől: [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Docm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Docm dokumentumok aláírása Metadata élő bemutatóval"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhelyen azonnal írjon alá Docm fájlt különféle aláírásokkal. Ingyenes online demo vár rád.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Egyéb támogatott Metadata aláírások a Java számára"
    content: |
        "A Docm más aláírástípusokkal is aláírható. Kérjük, tekintse meg az alábbi listát."
    format: 
       
       
back_to_top:
    enable: true
---