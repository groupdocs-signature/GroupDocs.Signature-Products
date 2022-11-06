---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Otp
productName: .NET
lang: hu
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Otp for C#

############################# Head ############################
head_title: "Metaadat elektronikus aláírások csatolása a Otp dokumentumokhoz a C# segítségével"
head_description: "Használja a metaadatokat rejtett elektronikus aláírásként a Otp dokumentumaiban néhány soros C# kód használatával. A GroupDocs Document Signature API használatával elektronikusan aláírhatja üzleti dokumentumait és fájljait metaadat-információkkal."

############################# Header ############################
title: "A Otp dokumentum metaadat-elektronikus aláírása a .NET-on keresztül egyszerű és könnyen használható!"
description: "eAláírja Otp dokumentumait és szerződéseit rejtett metaadat-bejegyzésekkel. Metaadatok generálása PDF-ekhez, MS Word dokumentumokhoz, MS Excel munkafüzetekhez, MS PowerPoint prezentációkhoz és különféle képformátumokhoz probléma és extra kódolás nélkül."
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
    title_left: "A {{Fájlformátum}} aláírásának lépései a Metadata segítségével a C# programban"
    content_left: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) lehetővé teszi a Otp dokumentumok gyors és egyszerű aláírását Metadata aláírással.
        
        * Hozzon létre egy példányt a Signature osztályból, amely {{Fájlformátum}} fájlt tartalmaz, amelyet elérési útként vagy memóriafolyamként kell aláírni
        * Példányosítsa a SignOptions osztályt, és állítsa be az összes kért adatot.
        * Hívja meg a Signature.Sign() metódust, amely átadja a kimeneti {{Fájlformátum}} fájlt vagy memóriafolyamot

    title_right: " rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for .NET minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Szerezze meg a legújabb GroupDocs.Signature for .NET terméket a következőtől: [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Otp file
        string filePath = "input.otp";
        // Set up output file
        string outputFilePath = "output.otp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Otp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Otp dokumentumok aláírása Metadata élő bemutatóval"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhelyen azonnal írjon alá Otp fájlt különféle aláírásokkal. Ingyenes online demo vár rád.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Egyéb támogatott Metadata aláírások a C# számára"
    content: |
        "A {{Fájlformátum}} más aláírástípusokkal is aláírható. Kérjük, tekintse meg az alábbi listát."
    format: 
       
       
back_to_top:
    enable: true
---