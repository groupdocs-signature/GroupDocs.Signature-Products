---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Doc
productName: .NET
lang: hu
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Doc with C#

############################# Head ############################
head_title: "Keressen Image aláírásokat a Doc fájlban a C# programban"
head_description: "A .NET használatával kereshet Image aláírásokat a Doc fájlokban néhány sornyi kód használatával."

############################# Header ############################
title: "Keressen Image aláírásokat a Doc fájlban"
description: "A .NET natív API lehetővé teszi a Image aláírások keresését a már aláírt Doc fájlokban. Végezzen speciális e-aláírás-keresést a Doc dokumentumaiban néhány sornyi kód használatával."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "A GroupDocs.Signature for .NET API-ról"
    content: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) biztosítja a .NET API-t dokumentumok feldolgozásához különböző aláírástípusok, például szövegek, képek, digitális tanúsítványok, vonalkódok, QR-kódok, bélyegzők vagy metaadatok használatával. A felhasználók hozzáadhatnak, törölhetnek, frissíthetnek, ellenőrizhetnek vagy kereshetnek elektronikus aláírásokban PDF-ekben, MS Word-dokumentumokban, MS Excel-munkafüzetekben, MS PowerPoint-prezentációkban, Adobe Photoshop-fájlokban és különféle képformátumokban, az aláírások tulajdonságainak szükség szerinti testreszabásának további támogatásával.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Image aláírások keresése a Doc fájlban"
    content_left: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) néhány egyszerű lépés végrehajtásával megkönnyíti a .NET fejlesztői számára, hogy Image aláírásokat keressenek alkalmazásaik Doc fájljaiban.
        
        * Hozzon létre egy új Signature osztály példányt, és adja meg a forrásdokumentum elérési útját konstruktor paraméterként.
        * Példányosítsa a SearchOptions objektumot igényei szerint, és adja meg a keresési beállításokat.
        * Hívja meg a Signature osztálypéldány keresési metódusát, és adja át neki a SearchOptions-t.
        * A keresési eredményeket az Ön igényei szerint dolgozza fel.

    title_right: "rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for .NET minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Töltse le a(z) GroupDocs.Signature for .NET legújabb verzióját innen: [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Doc document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image elektronikus aláírás keresése Élő bemutató"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhelyen azonnal kereshet a dokumentumban különféle elektronikus aláírásokat Doc fájlokhoz.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Más Image aláírások keresése a C# segítségével"
    content: |
        "Az elektronikus aláírások keresése különböző dokumentumokban. Keresse meg az aláírásokat a népszerű fájlformátumok egyikéből az alábbiak szerint."
    format: 
           
       
back_to_top:
    enable: true
---