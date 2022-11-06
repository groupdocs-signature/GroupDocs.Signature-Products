---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Xlsx
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xlsx for C#

############################# Head ############################
head_title: "Odstraňte podpisy Text ze souborů Xlsx prostřednictvím C#"
head_description: "Odstranění konkrétních podpisů Text z podepsaných dokumentů Xlsx lze snadno provést pomocí krátkého kódu .NET."

############################# Header ############################
title: "Odstraňte Text podpisy, které jsou umístěny v souborech Xlsx"
description: "Odstraňte různé podpisy Text z dokumentů Xlsx. Odstranění podpisů Text vyžaduje jednoduchý kód C#."
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
    title_left: "Jak odstranit podpisy Text z vašeho dokumentu Xlsx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje užitečnou funkci pro vymazání Xlsx dokumentů od Text podpisů pomocí několika řádků kódu.
        
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
                
        // Set up input Xlsx file
        string filePath = "input.xlsx";

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
    title: "Podepisování pomocí Text podpisů Živá ukázka"
    content: |
       Přidejte různé elektronické podpisy do souboru Xlsx právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Odstraňte své podpisy Text pomocí C#"
    content: |
        "Smazání elektronických podpisů, které byly přidány do různých formátů dokumentů. Odstraňte podpisy rychle bez dalšího kódu."
    format: 
       
       
back_to_top:
    enable: true
---