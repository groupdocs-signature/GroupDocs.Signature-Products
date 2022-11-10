---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Bmp
productName: .NET
lang: sk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Bmp for C#

############################# Head ############################
head_title: "Pridanie podpisov Image do súboru Bmp pomocou C#"
head_description: "Vložte podpis Image do súboru Bmp pre .NET pomocou niekoľkých riadkov kódu. Použite rozhranie GroupDocs Document Signature API na podpisovanie desiatok formátov súborov."

############################# Header ############################
title: "Podpíšte súbory Bmp pomocou podpisov Image v C#"
description: "Ako pridať podpis Image pomocou niekoľkých riadkov kódu .NET"
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
    title: "O rozhraní API pre podpisy obrázkov GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je obľúbené rozhranie API na elektronické podpisovanie digitálnych dokumentov. K dispozícii sú podpisy ako texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Podpisy možno umiestniť do súborov PDF, dokumentov MS Word, zošitov MS Excel, prezentácií MS PowerPoint, súborov Adobe Photoshop a rôznych formátov obrázkov. Zákazníci môžu podpísať svoj dokument a aktualizovať, vyhľadávať, overovať, mazať alebo zobrazovať elektronické podpisy, ktoré boli vložené do týchto dokumentov. Okrem toho je k dispozícii veľa možností na prispôsobenie podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky na podpísanie Bmp pomocou Image v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje možnosť rýchlo a jednoducho podpisovať dokumenty Bmp pomocou podpisov Image.
        
        * Vytvorte inštanciu triedy Signature poskytujúcej súbor Bmp, ktorý sa má podpisovať ako cesta alebo prúd pamäte
        * Instanciujte triedu SignOptions a nastavte všetky požadované údaje.
        * Vyvolajte metódu Signature.Sign() odovzdajúc výstupný súbor Bmp alebo prúd pamäte

    title_right: " Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získajte najnovší GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Bmp file
        string filePath = "input.bmp";
        // Set up output file
        string outputFilePath = "output.bmp";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Bmp document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanie dokumentov Bmp pomocou živej ukážky Image"
    content: |
       Podpíšte súbor Bmp pomocou rôznych podpisov práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čaká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ďalšie podporované podpisy Image pre C#"
    content: |
        "Bmp môžete podpísať aj inými typmi podpisov. Pozrite si zoznam nižšie."
    format: 
       
       
back_to_top:
    enable: true
---