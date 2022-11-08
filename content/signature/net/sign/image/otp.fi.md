---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Otp
productName: .NET
lang: fi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Otp for C#

############################# Head ############################
head_title: "Allekirjoitusten Image lisääminen tiedostoon Otp ohjelmalla C#"
head_description: "Aseta Image Allekirjoitus Otp-tiedostoon .NET käyttämällä muutamaa koodiriviä. Käytä GroupDocs Document Signature API allekirjoittaaksesi kymmeniä tiedostomuotoja."

############################# Header ############################
title: "Allekirjoita Otp tiedostot Image allekirjoituksilla C#"
description: "Kuinka lisätä Image-allekirjoitus, jossa on muutama rivi .NET-koodia"
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
    title: "Tietoja GroupDocs.Signature for .NET Image signatures API:sta"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) on suosittu sovellusliittymä digitaalisten asiakirjojen sähköiseen allekirjoittamiseen. Saatavilla on allekirjoituksia, kuten tekstejä, kuvia, digitaalisia varmenteita, viivakoodeja, QR-koodeja, leimoja tai metatietoja. Allekirjoituksia voidaan sijoittaa PDF-tiedostoihin, MS Word -asiakirjoihin, MS Excel -työkirjoihin, MS PowerPoint -esityksiin, Adobe Photoshop -tiedostoihin ja erilaisiin kuvamuotoihin. Asiakkaat voivat allekirjoittaa asiakirjansa ja päivittää, etsiä, tarkistaa, poistaa tai esikatsella asiakirjoihin lisättyjä sähköisiä allekirjoituksia. Lisäksi tarjolla on paljon mahdollisuuksia allekirjoitusten mukauttamiseen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Otp:n allekirjoittamiseen Image -sovelluksella C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tarjoaa mahdollisuuden allekirjoittaa Otp-asiakirjoja Image-allekirjoituksella nopeasti ja helposti.
        
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
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Otp document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Otp asiakirjoja Image Live-demolla"
    content: |
       Allekirjoita Otp-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Image allekirjoitukset ohjelmalle C#"
    content: |
        "Voit myös allekirjoittaa {{Tiedostomuoto}} muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
       
       
back_to_top:
    enable: true
---