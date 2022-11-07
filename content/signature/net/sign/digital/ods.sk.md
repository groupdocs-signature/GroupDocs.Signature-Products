---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ods
productName: .NET
lang: sk
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ods for C#

############################# Head ############################
head_title: "Pridanie digitálnych elektronických podpisov do súboru Ods pomocou C#"
head_description: "Vložte digitálny podpis do súboru Ods pre .NET pomocou niekoľkých riadkov kódu. Použite rozhranie GroupDocs Document Signature API na podpisovanie desiatok formátov súborov."

############################# Header ############################
title: "eSign Ods súbory s Digital podpismi v C#"
description: "Ako pridať podpis Digital pomocou niekoľkých riadkov kódu .NET"
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
    title: "O GroupDocs.Signature for .NET API pre digitálne podpisy"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je populárne rozhranie API na podpisovanie dokumentov pomocou digitálnych elektronických podpisov a digitálnych certifikátov. Pre rozhranie API pre digitálne podpisy používa súbory certifikátov PFX na esignovanie dokumentu pomocou súkromných a verejných kľúčov chránených heslom. Digitálne podpisy možno použiť na certifikáciu obchodných dokumentov pomocou konkrétnej stránky eSign PDF, certifikáciu celých dokumentov balíka Microsoft Office, ako sú Words, Excel, súbory Powerpoint a dokumenty Open Office. Zákazníci môžu s podpismi jednoducho manipulovať, napríklad ich upravovať, odstraňovať alebo upravovať. Rozhranie API poskytuje spôsob vyhľadávania a overovania podpisov. Okrem toho je k dispozícii veľa možností na prispôsobenie podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroky na podpísanie Ods pomocou Digital v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje možnosť rýchlo a jednoducho podpisovať dokumenty Ods pomocou podpisov Digital.
        
        * Vytvorte inštanciu triedy Signature poskytujúcej súbor Ods, ktorý sa má podpisovať ako cesta alebo prúd pamäte
        * Instanciujte triedu SignOptions a nastavte všetky požadované údaje.
        * Vyvolajte metódu Signature.Sign() odovzdajúc výstupný súbor Ods alebo prúd pamäte

    title_right: " Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Získajte najnovší GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";
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

                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanie dokumentov Ods pomocou živej ukážky Digital"
    content: |
       Podpíšte súbor Ods pomocou rôznych podpisov práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Bezplatné online demo na vás čaká.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ďalšie podporované podpisy Digital pre C#"
    content: |
        "Ods môžete podpísať aj inými typmi podpisov. Pozrite si zoznam nižšie."
    format: 
       
       
back_to_top:
    enable: true
---