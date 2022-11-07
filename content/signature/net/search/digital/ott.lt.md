---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Ott
productName: .NET
lang: lt
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Ott with C#

############################# Head ############################
head_title: "Ieškokite Digital parašų Ott faile C#"
head_description: "Naudokite .NET, norėdami ieškoti Digital parašų Ott failuose naudodami kelias kodo eilutes."

############################# Header ############################
title: "Ieškokite Digital parašų Ott faile"
description: ".NET savoji API leidžia ieškoti Digital parašų jau pasirašytuose Ott failuose. Atlikite išplėstinę el. parašo paiešką savo Ott dokumentuose naudodami kelias kodo eilutes."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Apie GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) teikia .NET API, skirtą dokumentams apdoroti naudojant įvairius parašo tipus, pvz., tekstus, vaizdus, ​​skaitmeninius sertifikatus, brūkšninius kodus, QR kodus, antspaudus ar metaduomenis. Vartotojai gali pridėti, ištrinti, atnaujinti, tikrinti arba ieškoti elektroninių parašų PDF rinkmenose, MS Word dokumentuose, MS Excel darbaknygėse, MS PowerPoint pristatymuose, Adobe Photoshop failuose ir įvairiuose vaizdo formatuose, su papildoma pagalba prireikus tinkinti parašų ypatybes.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kaip ieškoti Digital parašų Ott"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) leidžia .NET kūrėjams lengviau ieškoti Digital parašų Ott failuose iš savo programų, atlikdami kelis paprastus veiksmus.
        
        * Sukurkite naują Signature klasės egzempliorių ir nurodykite šaltinio dokumento kelią kaip konstruktoriaus parametrą.
        * Sukurkite paieškos parinkčių objektą pagal savo reikalavimus ir nurodykite paieškos parinktis.
        * Iškvieskite Signature klasės egzemplioriaus paieškos metodą ir perduokite jam paieškos parinktis.
        * Apdorokite paieškos rezultatus pagal savo poreikius.

    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for .NET palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Atsisiųskite naujausią GroupDocs.Signature for .NET versiją iš [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ott file
        string filePath = "input.ott";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                DigitalSearchOptions options = new DigitalSearchOptions()
                {
                    // specify special search criteria
                    Comments = "Approved",
                    // specify date range period of signature
                    SignDateTimeFrom = new DateTime(year: 2020, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2020, month: 12, day: 31)
                };

                // search for Digital signatures in Ott document
                List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

                // process signatures which were found                
                foreach (DigitalSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ieškokite Digital elektroninių parašų tiesioginės demonstracijos"
    content: |
       Dabar ieškokite dokumente įvairių elektroninių parašų prie Ott failų, apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Ieškokite kitų Digital parašų naudodami C#"
    content: |
        "Elektroninių parašų paieška įvairiuose dokumentuose. Raskite parašus iš vieno iš populiarių failų formatų, kaip parodyta toliau."
    format: 
           
       
back_to_top:
    enable: true
---