---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Otp
productName: .NET
lang: fi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Otp for C#

############################# Head ############################
head_title: "eSign Otp -asiakirja Interleaved2of5-viivakoodilla C#"
head_description: "Luo Interleaved2of5 Viivakoodiallekirjoitus ja laita se Otp-asiakirjaan, jossa on .NET muutamalla rivillä koodia. Käytä GroupDocs Document Signature API:ta eri tiedostomuotojen allekirjoittamiseen."

############################# Header ############################
title: "Luo Interleaved2of5 viivakoodiallekirjoitus asiakirjalle Otp ohjelmassa C#"
description: "eAllekirjoita Otp yritysasiakirjasi Interleaved2of5-viivakoodilla. Luo viivakoodiallekirjoitus nopeasti ja helposti muutamalla koodirivillä allekirjoitusvaihtoehtojen määrittämiseksi."
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
    title_left: "Vaiheet Otp:n allekirjoittamiseen Barcode -sovelluksella C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tarjoaa mahdollisuuden allekirjoittaa Otp-asiakirjoja Barcode-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Otp-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Otp -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for .NET on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Hanki uusin GroupDocs.Signature for .NET käyttäjältä [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Otp file
        string filePath = "input.otp";
        // Set up output file
        string outputFilePath = "output.otp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Interleaved2of5,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Otp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Otp asiakirjoja Barcode Live-demolla"
    content: |
       Allekirjoita Otp-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) on jatkuva kahden leveyden viivakoodisymboliikkakoodaus numeroita. Sitä käytetään kaupallisesti 135-kalvoon, ITF-14-viivakoodeihin ja joidenkin tuotteiden laatikoihin, kun taas sisällä olevat tuotteet on merkitty UPC- tai EAN-merkinnöillä.
          characterset: |
             Numeeriset numerot (0-9).
          textcapacity: |
             Vaihteleva pituus.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Barcode allekirjoitukset ohjelmalle C#"
    content: |
        "Voit myös allekirjoittaa Otp muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
        
       
back_to_top:
    enable: true
---