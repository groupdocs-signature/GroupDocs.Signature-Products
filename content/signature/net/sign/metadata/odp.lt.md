---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Odp
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Odp for C#

############################# Head ############################
head_title: "Pridėkite metaduomenų elektroninius parašus prie Odp dokumentų per C#"
head_description: "Naudokite metaduomenis kaip paslėptus elektroninius parašus savo Odp dokumentuose naudodami kelias C# kodo eilutes. Naudokite GroupDocs Document Signature API norėdami el. pasirašyti savo verslo dokumentus ir failus su metaduomenų informacija."

############################# Header ############################
title: "Dokumento Odp metaduomenų elektroniniai parašai naudojant .NET yra paprasti ir lengvai naudojami!"
description: "e. Pasirašykite savo Odp dokumentus ir sutartis su paslėptais metaduomenų įrašais. Kurkite PDF, MS Word dokumentų, MS Excel darbaknygių, MS PowerPoint pristatymų ir įvairių vaizdo formatų metaduomenis be problemų ir papildomo kodavimo."
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
    title: "Apie GroupDocs.Signature for .NET metaduomenų parašų API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) yra populiari skaitmeninių dokumentų el. pasirašymo API. Galimi parašai, tokie kaip tekstai, vaizdai, skaitmeniniai sertifikatai, brūkšniniai kodai, QR kodai, antspaudai ar metaduomenys. Parašai gali būti dedami ant PDF, MS Word dokumentų, MS Excel darbaknygų, MS PowerPoint pristatymų, Adobe Photoshop failų ir įvairių vaizdų formatų. Klientai gali pasirašyti savo dokumentą ir atnaujinti, ieškoti, tikrinti, ištrinti ar peržiūrėti ant tų dokumentų įrašytus el. Be to, suteikiama daug parašų pritaikymo galimybių.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Veiksmai norint pasirašyti Odp naudojant Metadata programoje C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) suteikia galimybę greitai ir lengvai pasirašyti Odp dokumentus su Metadata parašais.
        
        * Sukurkite parašo klasės egzempliorių, pateikiantį Odp failą, kuris turėtų būti pasirašytas kaip kelias arba atminties srautas
        * Sukurkite SignOptions klasę ir nustatykite visus reikalingus duomenis.
        * Iškvieskite Signature.Sign() metodą, perduodantį išvesties Odp failą arba atminties srautą

    title_right: " Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for .NET palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Gaukite naujausią GroupDocs.Signature for .NET iš [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Odp file
        string filePath = "input.odp";
        // Set up output file
        string outputFilePath = "output.odp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Odp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentų Odp pasirašymas naudojant Metadata tiesioginę demonstraciją"
    content: |
       Pasirašykite Odp failą įvairiais parašais dabar apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje. Jūsų laukia nemokama internetinė demonstracinė versija.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kiti palaikomi Metadata parašai, skirti C#"
    content: |
        "Taip pat galite pasirašyti Odp naudodami kitų tipų parašus. Žiūrėkite žemiau esantį sąrašą."
    format: 
       
       
back_to_top:
    enable: true
---