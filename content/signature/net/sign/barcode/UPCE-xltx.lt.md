---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCE
fileformat: Xltx
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xltx for C#

############################# Head ############################
head_title: "eSign Xltx dokumentas su UPCE brūkšniniu kodu C#"
head_description: "Sukurkite UPCE brūkšninio kodo parašą ir įdėkite jį į Xltx dokumentą su .NET naudodami kelias kodo eilutes. Naudokite GroupDocs Document Signature API norėdami pasirašyti įvairius failų formatus."

############################# Header ############################
title: "Sugeneruokite UPCE brūkšninio kodo parašą Xltx dokumentui C#"
description: "e. Pasirašykite Xltx verslo dokumentus naudodami UPCE brūkšninį kodą. Greitai ir lengvai sugeneruokite brūkšninio kodo parašą naudodami kelias kodo eilutes, kad nustatytumėte pasirašymo parinktis."
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
    title: "Apie GroupDocs.Signature for .NET brūkšninio kodo parašų API."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) yra greita ir paprasta API, skirta valdyti skaitmeninių dokumentų el. pasirašymą naudojant brūkšninių kodų tipus, pvz., UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 ir daugelis kitų. Klientai gali lengvai sukurti brūkšninius kodus su reikiamu tekstu ir įdėti juos į PDF, Microsoft Office Words dokumentus, Microsoft Office Excel darbaknyges, MS PowerPoint pristatymus, Adobe Photoshop failus ir įvairius vaizdo formatus. Brūkšninius kodus, esančius dokumentuose, galima atnaujinti, ieškoti, patikrinti, ištrinti arba peržiūrėti. Be to, palaikomas brūkšninių kodų pritaikymas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Veiksmai norint pasirašyti Xltx naudojant Barcode programoje C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) suteikia galimybę greitai ir lengvai pasirašyti Xltx dokumentus su Barcode parašais.
        
        * Sukurkite parašo klasės egzempliorių, pateikiantį Xltx failą, kuris turėtų būti pasirašytas kaip kelias arba atminties srautas
        * Sukurkite SignOptions klasę ir nustatykite visus reikalingus duomenis.
        * Iškvieskite Signature.Sign() metodą, perduodantį išvesties Xltx failą arba atminties srautą

    title_right: " Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for .NET palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Gaukite naujausią GroupDocs.Signature for .NET iš [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xltx file
        string filePath = "input.xltx";
        // Set up output file
        string outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.UPCE,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Xltx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentų Xltx pasirašymas naudojant Barcode tiesioginę demonstraciją"
    content: |
       Pasirašykite Xltx failą įvairiais parašais dabar apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje. Jūsų laukia nemokama internetinė demonstracinė versija.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCE Barcode"
          content: |
            Universalus produkto kodas yra brūkšninio kodo simbolika, plačiai naudojama visame pasaulyje stebint prekybos prekes parduotuvėse. UPCE yra 8 skaitmenų UPC variantas.
          characterset: |
             Palaiko tik skaitinius skaitmenis (0–9).
          textcapacity: |
             Kodo teksto talpa: tiksliai 7 skaitmenys + 1 kontrolinis skaitmuo.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAEAAAABjCAYAAAArUQZGAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAUTSURBVHhe7ZBBqmQBCAP7/pfuMUwXyMcIkuV7BRK1wIWf78N5H/DLx/I+4JeP5X3ALx/L+oDP57/+m0I9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE548xDeB/zysbwP+OVjefgDvt9/E/iHbcwlZ5QAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kiti palaikomi Barcode parašai, skirti C#"
    content: |
        "Taip pat galite pasirašyti Xltx naudodami kitų tipų parašus. Žiūrėkite žemiau esantį sąrašą."
    format: 
        
       
back_to_top:
    enable: true
---