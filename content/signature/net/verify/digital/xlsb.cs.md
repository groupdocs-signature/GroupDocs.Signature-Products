---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Xlsb
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsb for C#

############################# Head ############################
head_title: "Ověření podpisů Digital pro soubory Xlsb prostřednictvím C#"
head_description: "Použijte pouze několik řádků kódu .NET k ověření dokumentů Xlsb a jejich podpisů Digital."

############################# Header ############################
title: "Ověření podpisů Digital pro soubory Xlsb"
description: "API pro .NET poskytuje příležitost ověřit podpisy Digital v dokumentech Xlsb. Ověření elektronických podpisů ve vašich dokumentech Xlsb může být provedeno rychle a snadno."
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
    title: "Objevte nové funkce API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API poskytuje širokou škálu způsobů zpracování mnoha formátů dokumentů pomocí elektronických podpisů. Je podporováno mnoho typů digitálních podpisů, jako jsou texty, obrázky, digitální certifikáty, čárové kódy, QR kódy, razítka nebo metadata. Zákazníci mohou přidávat, odstraňovat, upravovat, ověřovat nebo prohledávat digitální podpisy v souborech PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých formátech obrázků. K dispozici je úžasný počet dalších funkcí a nastavení.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak ověřit podpisy Digital ve vašem dokumentu Xlsb"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) obsahuje užitečné funkce, jako je ověřování podpisů Digital umístěných v dokumentech Xlsb. Využijte tuto příležitost bez implementace dalšího kódu.
        
        * Nejprve vytvořte instanci třídy Signature poskytující jako parametr konstruktoru cestu k dokumentu, který má být ověřen.
        * Za druhé, vytvořte nový objekt VerifyOptions a nastavte všechny požadované vlastnosti.
        * Nakonec vyvolejte metodu Verify objektu Signature předávající instanci VerifyOptions.
        * Poté zpracujte výsledky ověření.

    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte ve svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Stáhněte si nejnovější verzi GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování pomocí Digital podpisů Živá ukázka"
    content: |
       Přidejte různé elektronické podpisy do souboru Xlsb právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ověřte další podpisy Digital pomocí C#"
    content: |
        "Ověřování elektronických podpisů umístěných v různých dokumentech. Zkontrolujte kvalitu podpisů v oblíbených formátech souborů, jak je uvedeno níže."
    format: 
       
       
back_to_top:
    enable: true
---