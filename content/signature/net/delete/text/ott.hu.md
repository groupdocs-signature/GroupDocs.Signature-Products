---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Ott
productName: .NET
lang: hu
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Ott for C#

############################# Head ############################
head_title: "Törölje a Text aláírásokat a Ott fájlokból a C# segítségével"
head_description: "Az aláírt Ott dokumentumokból bizonyos Text aláírások törlése egyszerűen végrehajtható rövid .NET kóddal."

############################# Header ############################
title: "Távolítsa el a Text aláírásokat, amelyek a {{Fájlformátum}} fájlokban vannak elhelyezve"
description: "Törölje a különböző Text aláírásokat a {{Fájlformátum}} dokumentumokból. A Text aláírások eltávolításához egyszerű C# kód szükséges."
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
    title: "Tájékozódjon a GroupDocs.Signature for .NET API funkcióiról"
    content: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API számos módot biztosít a dokumentumok elektronikus aláírással történő feldolgozására. Digitális aláírások, például szövegek, képek, digitális tanúsítványok, vonalkódok, QR-kódok, bélyegzők vagy metaadatok állnak rendelkezésre. Az ügyfeleknek lehetőségük van digitális aláírások hozzáadására, törlésére, frissítésére, ellenőrzésére vagy keresésére PDF-ekben, MS Word dokumentumokban, MS Excel munkafüzetekben, MS PowerPoint prezentációkban, Adobe Photoshop fájlokban és különféle képformátumokban. Számos hasznos funkció és beállítás érhető el.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hogyan távolíthatja el a Text aláírásokat a Ott dokumentumból"
    content_left: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) hasznos funkciót biztosít a Ott dokumentumok Text aláírásainak néhány soros kóddal történő törléséhez.
        
        * Először is, példányosítsa az Signature objektumot, amely konstruktor paraméterként adja át a dokumentum elérési útját.
        * Ezután hozzon létre egy megfelelő aláírási objektumot, és állítsa be annak egyedi azonosítóját.
        * Ezt követően hívja meg a Delete metódust, amely átadja az aláírási objektumot, amelyet törölni kell.
        * Végül a folyamat működési eredményei.

    title_right: "rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for .NET minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Töltse le a(z) GroupDocs.Signature for .NET legújabb verzióját innen: [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ott file
        string filePath = "input.ott";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Aláírás Text aláírásokkal Élő bemutató"
    content: |
       A [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webhely meglátogatásával azonnal adjon hozzá különféle elektronikus aláírásokat a Ott fájlhoz.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Törölje Text aláírásait a C# segítségével"
    content: |
        "A különböző dokumentumformátumokhoz hozzáadott e-aláírások törlése. Az aláírások gyors eltávolítása extra kód nélkül."
    format: 
       
       
back_to_top:
    enable: true
---