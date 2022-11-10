---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Postnet
fileformat: Pdf
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pdf for C#

############################# Head ############################
head_title: "Dokument eSign Pdf s čárovým kódem Postnet v C#"
head_description: "Vytvořte podpis čárového kódu Postnet a vložte jej do dokumentu Pdf s .NET pomocí několika řádků kódu. K podepisování různých formátů souborů použijte rozhraní GroupDocs Document Signature API."

############################# Header ############################
title: "Vygenerujte podpis čárového kódu Postnet pro dokument Pdf v C#"
description: "ePodepište své obchodní dokumenty ve formátu Pdf pomocí čárového kódu Postnet. Vygenerujte podpis čárového kódu rychle a snadno pomocí několika řádků kódu pro nastavení možností podepisování."
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
    title: "O rozhraní API pro podpisy čárových kódů GroupDocs.Signature for .NET."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je rychlé a snadné rozhraní API pro správu elektronického podepisování digitálních dokumentů pomocí typů čárových kódů, jako jsou UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 a mnoho dalších. Zákazníci mohou snadno vytvářet čárové kódy poskytující požadovaný text a vkládat je do PDF, dokumentů Microsoft Office Words, sešitů Microsoft Office Excel, prezentací MS PowerPoint, souborů Adobe Photoshop a různých obrazových formátů. Čárové kódy umístěné v dokumentech lze aktualizovat, vyhledávat, ověřovat, mazat nebo zobrazovat náhled. Navíc je podporováno přizpůsobení čárových kódů.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky k podepsání Pdf pomocí Barcode v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) umožňuje rychle a snadno podepisovat dokumenty Pdf pomocí podpisů Barcode.
        
        * Vytvořte instanci třídy Signature poskytující soubor Pdf, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Pdf nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získejte nejnovější GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pdf file
        string filePath = "input.pdf";
        // Set up output file
        string outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Postnet,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Pdf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Pdf pomocí živé ukázky Barcode"
    content: |
       Podepište soubor Pdf pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Postnet Barcode"
          content: |
            POSTNET (Postal Numeric Encoding Technique) je symbolika čárového kódu, kterou používá poštovní služba Spojených států pro pomoc při směrování pošty.
          characterset: |
             Číslice (0-9).
          textcapacity: |
             Až 11 znaků.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAACcAAAAjCAYAAAAXMhMjAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACeSURBVFhH7c7BCkMxEELR/P9Pp1LoRrCXpi4Cbw5kIRKZtS82x52a407Ncae+HrfWer8Pyr+i/3NcQv/nuIT+z3EJ/X/Ocf9mlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2ubnAHHdqjjt18XF7vwDevzbHqsQWPwAAAABJRU5ErkJggg==

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Barcode pro C#"
    content: |
        "Můžete také podepsat Pdf pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
        
       
back_to_top:
    enable: true
---