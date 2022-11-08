---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ods
productName: .NET
lang: hu
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ods for C#

############################# Head ############################
head_title: "Metaadat elektronikus aláírások csatolása a Ods dokumentumokhoz a C# segítségével"
head_description: "Használja a metaadatokat rejtett elektronikus aláírásként a Ods dokumentumaiban néhány soros C# kód használatával. A GroupDocs Document Signature API használatával elektronikusan aláírhatja üzleti dokumentumait és fájljait metaadat-információkkal."

############################# Header ############################
title: "A Ods dokumentum metaadat-elektronikus aláírása a .NET-on keresztül egyszerű és könnyen használható!"
description: "eAláírja Ods dokumentumait és szerződéseit rejtett metaadat-bejegyzésekkel. Metaadatok generálása PDF-ekhez, MS Word dokumentumokhoz, MS Excel munkafüzetekhez, MS PowerPoint prezentációkhoz és különféle képformátumokhoz probléma és extra kódolás nélkül."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "A GroupDocs.Signature for .NET metaadat-aláírások API-járól"
    content: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) egy népszerű API a digitális dokumentumok elektronikus aláírására. Aláírások, például szövegek, képek, digitális tanúsítványok, vonalkódok, QR-kódok, bélyegzők vagy metaadatok állnak rendelkezésre. Az aláírások elhelyezhetők PDF-eken, MS Word dokumentumokon, MS Excel munkafüzeteken, MS PowerPoint prezentációkban, Adobe Photoshop fájlokon és különféle képformátumokban. Az ügyfelek aláírhatják dokumentumaikat, és frissíthetik, kereshetik, ellenőrizhetik, törölhetik vagy megtekinthetik a dokumentumokon elhelyezett e-aláírásokat. Ezenkívül számos lehetőség áll rendelkezésre az aláírások testreszabásához.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "A Ods aláírásának lépései a Metadata segítségével a C# programban"
    content_left: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) lehetővé teszi a Ods dokumentumok gyors és egyszerű aláírását Metadata aláírással.
        
        * Hozzon létre egy példányt a Signature osztályból, amely Ods fájlt tartalmaz, amelyet elérési útként vagy memóriafolyamként kell aláírni
        * Példányosítsa a SignOptions osztályt, és állítsa be az összes kért adatot.
        * Hívja meg a Signature.Sign() metódust, amely átadja a kimeneti Ods fájlt vagy memóriafolyamot

    title_right: " rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for .NET minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Szerezze meg a legújabb GroupDocs.Signature for .NET terméket a következőtől: [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ods dokumentumok aláírása Metadata élő bemutatóval"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhelyen azonnal írjon alá Ods fájlt különféle aláírásokkal. Ingyenes online demo vár rád.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Egyéb támogatott Metadata aláírások a C# számára"
    content: |
        "A Ods más aláírástípusokkal is aláírható. Kérjük, tekintse meg az alábbi listát."
    format: 
       
       
back_to_top:
    enable: true
---