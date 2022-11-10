---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "Ištrinkite Digital parašus iš Doc failų naudodami C#"
head_description: "Konkrečius Digital parašus iš pasirašytų Doc dokumentų galima lengvai ištrinti naudojant trumpą .NET kodą."

############################# Header ############################
title: "Pašalinkite Digital parašus, kurie yra Doc failuose"
description: "Ištrinkite įvairius Digital parašus iš Doc dokumentų. Norint pašalinti Digital parašus, reikia paprasto C# kodo."
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
    title_left: "Kaip pašalinti Digital parašus iš Doc dokumento"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) yra naudinga funkcija, skirta išvalyti Doc dokumentus nuo Digital parašų naudojant kelias kodo eilutes.
        
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
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Pasirašymas naudojant Digital parašus Tiesioginė demonstracija"
    content: |
       Pridėkite įvairių elektroninių parašų prie Doc failo dabar, apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ištrinkite savo Digital parašus naudodami C#"
    content: |
        "El. parašų, kurie buvo pridėti prie įvairių formatų dokumentų, panaikinimas. Greitai pašalinkite parašus be papildomo kodo."
    format: 
       
       
back_to_top:
    enable: true
---