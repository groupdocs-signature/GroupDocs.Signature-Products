---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Ods
productName: .NET
lang: hu
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ods for C#

############################# Head ############################
head_title: "eSign Ods dokumentum Pharmacode vonalkóddal a C# nyelven"
head_description: "Hozzon létre Pharmacode vonalkód-aláírást, és helyezze el a Ods dokumentumra a .NET termékkel, néhány sor kóddal. Használja a GroupDocs Document Signature API-t különböző fájlformátumok aláírásához."

############################# Header ############################
title: "Pharmacode vonalkód aláírás létrehozása a Ods dokumentumhoz a C# programban"
description: "eAláírja Ods üzleti dokumentumait Pharmacode vonalkóddal. Néhány soros kóddal gyorsan és egyszerűen generálhat vonalkód-aláírást az aláírási lehetőségek beállításához."
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
    title: "A GroupDocs.Signature for .NET Vonalkód aláírások API-ról."
    content: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) egy gyors és egyszerű API digitális dokumentumok elektronikus aláírásának kezelésére olyan vonalkódtípusok használatával, mint az UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 és még sokan mások. Az ügyfelek egyszerűen létrehozhatnak vonalkódokat a szükséges szöveggel, és elhelyezhetik azokat PDF-ben, Microsoft Office Words dokumentumokban, Microsoft Office Excel munkafüzetekben, MS PowerPoint bemutatókban, Adobe Photoshop fájlokban és különféle képformátumokban. A dokumentumokban elhelyezett vonalkódok frissíthetők, kereshetők, ellenőrizhetők, törölhetők vagy megtekinthetők. Ezenkívül a vonalkódok testreszabása támogatott.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "A Ods aláírásának lépései a Barcode segítségével a C# programban"
    content_left: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) lehetővé teszi a Ods dokumentumok gyors és egyszerű aláírását Barcode aláírással.
        
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
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ods dokumentumok aláírása Barcode élő bemutatóval"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhelyen azonnal írjon alá Ods fájlt különféle aláírásokkal. Ingyenes online demo vár rád.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            A Pharmacode, más néven Pharmaceutical Binary Code, egy vonalkód-szabvány, amelyet a gyógyszeriparban csomagolásellenőrző rendszerként használnak.
          characterset: |
             Numerikus számjegyek (0-9).
          textcapacity: |
             Csak egyetlen egész számot jelöl 3 és 131070 között.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Egyéb támogatott Barcode aláírások a C# számára"
    content: |
        "A Ods más aláírástípusokkal is aláírható. Kérjük, tekintse meg az alábbi listát."
    format: 
        
       
back_to_top:
    enable: true
---