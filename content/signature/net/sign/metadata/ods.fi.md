---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ods
productName: .NET
lang: fi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ods for C#

############################# Head ############################
head_title: "Liitä metatietojen sähköiset allekirjoitukset Ods-asiakirjoihin C#:n kautta"
head_description: "Käytä metatietoja piilotettuina sähköisinä allekirjoituksina Ods-asiakirjoissasi käyttämällä pari riviä C#-koodia. Käytä GroupDocs Document Signature API:ta yrityksesi dokumenttien ja tiedostojen sähköiseen allekirjoittamiseen metatietotiedoilla."

############################# Header ############################
title: "Metatietojen sähköiset allekirjoitukset asiakirjalle Ods tuotteen .NET kautta ovat yksinkertaisia ​​ja helppokäyttöisiä!"
description: "eAllekirjoita Ods asiakirjasi ja sopimuksi piilotetuilla metatietomerkinnöillä. Luo metatietoja PDF-tiedostoille, MS Word -asiakirjoille, MS Excel -työkirjoille, MS PowerPoint -esityksille ja erilaisille kuvamuodoille ilman ongelmia ja ylimääräistä koodausta."
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
    title: "Tietoja GroupDocs.Signature for .NET Metadata Signatures API:sta"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) on suosittu sovellusliittymä digitaalisten asiakirjojen sähköiseen allekirjoittamiseen. Saatavilla on allekirjoituksia, kuten tekstejä, kuvia, digitaalisia varmenteita, viivakoodeja, QR-koodeja, leimoja tai metatietoja. Allekirjoituksia voidaan sijoittaa PDF-tiedostoihin, MS Word -asiakirjoihin, MS Excel -työkirjoihin, MS PowerPoint -esityksiin, Adobe Photoshop -tiedostoihin ja erilaisiin kuvamuotoihin. Asiakkaat voivat allekirjoittaa asiakirjansa ja päivittää, etsiä, tarkistaa, poistaa tai esikatsella asiakirjoihin lisättyjä sähköisiä allekirjoituksia. Lisäksi tarjolla on paljon mahdollisuuksia allekirjoitusten mukauttamiseen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Vaiheet Ods:n allekirjoittamiseen Metadata -sovelluksella C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tarjoaa mahdollisuuden allekirjoittaa Ods-asiakirjoja Metadata-allekirjoituksella nopeasti ja helposti.
        
        * Luo Signature-luokan ilmentymä, joka tarjoaa Ods-tiedoston, joka on tarkoitus allekirjoittaa polkuna tai muistivirtana
        * Luo SignOptions-luokka ja aseta kaikki vaaditut tiedot.
        * Kutsu Signature.Sign() -menetelmä, joka välittää Ods -tiedoston tai muistivirran

    title_right: " Laitteistovaatimukset"
    content_right: |
        GroupDocs.Signature for .NET on tuettu kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.

        * Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        * Kehitysympäristöt: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Hanki uusin GroupDocs.Signature for .NET käyttäjältä [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allekirjoitetaan Ods asiakirjoja Metadata Live-demolla"
    content: |
       Allekirjoita Ods-tiedosto useilla allekirjoituksilla heti käymällä [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) -sivustolla. Ilmainen online-demo odottaa sinua.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muut tuetut Metadata allekirjoitukset ohjelmalle C#"
    content: |
        "Voit myös allekirjoittaa {{Tiedostomuoto}} muilla allekirjoitustyypeillä. Katso alla oleva luettelo."
    format: 
       
       
back_to_top:
    enable: true
---