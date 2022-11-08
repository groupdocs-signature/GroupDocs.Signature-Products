---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Docx
productName: .NET
lang: fi
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docx for C#

############################# Head ############################
head_title: "Digitaalisten sähköisten allekirjoitusten lisääminen tiedostoon Docx ohjelmalla C#"
head_description: "Aseta digitaalinen allekirjoitus Docx-tiedostoon .NET käyttämällä muutamaa koodiriviä. Käytä GroupDocs Document Signature API allekirjoittaaksesi kymmeniä tiedostomuotoja."

############################# Header ############################
title: "eSign Docx tiedostot Digital allekirjoituksella C#"
description: "Allekirjoituksen Digital lisääminen muutamalla rivillä .NET-koodia"
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
    title: "Tietoja digitaalisten allekirjoitusten sovellusliittymästä GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) on suosittu sovellusliittymä asiakirjojen allekirjoittamiseen digitaalisilla sähköisillä allekirjoituksilla ja digitaalisilla varmenteilla. Digitaalisten allekirjoitusten API käyttää PFX-sertifikaattitiedostoja asiakirjan allekirjoittamiseen salasanalla suojatuilla yksityisillä ja julkisilla avaimilla. Digitaalisia allekirjoituksia voidaan käyttää sertifioimaan yritysasiakirjoja tietyllä eSign PDF -sivulla, sertifioimaan kokonaisia ​​Microsoft Office -asiakirjoja, kuten Words-, Excel-, Powerpoint-tiedostoja ja Open Office -asiakirjoja. Asiakkaat voivat helposti muokata allekirjoituksia, kuten muokata niitä, poistaa tai säätää. API tarjoaa tavan etsiä ja vahvistaa allekirjoituksia. Lisäksi tarjolla on paljon mahdollisuuksia allekirjoitusten mukauttamiseen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Docx:n allekirjoittamiseen Digital -sovelluksella C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tarjoaa mahdollisuuden allekirjoittaa Docx-asiakirjoja Digital-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Docx-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Docx -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for .NET on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Hanki uusin GroupDocs.Signature for .NET käyttäjältä [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docx file
        string filePath = "input.docx";
        // Set up output file
        string outputFilePath = "output.docx";
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

                // sign Docx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Docx asiakirjoja Digital Live-demolla"
    content: |
       Allekirjoita Docx-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Digital allekirjoitukset ohjelmalle C#"
    content: |
        "Voit myös allekirjoittaa Docx muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
       
       
back_to_top:
    enable: true
---