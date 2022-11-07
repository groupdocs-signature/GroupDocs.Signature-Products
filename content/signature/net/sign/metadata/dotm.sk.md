---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Dotm
productName: .NET
lang: sk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Dotm for C#

############################# Head ############################
head_title: "Pripojte elektronické podpisy metadát k dokumentom Dotm cez C#"
head_description: "Použite metadáta ako skryté elektronické podpisy vo svojich dokumentoch Dotm pomocou niekoľkých riadkov kódu C#. Použite rozhranie GroupDocs Document Signature API na elektronické podpisovanie obchodných dokumentov a súborov pomocou informácií o metadátach."

############################# Header ############################
title: "Elektronické podpisy metadát pre dokument Dotm prostredníctvom .NET sú jednoduché a ľahko sa používajú!"
description: "ePodpíšte svoje dokumenty a zmluvy Dotm so skrytými položkami metadát. Vytvárajte metadáta pre súbory PDF, dokumenty MS Word, zošity MS Excel, prezentácie MS PowerPoint a rôzne obrazové formáty bez problémov a navyše s kódovaním."
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
    title: "O rozhraní API pre podpisy metadát GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je obľúbené rozhranie API na elektronické podpisovanie digitálnych dokumentov. K dispozícii sú podpisy ako texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Podpisy možno umiestniť do súborov PDF, dokumentov MS Word, zošitov MS Excel, prezentácií MS PowerPoint, súborov Adobe Photoshop a rôznych formátov obrázkov. Zákazníci môžu podpísať svoj dokument a aktualizovať, vyhľadávať, overovať, mazať alebo zobrazovať elektronické podpisy, ktoré boli vložené do týchto dokumentov. Okrem toho je k dispozícii veľa možností na prispôsobenie podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky na podpísanie Dotm pomocou Metadata v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje možnosť rýchlo a jednoducho podpisovať dokumenty Dotm pomocou podpisov Metadata.
        
        * Vytvorte inštanciu triedy Signature poskytujúcej súbor Dotm, ktorý sa má podpisovať ako cesta alebo prúd pamäte
        * Instanciujte triedu SignOptions a nastavte všetky požadované údaje.
        * Vyvolajte metódu Signature.Sign() odovzdajúc výstupný súbor Dotm alebo prúd pamäte

    title_right: " Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získajte najnovší GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotm file
        string filePath = "input.dotm";
        // Set up output file
        string outputFilePath = "output.dotm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Dotm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanie dokumentov Dotm pomocou živej ukážky Metadata"
    content: |
       Podpíšte súbor Dotm pomocou rôznych podpisov práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čaká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ďalšie podporované podpisy Metadata pre C#"
    content: |
        "Dotm môžete podpísať aj inými typmi podpisov. Pozrite si zoznam nižšie."
    format: 
       
       
back_to_top:
    enable: true
---