---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Ots
productName: .NET
lang: fi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Ots with C#

############################# Head ############################
head_title: "Etsi Text allekirjoituksia Ots-tiedostosta C#"
head_description: "Käytä .NET:a etsiäksesi Text-allekirjoituksia Ots-tiedostoista muutamalla koodirivillä."

############################# Header ############################
title: "Etsi Text allekirjoituksia Ots-tiedostosta"
description: ".NET-natiivisovellusliittymä mahdollistaa Text-allekirjoitusten etsimisen jo allekirjoitetuista Ots-tiedostoista. Suorita laajennettu sähköinen allekirjoitushaku Ots-asiakirjoissasi muutaman koodirivin avulla."
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
    title: "Tietoja GroupDocs.Signature for .NET API:sta"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tarjoaa .NET-sovellusliittymän asiakirjojen käsittelyyn käyttämällä erilaisia ​​allekirjoitustyyppejä, kuten tekstejä, kuvia, digitaalisia varmenteita, viivakoodeja, QR-koodeja, leimoja tai metatietoja. Käyttäjät voivat lisätä, poistaa, päivittää, tarkistaa tai etsiä sähköisiä allekirjoituksia PDF-tiedostoista, MS Word -asiakirjoista, MS Excel -työkirjoista, MS PowerPoint -esityksistä, Adobe Photoshop -tiedostoista ja erilaisista kuvaformaateista, ja allekirjoitusten ominaisuuksien mukauttamiseen tarvitaan lisätukea.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Allekirjoitusten Text etsiminen tiedostomuodossa Ots"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) helpottaa .NET-kehittäjien etsimistä Text-allekirjoituksista Ots-tiedostoista sovelluksistaan ​​toteuttamalla muutaman helpon vaiheen.
        
        * Luo uusi Signature-luokan esiintymä ja anna lähdedokumentin polku rakentajaparametriksi.
        * Instantoi SearchOptions-objekti tarpeidesi mukaan ja määritä hakuasetukset.
        * Kutsu Signature-luokan ilmentymän hakumenetelmä ja välitä sille SearchOptions.
        * Käsittele hakutulokset tarpeidesi mukaan.

    title_right: "Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for .NET on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Lataa tuotteen GroupDocs.Signature for .NET uusin versio osoitteesta [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ots file
        string filePath = "input.ots";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Ots document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Etsi Text sähköisiä allekirjoituksia Live Demo"
    content: |
       Etsi asiakirjasta erilaisia ​​sähköisiä allekirjoituksia Ots-tiedostoille juuri nyt käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Etsi muita Text allekirjoituksia käyttämällä C#"
    content: |
        "Sähköiset allekirjoitukset hakevat eri asiakirjoista. Etsi allekirjoituksia yhdestä suosituista tiedostomuodoista alla olevan kuvan mukaisesti."
    format: 
           
       
back_to_top:
    enable: true
---