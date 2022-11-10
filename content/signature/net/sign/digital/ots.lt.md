---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ots
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ots for C#

############################# Head ############################
head_title: "Skaitmeninių elektroninių parašų pridėjimas prie failo Ots naudojant C#"
head_description: "Įdėkite skaitmeninį parašą į Ots failą, skirtą .NET, naudodami kelias kodo eilutes. Norėdami pasirašyti daugybę failų formatų, naudokite GroupDocs Document Signature API."

############################# Header ############################
title: "eSign Ots failai su Digital parašais C#"
description: "Kaip pridėti Digital parašą su keliomis .NET kodo eilutėmis"
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
    title: "Apie GroupDocs.Signature for .NET skaitmeninių parašų API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) yra populiari API, skirta dokumentams pasirašyti su skaitmeniniais elektroniniais parašais ir skaitmeniniais sertifikatais. Skaitmeninių parašų API naudoja PFX sertifikatų failus, kad pasirašytų dokumentą su slaptažodžiu apsaugotais privačiais ir viešaisiais raktais. Skaitmeniniai parašai gali būti naudojami verslo dokumentams sertifikuoti naudojant eSign PDF konkretų puslapį, sertifikuoti visus Microsoft Office dokumentus, pvz., Words, Excel, Powerpoint failus ir Open Office dokumentus. Klientai gali lengvai manipuliuoti parašais, pavyzdžiui, juos redaguoti, pašalinti ar koreguoti. API suteikia galimybę ieškoti ir patikrinti parašus. Be to, suteikiama daug parašų pritaikymo galimybių.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Veiksmai norint pasirašyti Ots naudojant Digital programoje C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) suteikia galimybę greitai ir lengvai pasirašyti Ots dokumentus su Digital parašais.
        
        * Sukurkite parašo klasės egzempliorių, pateikiantį Ots failą, kuris turėtų būti pasirašytas kaip kelias arba atminties srautas
        * Sukurkite SignOptions klasę ir nustatykite visus reikalingus duomenis.
        * Iškvieskite Signature.Sign() metodą, perduodantį išvesties Ots failą arba atminties srautą

    title_right: " Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for .NET palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Gaukite naujausią GroupDocs.Signature for .NET iš [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ots file
        string filePath = "input.ots";
        // Set up output file
        string outputFilePath = "output.ots";
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

                // sign Ots document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentų Ots pasirašymas naudojant Digital tiesioginę demonstraciją"
    content: |
       Pasirašykite Ots failą įvairiais parašais dabar apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje. Jūsų laukia nemokama internetinė demonstracinė versija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kiti palaikomi Digital parašai, skirti C#"
    content: |
        "Taip pat galite pasirašyti Ots naudodami kitų tipų parašus. Žiūrėkite žemiau esantį sąrašą."
    format: 
       
       
back_to_top:
    enable: true
---