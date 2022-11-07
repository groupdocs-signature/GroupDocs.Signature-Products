---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Potm
productName: .NET
lang: sk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Potm with C#

############################# Head ############################
head_title: "Vyhľadajte podpisy Text v súbore Potm v C#"
head_description: "Použite .NET na vyhľadávanie Text podpisov v súboroch Potm pomocou niekoľkých riadkov kódu."

############################# Header ############################
title: "Vyhľadajte podpisy Text v súbore Potm"
description: "Natívne API .NET umožňuje vyhľadávať podpisy Text v už podpísaných súboroch Potm. Vykonajte rozšírené vyhľadávanie elektronických podpisov vo svojich dokumentoch Potm pomocou niekoľkých riadkov kódu."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) poskytuje .NET API na spracovanie dokumentov pomocou rôznych typov podpisov, ako sú texty, obrázky, digitálne certifikáty, čiarové kódy, QR kódy, pečiatky alebo metadáta. Používatelia môžu pridávať, mazať, aktualizovať, overovať alebo vyhľadávať elektronické podpisy v súboroch PDF, dokumentoch MS Word, zošitoch MS Excel, prezentáciách MS PowerPoint, súboroch Adobe Photoshop a rôznych obrazových formátoch s ďalšou podporou prispôsobenia vlastností podpisov podľa potreby.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ako vyhľadať podpisy Text v Potm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) uľahčuje vývojárom .NET vyhľadávanie podpisov Text v súboroch Potm z ich aplikácií implementáciou niekoľkých jednoduchých krokov.
        
        * Vytvorte novú inštanciu triedy Signature a odovzdajte cestu zdrojového dokumentu ako parameter konštruktora.
        * Vytvorte inštanciu objektu SearchOptions podľa svojich požiadaviek a zadajte možnosti vyhľadávania.
        * Zavolajte metódu vyhľadávania inštancie triedy Signature a odovzdajte jej SearchOptions.
        * Spracujte výsledky vyhľadávania podľa vašich požiadaviek.

    title_right: "Požiadavky na systém"
    content_right: |
        GroupDocs.Signature for .NET sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.

        * Operačné systémy: Microsoft Windows, Linux, MacOS
        * Vývojové prostredia: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Stiahnite si najnovšiu verziu GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Potm file
        string filePath = "input.potm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Potm document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Vyhľadajte živé ukážky elektronických podpisov Text"
    content: |
       Vyhľadajte v dokumente rôzne elektronické podpisy do súborov Potm práve teraz na webovej lokalite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Vyhľadajte ďalšie podpisy Text pomocou C#"
    content: |
        "Elektronické podpisy vyhľadávajú v rôznych dokumentoch. Nájdite podpisy z jedného z populárnych formátov súborov, ako je uvedené nižšie."
    format: 
           
       
back_to_top:
    enable: true
---