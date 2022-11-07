---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Xlsm
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Xlsm for C#

############################# Head ############################
head_title: "Ištrinkite Qrcode parašus iš Xlsm failų naudodami C#"
head_description: "Konkrečius Qrcode parašus iš pasirašytų Xlsm dokumentų galima lengvai ištrinti naudojant trumpą .NET kodą."

############################# Header ############################
title: "Pašalinkite Qrcode parašus, kurie yra Xlsm failuose"
description: "Ištrinkite įvairius Qrcode parašus iš Xlsm dokumentų. Norint pašalinti Qrcode parašus, reikia paprasto C# kodo."
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
    title: "Gaukite informacijos apie GroupDocs.Signature for .NET API funkcijas"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API suteikia daug būdų, kaip apdoroti dokumentus naudojant elektroninius parašus. Galimi skaitmeniniai parašai, tokie kaip tekstai, vaizdai, skaitmeniniai sertifikatai, brūkšniniai kodai, QR kodai, antspaudai ar metaduomenys. Klientai turi galimybę pridėti, ištrinti, atnaujinti, tikrinti ar ieškoti skaitmeninių parašų PDF, MS Word dokumentuose, MS Excel darbaknygėse, MS PowerPoint pristatymuose, Adobe Photoshop failuose ir įvairiuose vaizdo formatuose. Pateikiama daugybė naudingų funkcijų ir nustatymų.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kaip pašalinti Qrcode parašus iš Xlsm dokumento"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) yra naudinga funkcija, skirta išvalyti Xlsm dokumentus nuo Qrcode parašų naudojant kelias kodo eilutes.
        
        * Pirma, kaip konstruktoriaus parametrą sukurkite parašo objektą, perduodantį kelią į jūsų dokumentą.
        * Tada sukurkite atitinkamą parašo objektą ir nustatykite jo unikalų identifikatorių.
        * Po to iškvieskite Delete metodą, perduodantį parašo objektą, kurį reikia ištrinti.
        * Galiausiai proceso operacijos rezultatai.

    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for .NET palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Atsisiųskite naujausią GroupDocs.Signature for .NET versiją iš [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsm file
        string filePath = "input.xlsm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                // set up particular signature id
                QrCodeSignature signatureToDelete = new QrCodeSignature(id);

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
    title: "Pasirašymas naudojant Qrcode parašus Tiesioginė demonstracija"
    content: |
       Pridėkite įvairių elektroninių parašų prie Xlsm failo dabar, apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ištrinkite savo Qrcode parašus naudodami C#"
    content: |
        "El. parašų, kurie buvo pridėti prie įvairių formatų dokumentų, panaikinimas. Greitai pašalinkite parašus be papildomo kodo."
    format: 
       
       
back_to_top:
    enable: true
---