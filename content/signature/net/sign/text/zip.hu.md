---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Zip
productName: .NET
lang: hu
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Zip for C#

############################# Head ############################
head_title: "Szöveges elektronikus aláírások létrehozása a Zip fájlhoz a C# segítségével"
head_description: "Helyezze a Text eSignature-t a .NET Zip fájljába néhány sor kóddal. A GroupDocs Document Signature API segítségével több tucat fájlformátumot írhat alá."

############################# Header ############################
title: "Zip fájl aláírása Text aláírással a C# alkalmazásban"
description: "Text aláírás hozzáadása néhány soros .NET kóddal"
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
    title: "A GroupDocs.Signature for .NET API-ról"
    content: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) egy népszerű API a digitális dokumentumok elektronikus aláírására. Aláírások, például szövegek, képek, digitális tanúsítványok, vonalkódok, QR-kódok, bélyegzők vagy metaadatok állnak rendelkezésre. Az aláírások elhelyezhetők PDF-eken, MS Word dokumentumokon, MS Excel munkafüzeteken, MS PowerPoint prezentációkban, Adobe Photoshop fájlokon és különféle képformátumokban. Az ügyfelek aláírhatják dokumentumaikat, és frissíthetik, kereshetik, ellenőrizhetik, törölhetik vagy megtekinthetik a dokumentumokon elhelyezett e-aláírásokat. Ezenkívül számos lehetőség áll rendelkezésre az aláírások testreszabásához.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "A Zip aláírásának lépései a Text segítségével a C# programban"
    content_left: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) lehetővé teszi a Zip dokumentumok gyors és egyszerű aláírását Text aláírással.
        
        * Hozzon létre egy példányt a Signature osztályból, amely Zip fájlt tartalmaz, amelyet elérési útként vagy memóriafolyamként kell aláírni
        * Példányosítsa a SignOptions osztályt, és állítsa be az összes kért adatot.
        * Hívja meg a Signature.Sign() metódust, amely átadja a kimeneti Zip fájlt vagy memóriafolyamot

    title_right: " rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for .NET minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Szerezze meg a legújabb GroupDocs.Signature for .NET terméket a következőtől: [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Zip file
        string filePath = "input.zip";
        // Set up output file
        string outputFilePath = "output.zip";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Zip document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Zip dokumentumok aláírása Text élő bemutatóval"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhelyen azonnal írjon alá Zip fájlt különféle aláírásokkal. Ingyenes online demo vár rád.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Egyéb támogatott Text aláírások a C# számára"
    content: |
        "A Zip más aláírástípusokkal is aláírható. Kérjük, tekintse meg az alábbi listát."
    format: 
       
       
back_to_top:
    enable: true
---