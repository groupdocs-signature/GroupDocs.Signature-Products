---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Potx
productName: .NET
lang: et
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Potx for C#

############################# Head ############################
head_title: "Kustutage Text allkirjad failist Potx läbi C#"
head_description: "Konkreetsete Text allkirjade kustutamine allkirjastatud Potx dokumentidest saab hõlpsasti teostada lühikese .NET koodiga."

############################# Header ############################
title: "Eemaldage allkirjad Text, mis on paigutatud failidesse Potx"
description: "Kustutage erinevad allkirjad Text dokumentidest Potx. Allkirjade Text eemaldamine nõuab lihtsat C# koodi."
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
    title: "Hankige teavet toote GroupDocs.Signature for .NET API funktsioonide kohta"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API pakub palju võimalusi dokumentide töötlemiseks elektrooniliste allkirjade abil. Saadaval on digitaalallkirjad, nagu tekstid, pildid, digitaalsed sertifikaadid, vöötkoodid, QR-koodid, templid või metaandmed. Klientidel on võimalus lisada, kustutada, uuendada, kontrollida või otsida digiallkirju PDF-idest, MS Wordi dokumentidest, MS Exceli töövihikutest, MS PowerPointi esitlustest, Adobe Photoshopi failidest ja erinevatest pildivormingutest. Saadaval on suur hulk kasulikke funktsioone ja sätteid.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kuidas eemaldada allkirjad Text oma dokumendist Potx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) pakub kasulikku funktsiooni Potx dokumentide Text allkirjade eemaldamiseks mõne koodireaga.
        
        * Esiteks looge signatuuriobjekt, mis edastab konstruktori parameetrina teie dokumendi tee.
        * Seejärel looge sobiv allkirjaobjekt ja seadistage selle kordumatu identifikaator.
        * Pärast seda käivitage kustutamismeetod, mis edastab allkirjaobjekti, mis tuleb kustutada.
        * Lõpuks protsessi toimimise tulemused.

    title_right: "Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for .NET toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laadige alla toote GroupDocs.Signature for .NET uusim versioon saidilt [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Potx file
        string filePath = "input.potx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allkirjastamine Text allkirjaga Live Demo"
    content: |
       Lisage kohe failile Potx erinevad elektroonilised allkirjad, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kustutage oma allkirjad Text rakendusega C#"
    content: |
        "Erinevatele dokumendivormingutele lisatud e-allkirjade kustutamine. Eemaldage allkirjad kiiresti ilma lisakoodita."
    format: 
       
       
back_to_top:
    enable: true
---