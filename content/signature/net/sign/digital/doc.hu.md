---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: hu
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "Digitális elektronikus aláírás hozzáadása a Doc fájlhoz a C# segítségével"
head_description: "Helyezze el a digitális aláírást a .NET Doc fájljába néhány sor kód használatával. A GroupDocs Document Signature API segítségével több tucat fájlformátumot írhat alá."

############################# Header ############################
title: "eSign Doc fájlok Digital aláírással a C# nyelven"
description: "Digital aláírás hozzáadása néhány soros .NET kóddal"
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
    title: "A GroupDocs.Signature for .NET digitális aláírás API-ról"
    content: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) egy népszerű API dokumentumok digitális elektronikus aláírással és digitális tanúsítványokkal történő aláírására. A digitális aláírásokhoz az API PFX tanúsítványfájlokat használ a dokumentumok jelszóval védett privát és nyilvános kulccsal történő aláírására. A digitális aláírások használhatók üzleti dokumentumok hitelesítésére az eSign PDF adott oldallal, teljes Microsoft Office dokumentumok, például Words, Excel, Powerpoint fájlok és Open Office dokumentumok hitelesítésére. Az ügyfelek könnyen módosíthatják az aláírásokat, például szerkeszthetik, eltávolíthatják vagy módosíthatják. Az API lehetőséget biztosít az aláírások keresésére és ellenőrzésére. Ezenkívül számos lehetőség áll rendelkezésre az aláírások testreszabásához.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "A Doc aláírásának lépései a Digital segítségével a C# programban"
    content_left: |
        A [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) lehetővé teszi a Doc dokumentumok gyors és egyszerű aláírását Digital aláírással.
        
        * Hozzon létre egy példányt a Signature osztályból, amely Doc fájlt tartalmaz, amelyet elérési útként vagy memóriafolyamként kell aláírni
        * Példányosítsa a SignOptions osztályt, és állítsa be az összes kért adatot.
        * Hívja meg a Signature.Sign() metódust, amely átadja a kimeneti Doc fájlt vagy memóriafolyamot

    title_right: " rendszerkövetelmények"
    content_right: |
        A GroupDocs.Signature for .NET minden nagyobb platformon és operációs rendszeren támogatott. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.

        * Operációs rendszerek: Microsoft Windows, Linux, MacOS
        * Fejlesztői környezetek: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Szerezze meg a legújabb GroupDocs.Signature for .NET terméket a következőtől: [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

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
    title: "Egyéb támogatott Digital aláírások a C# számára"
    content: |
        "A Doc más aláírástípusokkal is aláírható. Kérjük, tekintse meg az alábbi listát."
    format: 
       
       
back_to_top:
    enable: true
---