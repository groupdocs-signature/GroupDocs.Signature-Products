---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Potm
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Potm for C#

############################# Head ############################
head_title: "Qrcode failų Potm parašų patvirtinimas naudojant C#"
head_description: "Naudokite tik kelias .NET kodo eilutes, kad patikrintumėte Potm dokumentus ir jų Qrcode parašus."

############################# Header ############################
title: "Qrcode parašų patvirtinimas Potm failams"
description: "API, skirta .NET, suteikia galimybę patvirtinti Qrcode parašus Potm dokumentuose. El. parašų patvirtinimas jūsų Potm dokumentuose gali būti atliktas greitai ir paprastai."
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
    title: "Atraskite naujas GroupDocs.Signature for .NET API funkcijas"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API suteikia daug įvairių būdų, kaip apdoroti įvairių formatų dokumentus naudojant elektroninius parašus. Palaikomi daugelio tipų skaitmeniniai parašai, tokie kaip tekstai, vaizdai, skaitmeniniai sertifikatai, brūkšniniai kodai, QR kodai, antspaudai ar metaduomenys. Klientai gali pridėti, pašalinti, redaguoti, patvirtinti arba ieškoti skaitmeninių parašų PDF, MS Word dokumentuose, MS Excel darbaknygėse, MS PowerPoint pristatymuose, Adobe Photoshop failuose ir įvairiuose vaizdo formatuose. Galimas stulbinantis papildomų funkcijų ir nustatymų skaičius.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kaip patvirtinti Qrcode parašus Potm dokumente"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) apima naudingas funkcijas, pvz., Qrcode parašų, pateiktų Potm dokumentuose, patvirtinimą. Pasinaudokite šia galimybe neįdiegę papildomo kodo.
        
        * Pirma, sukurkite parašo klasę, kaip konstruktoriaus parametro kelią į dokumentą, kuris turėtų būti patikrintas.
        * Antra, sukurkite naują VerifyOptions objektą ir nustatykite visas reikalingas ypatybes.
        * Galiausiai iškvieskite Signature objekto Verify metodą, perduodantį VerifyOptions egzempliorių.
        * Tada apdorokite patikrinimo rezultatus.

    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for .NET palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Atsisiųskite naujausią GroupDocs.Signature for .NET versiją iš [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Potm file
        string filePath = "input.potm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Pasirašymas naudojant Qrcode parašus Tiesioginė demonstracija"
    content: |
       Pridėkite įvairių elektroninių parašų prie Potm failo dabar, apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Patikrinkite kitus Qrcode parašus naudodami C#"
    content: |
        "Įvairiuose dokumentuose dedamų elektroninių parašų tikrinimas. Patikrinkite parašų kokybę populiariuose failų formatuose, kaip parodyta toliau."
    format: 
       
       
back_to_top:
    enable: true
---