---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Xltx
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xltx for C#

############################# Head ############################
head_title: "Odstraňte podpisy Image ze souborů Xltx prostřednictvím C#"
head_description: "Odstranění konkrétních podpisů Image z podepsaných dokumentů Xltx lze snadno provést pomocí krátkého kódu .NET."

############################# Header ############################
title: "Odstraňte Image podpisy, které jsou umístěny v souborech Xltx"
description: "Odstraňte různé podpisy Image z dokumentů Xltx. Odstranění podpisů Image vyžaduje jednoduchý kód C#."
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
    title: "Získejte informace o GroupDocs.Signature for .NET funkcích API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API poskytuje mnoho způsobů, jak zpracovávat vaše dokumenty pomocí elektronických podpisů. K dispozici jsou digitální podpisy, jako jsou texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Zákazníci mají možnost přidávat, mazat, aktualizovat, ověřovat nebo vyhledávat digitální podpisy v PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých obrazových formátech. K dispozici je velké množství užitečných funkcí a nastavení.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak odstranit podpisy Image z vašeho dokumentu Xltx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje užitečnou funkci pro vymazání Xltx dokumentů od Image podpisů pomocí několika řádků kódu.
        
        * Nejprve vytvořte instanci předávací cesty objektu Signature do vašeho dokumentu jako parametr konstruktoru.
        * Poté vytvořte vhodný objekt podpisu a nastavte jeho jedinečný identifikátor.
        * Poté vyvolejte metodu Delete předáním objektu podpisu, který musí být smazán.
        * Nakonec výsledky operace procesu.

    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte ve svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Stáhněte si nejnovější verzi GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltx file
        string filePath = "input.xltx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

                // provide signature features to delete
                // set up particular signature id
                ImageSignature signatureToDelete = new ImageSignature(id);

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
    title: "Podepisování pomocí Image podpisů Živá ukázka"
    content: |
       Přidejte různé elektronické podpisy do souboru Xltx právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Odstraňte své podpisy Image pomocí C#"
    content: |
        "Smazání elektronických podpisů, které byly přidány do různých formátů dokumentů. Odstraňte podpisy rychle bez dalšího kódu."
    format: 
       
       
back_to_top:
    enable: true
---