---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Doc
productName: .NET
lang: sk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Doc for C#

############################# Head ############################
head_title: "Vytvorte textové elektronické podpisy do súboru Doc pomocou C#"
head_description: "Vložte elektronický podpis Text do súboru Doc pre .NET pomocou niekoľkých riadkov kódu. Použite rozhranie GroupDocs Document Signature API na podpisovanie desiatok formátov súborov."

############################# Header ############################
title: "Podpíšte súbory Doc pomocou podpisov Text v C#"
description: "Ako pridať podpis Text pomocou niekoľkých riadkov kódu .NET"
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
    title: "O GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je obľúbené rozhranie API na elektronické podpisovanie digitálnych dokumentov. K dispozícii sú podpisy ako texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Podpisy možno umiestniť do súborov PDF, dokumentov MS Word, zošitov MS Excel, prezentácií MS PowerPoint, súborov Adobe Photoshop a rôznych formátov obrázkov. Zákazníci môžu podpísať svoj dokument a aktualizovať, vyhľadávať, overovať, mazať alebo zobrazovať elektronické podpisy, ktoré boli vložené do týchto dokumentov. Okrem toho je k dispozícii veľa možností na prispôsobenie podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky na podpísanie Doc pomocou Text v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje možnosť rýchlo a jednoducho podpisovať dokumenty Doc pomocou podpisov Text.
        
        * Vytvorte inštanciu triedy Signature poskytujúcej súbor Doc, ktorý sa má podpisovať ako cesta alebo prúd pamäte
        * Instanciujte triedu SignOptions a nastavte všetky požadované údaje.
        * Vyvolajte metódu Signature.Sign() odovzdajúc výstupný súbor Doc alebo prúd pamäte

    title_right: " Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získajte najnovší GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
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
    title: "Podpisovanie dokumentov Doc pomocou živej ukážky Text"
    content: |
       Podpíšte súbor Doc pomocou rôznych podpisov práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čaká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ďalšie podporované podpisy Text pre C#"
    content: |
        "Doc môžete podpísať aj inými typmi podpisov. Pozrite si zoznam nižšie."
    format: 
       
       
back_to_top:
    enable: true
---