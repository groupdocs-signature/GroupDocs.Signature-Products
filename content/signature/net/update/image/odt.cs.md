---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Odt
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Odt for C#

############################# Head ############################
head_title: "Aktualizujte podpisy Image umístěné v souborech Odt pomocí C#"
head_description: "Použijte jednoduchý a snadno pochopitelný kód .NET pro aktualizaci podpisů Image v podepsaných dokumentech Odt."

############################# Header ############################
title: "Upravte a aktualizujte podpisy Image umístěné v souborech Odt"
description: "API pro .NET poskytuje funkce pro aktualizaci podpisů Image v dokumentech Odt. Aktualizujte elektronické podpisy ve svých dokumentech Odt pomocí několika řádků kódu C# rychle a snadno."
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
    title: "Přečtěte si o funkcích API služby GroupDocs.Signature for .NET"
    content: |
        Funkce API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) obsahuje široký výběr prostředků pro zpracování dokumentů ve formátech poptávky pomocí elektronických podpisů. Je podporováno široké spektrum elektronických podpisů, jako jsou texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Zákazníci mohou přidávat, odstraňovat, upravovat, ověřovat nebo prohledávat digitální podpisy v souborech PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých formátech obrázků. K dispozici je řada užitečných funkcí a nastavení.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak změnit podpisy Image ve vašem dokumentu Odt"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) obsahuje užitečné funkce, jako je aktualizace podpisů Image umístěných v dokumentech Odt. Umožňuje měnit vlastnosti podpisů bez dalšího kódu.
        
        * Začněte tím, že vytvoříte objekt Signature, který bude předán jako cesta parametru konstruktoru k dokumentu, který má být aktualizován.
        * Poté vytvořte instanci příslušného konkrétního objektu podpisu a nastavte jeho identifikátor a vlastnosti, které je třeba změnit.
        * Nakonec zavolejte metodu Signature's Update předáním konkrétního objektu podpisu.
        * Zpracujte aktualizaci výsledků k vašemu upozornění.

    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte ve svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Stáhněte si nejnovější verzi GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Aktualizace podpisů Image na stránkách dokumentu - Živá ukázka"
    content: |
       Upravte různé elektronické podpisy dokumentu Odt právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aktualizujte různé podpisy Image prostřednictvím C#"
    content: |
        "Úpravy digitálních podpisů, které jsou umístěny v různých formátech dokumentů. Aktualizujte data podpisů bez dalšího kódu."
    format: 
       
       
back_to_top:
    enable: true
---