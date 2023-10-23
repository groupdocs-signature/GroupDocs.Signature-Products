---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Tar
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Tar for C#

############################# Head ############################
head_title: "Přidání digitálních elektronických podpisů do souboru Tar pomocí C#"
head_description: "Vložte digitální podpis do souboru Tar pro .NET pomocí několika řádků kódu. Pomocí rozhraní GroupDocs Document Signature API podepisujte desítky formátů souborů."

############################# Header ############################
title: "Soubory eSign Tar s podpisy Digital v C#"
description: "Jak přidat podpis Digital pomocí několika řádků kódu .NET"
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
    title: "O GroupDocs.Signature for .NET rozhraní API pro digitální podpisy"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je populární API pro podepisování dokumentů pomocí digitálních elektronických podpisů a digitálních certifikátů. Pro rozhraní API pro digitální podpisy používá soubory certifikátů PFX k podpisu dokumentu pomocí soukromých a veřejných klíčů chráněných heslem. Digitální podpisy lze použít k certifikaci obchodních dokumentů s konkrétní stránkou eSign PDF, k certifikaci celých dokumentů Microsoft Office, jako jsou Words, Excel, soubory Powerpoint a dokumenty Open Office. Zákazníci mohou s podpisy snadno manipulovat, například je upravovat, odstraňovat nebo upravovat. API poskytuje způsob, jak vyhledávat a ověřovat podpisy. Navíc je k dispozici mnoho schopností pro přizpůsobení podpisů.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky k podepsání Tar pomocí Digital v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) umožňuje rychle a snadno podepisovat dokumenty Tar pomocí podpisů Digital.
        
        * Vytvořte instanci třídy Signature poskytující soubor Tar, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Tar nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získejte nejnovější GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Tar file
        string filePath = "input.tar";
        // Set up output file
        string outputFilePath = "output.tar";
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

                // sign Tar document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Tar pomocí živé ukázky Digital"
    content: |
       Podepište soubor Tar pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Digital pro C#"
    content: |
        "Můžete také podepsat Tar pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
       
       
back_to_top:
    enable: true
---