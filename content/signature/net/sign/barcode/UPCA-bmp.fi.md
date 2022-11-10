---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCA
fileformat: Bmp
productName: .NET
lang: fi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Bmp for C#

############################# Head ############################
head_title: "eSign Bmp -asiakirja UPCA-viivakoodilla C#"
head_description: "Luo UPCA Viivakoodiallekirjoitus ja laita se Bmp-asiakirjaan, jossa on .NET muutamalla rivillä koodia. Käytä GroupDocs Document Signature API:ta eri tiedostomuotojen allekirjoittamiseen."

############################# Header ############################
title: "Luo UPCA viivakoodiallekirjoitus asiakirjalle Bmp ohjelmassa C#"
description: "eAllekirjoita Bmp yritysasiakirjasi UPCA-viivakoodilla. Luo viivakoodiallekirjoitus nopeasti ja helposti muutamalla koodirivillä allekirjoitusvaihtoehtojen määrittämiseksi."
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
    title: "Tietoja GroupDocs.Signature for .NET Viivakoodin allekirjoitusten sovellusliittymästä."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) on nopea ja helppo sovellusliittymä digitaalisten asiakirjojen sähköiseen allekirjoittamiseen käyttämällä viivakoodityyppejä, kuten UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 ja monet muut. Asiakkaat voivat luoda helposti tarvittavan tekstin sisältäviä viivakoodeja ja laittaa ne PDF-tiedostoihin, Microsoft Office Words -asiakirjoihin, Microsoft Office Excel -työkirjoihin, MS PowerPoint -esityksiin, Adobe Photoshop -tiedostoihin ja erilaisiin kuvamuotoihin. Asiakirjoihin sijoitettuja viivakoodeja voidaan päivittää, etsiä, tarkistaa, poistaa tai esikatsella joko. Lisäksi viivakoodien räätälöintiä tuetaan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Bmp:n allekirjoittamiseen Barcode -sovelluksella C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tarjoaa mahdollisuuden allekirjoittaa Bmp-asiakirjoja Barcode-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Bmp-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Bmp -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for .NET on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Hanki uusin GroupDocs.Signature for .NET käyttäjältä [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Bmp file
        string filePath = "input.bmp";
        // Set up output file
        string outputFilePath = "output.bmp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.UPCA,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Bmp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Bmp asiakirjoja Barcode Live-demolla"
    content: |
       Allekirjoita Bmp-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCA Barcode"
          content: |
            Universaali tuotekoodi on viivakoodisymboliikka, jota käytetään laajasti maailmanlaajuisesti myymälöissä olevien tuotteiden seuraamiseen.
          characterset: |
             Numeeriset numerot (0-9).
          textcapacity: |
             Täsmälleen 11 numeroa + 1 tarkistusnumero.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAGwAAABjCAYAAAB+MOUYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAARpSURBVHhe7ZFBimBRCMT6/pfuUYaAi6pe58MLSJCAG39+H5/iPexjvId9jPewj/Ee9jHewz7Ge9jH+PNhPz//M4bdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXh5K3sM+xnvYx3gP+xjvYR/jPexT/P7+A4FOQDtpBhIBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Barcode allekirjoitukset ohjelmalle C#"
    content: |
        "Voit myös allekirjoittaa Bmp muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
        
       
back_to_top:
    enable: true
---