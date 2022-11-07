---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Doc
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Doc for C#

############################# Head ############################
head_title: "Sukurkite tekstinius elektroninius parašus į failą Doc naudodami C#"
head_description: "Įdėkite Text el. parašą į Doc failą, skirtą .NET, naudodami kelias kodo eilutes. Norėdami pasirašyti daugybę failų formatų, naudokite GroupDocs Document Signature API."

############################# Header ############################
title: "Pasirašykite Doc failus naudodami Text parašus C#"
description: "Kaip pridėti Text parašą su keliomis .NET kodo eilutėmis"
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
    title: "Apie GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) yra populiari skaitmeninių dokumentų el. pasirašymo API. Galimi parašai, tokie kaip tekstai, vaizdai, skaitmeniniai sertifikatai, brūkšniniai kodai, QR kodai, antspaudai ar metaduomenys. Parašai gali būti dedami ant PDF, MS Word dokumentų, MS Excel darbaknygų, MS PowerPoint pristatymų, Adobe Photoshop failų ir įvairių vaizdų formatų. Klientai gali pasirašyti savo dokumentą ir atnaujinti, ieškoti, tikrinti, ištrinti ar peržiūrėti ant tų dokumentų įrašytus el. Be to, suteikiama daug parašų pritaikymo galimybių.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Veiksmai norint pasirašyti Doc naudojant Text programoje C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) suteikia galimybę greitai ir lengvai pasirašyti Doc dokumentus su Text parašais.
        
        * Sukurkite parašo klasės egzempliorių, pateikiantį Doc failą, kuris turėtų būti pasirašytas kaip kelias arba atminties srautas
        * Sukurkite SignOptions klasę ir nustatykite visus reikalingus duomenis.
        * Iškvieskite Signature.Sign() metodą, perduodantį išvesties Doc failą arba atminties srautą

    title_right: " Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for .NET palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Gaukite naujausią GroupDocs.Signature for .NET iš [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentų Doc pasirašymas naudojant Text tiesioginę demonstraciją"
    content: |
       Pasirašykite Doc failą įvairiais parašais dabar apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje. Jūsų laukia nemokama internetinė demonstracinė versija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kiti palaikomi Text parašai, skirti C#"
    content: |
        "Taip pat galite pasirašyti Doc naudodami kitų tipų parašus. Žiūrėkite žemiau esantį sąrašą."
    format: 
       
       
back_to_top:
    enable: true
---