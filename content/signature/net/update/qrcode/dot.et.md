---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Qrcode
fileformat: Dot
productName: .NET
lang: et
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Dot for C#

############################# Head ############################
head_title: "Värskendage Qrcode allkirja, mis on pandud failidesse Dot rakendusega C#"
head_description: "Kasutage allkirjastatud Dot dokumentides allkirjade Qrcode värskendamiseks lihtsat ja hõlpsasti mõistetavat .NET koodi."

############################# Header ############################
title: "Muutke ja värskendage failidesse Dot pandud allkirju Qrcode"
description: "API for .NET pakub funktsiooni Qrcode allkirjade värskendamiseks dokumentides Dot. Värskendage oma Dot dokumentides olevaid e-allkirju paari rea koodiga C# kiiresti ja lihtsalt."
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
    title_left: "Kuidas muuta allkirja Qrcode oma dokumendis Dot"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) sisaldab kasulikke funktsioone, nagu Qrcode allkirjade värskendamine, mis on paigutatud dokumentidele Dot. See võimaldab muuta allkirjafunktsioone ilma lisakoodita.
        
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
                
        // Set up input Dot file
        string filePath = "input.dot";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to update
                // set up particular signature id
                QrCodeSignature signatureToUpdate = new QrCodeSignature(id)
                {
                    // specify signature width
                    Width = 200,
                    // specify signature height
                    Height = 200,
                    // set left position
                    Left = 120,
                    // set top position
                    Top = 160
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
    title: "Allkirjade Qrcode värskendamine dokumendilehtedel – reaalajas demo"
    content: |
       Saate kohe redigeerida dokumendi Dot erinevaid elektroonilisi allkirju, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Värskendage Qrcode allkirju C# kaudu"
    content: |
        "Erinevatesse dokumendivormingutesse paigutatud digitaalallkirjade redigeerimine. Uuendage allkirjaandmeid ilma lisakoodita."
    format: 
       
       
back_to_top:
    enable: true
---