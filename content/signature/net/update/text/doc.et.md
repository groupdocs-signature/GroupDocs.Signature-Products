---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Doc
productName: .NET
lang: et
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Doc for C#

############################# Head ############################
head_title: "Värskendage Text allkirja, mis on pandud failidesse Doc rakendusega C#"
head_description: "Kasutage allkirjastatud Doc dokumentides allkirjade Text värskendamiseks lihtsat ja hõlpsasti mõistetavat .NET koodi."

############################# Header ############################
title: "Muutke ja värskendage failidesse Doc pandud allkirju Text"
description: "API for .NET pakub funktsiooni Text allkirjade värskendamiseks dokumentides Doc. Värskendage oma Doc dokumentides olevaid e-allkirju paari rea koodiga C# kiiresti ja lihtsalt."
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
    title: "Lisateave toote GroupDocs.Signature for .NET API funktsioonide kohta"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API-funktsioonid sisaldavad laia valikut vahendeid nõutavate dokumentide vormingute töötlemiseks elektrooniliste allkirjade abil. Toetatud on lai valik e-allkirju, nagu tekstid, pildid, digitaalsed sertifikaadid, vöötkoodid, QR-koodid, templid või metaandmed. Kliendid saavad lisada, eemaldada, redigeerida, kinnitada või otsida digitaalallkirju PDF-ides, MS Wordi dokumentides, MS Exceli töövihikutes, MS PowerPointi esitlustes, Adobe Photoshopi failides ja erinevates pildivormingutes. Saadaval on palju kasulikke funktsioone ja seadeid.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kuidas muuta allkirja Text oma dokumendis Doc"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) sisaldab kasulikke funktsioone, nagu Text allkirjade värskendamine, mis on paigutatud dokumentidele Doc. See võimaldab muuta allkirjafunktsioone ilma lisakoodita.
        
        * Alustuseks looge allkirjaobjekt, mis edastab konstruktori parameetri teena dokumendile, mida peaks värskendama.
        * Seejärel looge sobiv konkreetne allkirjaobjekt ja seadistage selle identifikaator ja atribuudid, mida tuleb muuta.
        * Lõpuks helistage Signature's Update meetodile, edastades konkreetse allkirjaobjekti.
        * Töötlege tulemuste värskendamist teie teate järgi.

    title_right: "Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for .NET toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laadige alla toote GroupDocs.Signature for .NET uusim versioon saidilt [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                TextSignature signatureToUpdate = new TextSignature(id)
                {
                    // specify signature width
                    Width = 130,
                    // specify signature height
                    Height = 20,
                    // set left position
                    Left = 40,
                    // set top position
                    Top = 50,
                    // set up new text
                    Text = "Mr. John Smith"
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
    title: "Allkirjade Text värskendamine dokumendilehtedel – reaalajas demo"
    content: |
       Saate kohe redigeerida dokumendi Doc erinevaid elektroonilisi allkirju, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Värskendage Text allkirju C# kaudu"
    content: |
        "Erinevatesse dokumendivormingutesse paigutatud digitaalallkirjade redigeerimine. Uuendage allkirjaandmeid ilma lisakoodita."
    format: 
       
       
back_to_top:
    enable: true
---