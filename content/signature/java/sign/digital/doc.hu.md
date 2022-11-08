---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: Java
lang: hu
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for Java

############################# Head ############################
head_title: "Digitális elektronikus aláírás hozzáadása a Doc fájlhoz a Java segítségével"
head_description: "Helyezze el a digitális aláírást a Java Doc fájljába néhány sor kód használatával. A GroupDocs Document Signature API segítségével több tucat fájlformátumot írhat alá."

############################# Header ############################
title: "eSign Doc fájlok Digital aláírással a Java nyelven"
description: "Digital aláírás hozzáadása néhány soros Java kóddal"
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
    title: "A GroupDocs.Signature for Java digitális aláírás API-ról"
    content: |
        A [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) egy népszerű API dokumentumok digitális elektronikus aláírással és digitális tanúsítványokkal történő aláírására. A digitális aláírásokhoz az API PFX tanúsítványfájlokat használ a dokumentumok jelszóval védett privát és nyilvános kulccsal történő aláírására. A digitális aláírások használhatók üzleti dokumentumok hitelesítésére az eSign PDF adott oldallal, teljes Microsoft Office dokumentumok, például Words, Excel, Powerpoint fájlok és Open Office dokumentumok hitelesítésére. Az ügyfelek könnyen módosíthatják az aláírásokat, például szerkeszthetik, eltávolíthatják vagy módosíthatják. Az API lehetőséget biztosít az aláírások keresésére és ellenőrzésére. Ezenkívül számos lehetőség áll rendelkezésre az aláírások testreszabásához.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "A Doc aláírásának lépései a Digital segítségével a Java programban"
    content_left: |
        A [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) lehetővé teszi a Doc dokumentumok gyors és egyszerű aláírását Digital aláírással.
        
        * Hozzon létre egy példányt a Signature osztályból, amely Doc fájlt tartalmaz, amelyet elérési útként vagy memóriafolyamként kell aláírni
        * Példányosítsa a SignOptions osztályt, és állítsa be az összes kért adatot.
        * Hívja meg a Signature.Sign() metódust, amely átadja a kimeneti Doc fájlt vagy memóriafolyamot

    title_right: " rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for Java minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Szerezze meg a legújabb GroupDocs.Signature for Java terméket a következőtől: [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";
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

        // sign Doc document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Doc dokumentumok aláírása Digital élő bemutatóval"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhelyen azonnal írjon alá Doc fájlt különféle aláírásokkal. Ingyenes online demo vár rád.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Egyéb támogatott Digital aláírások a Java számára"
    content: |
        "A Doc más aláírástípusokkal is aláírható. Kérjük, tekintse meg az alábbi listát."
    format: 
       
       
back_to_top:
    enable: true
---