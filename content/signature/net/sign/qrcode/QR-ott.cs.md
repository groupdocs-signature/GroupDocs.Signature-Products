---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: QR
fileformat: Ott
productName: .NET
lang: cs
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Ott for C#

############################# Head ############################
head_title: "Dokument eSign Ott s QR QR kódem v C#"
head_description: "Vytvořte QR kód QR a vložte jej do souboru Ott pomocí .NET s krátkým kódem C#. Použijte GroupDocs Document Signature API k elektronickému podepisování obchodních dokumentů a souborů pomocí QR kódu."

############################# Header ############################
title: "Vygenerujte podpis QR QR kódu pro dokument Ott v C#"
description: "ePodepište své dokumenty a smlouvy ve formátu Ott pomocí QR kódu QR. Vygenerujte podpis QR kódu rychle a snadno."
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
    title: "O rozhraní API pro podpisy QR kódu GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je vyspělé rozhraní API pro vytváření a generování podpisů QR kódu pro dokumenty. Uživatelé mohou generovat podpisy QR kódu poskytující text ke stažení nebo sdílení přes sociální média jako obrázek. Podepsaný dokument lze naskenovat pomocí API nebo jednoduše přes mobilní kameru! Podepisujte elektronicky své obchodní smlouvy a úřední dokumenty přidáním podpisu QR kódu a manipulujte s nimi. Jakýkoli podpis QR kódu bude obsahovat jedinečné vlastní informace, které identifikují podepisujícího nebo autorizují dokument. Kromě toho lze obsah QR kódu programově šifrovat a dešifrovat pomocí osobních klíčů. To otevírá mnoho možností pro sdílení citlivých dat uvnitř veřejných dokumentů. Po podpisu může uživatel aktualizovat, ověřovat, mazat, zobrazovat náhled nebo vyhledávat QR kódy v souborech PDF, dokumentech MS Word, sešitech MS Excel, prezentacích MS PowerPoint, souborech Adobe Photoshop a různých formátech obrázků. QR kódy lze dodatečně upravit.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky k podepsání Ott pomocí Qrcode v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) umožňuje rychle a snadno podepisovat dokumenty Ott pomocí podpisů Qrcode.
        
        * Vytvořte instanci třídy Signature poskytující soubor Ott, který se má podepisovat jako cesta nebo proud paměti
        * Instantujte třídu SignOptions a nastavte všechna požadovaná data.
        * Vyvolejte metodu Signature.Sign() předáním výstupního souboru Ott nebo proudu paměti

    title_right: " Požadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.

        * Operační systémy: Microsoft Windows, Linux, MacOS
        * Vývojová prostředí: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získejte nejnovější GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ott file
        string filePath = "input.ott";
        // Set up output file
        string outputFilePath = "output.ott";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.QR,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Ott document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podepisování dokumentů Ott pomocí živé ukázky Qrcode"
    content: |
       Podepište soubor Ott pomocí různých podpisů právě teď na webu [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čeká.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About QR QrCode"
          content: |
            QR Code (zkráceně Quick Response Code) je ochranná známka pro typ maticového čárového kódu (nebo dvourozměrného čárového kódu). Jedná se o nejoblíbenější a nejrozšířenější typ dvourozměrného kódu. V praxi QR kódy často obsahují data pro lokátor, identifikátor nebo tracker, který ukazuje na webovou stránku nebo aplikaci.
          characterset: |
             Všech 256 znaků ASCII + Kanji
          textcapacity: |
             Až 7089 číselných znaků, 4296 alfanumerických znaků, 2953 bajtů (binární data) nebo 1817 znaků Kanji.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Další podporované podpisy Qrcode pro C#"
    content: |
        "Můžete také podepsat Ott pomocí jiných typů podpisů. Podívejte se prosím na níže uvedený seznam."
    format: 
        
       
back_to_top:
    enable: true
---