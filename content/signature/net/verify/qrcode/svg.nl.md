---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Svg
productName: .NET
lang: nl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Svg for C#

############################# Head ############################
head_title: "Verificatie van Qrcode handtekeningen voor Svg bestanden via C#"
head_description: "Gebruik slechts een paar regels .NET-code om Svg-documenten en hun Qrcode-handtekeningen te verifiëren."

############################# Header ############################
title: "Qrcode handtekeningverificatie voor Svg bestanden"
description: "API voor .NET biedt de mogelijkheid om Qrcode handtekeningen te verifiëren bij Svg documenten. Verificatie van elektronische handtekeningen in uw Svg documenten kan snel en gemakkelijk worden uitgevoerd."
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
    title: "Ontdek nieuwe GroupDocs.Signature for .NET API-functies"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API biedt een breed scala aan manieren om tal van documentformaten te verwerken met behulp van elektronische handtekeningen. Vele soorten digitale handtekeningen zoals teksten, afbeeldingen, digitale certificaten, barcodes, QR-codes, stempels of metadata worden ondersteund. Klanten kunnen digitale handtekeningen toevoegen, verwijderen, bewerken, valideren of zoeken in PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsformaten. Verbazingwekkend aantal extra functies en instellingen zijn beschikbaar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe u Qrcode handtekeningen valideert in uw Svg document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bevat handige functies zoals verificatie van Qrcode handtekeningen die bij Svg documenten zijn geplaatst. Gebruik deze mogelijkheid zonder extra code te implementeren.
        
        * Ten eerste, instantiëren Signature-klasse die als een constructorparameterpad biedt naar een document dat moet worden geverifieerd.
        * Maak vervolgens een nieuw VerifyOptions-object en stel alle vereiste eigenschappen in.
        * Roep ten slotte de object Verify-methode van Signature aan die de instantie van VerifyOptions doorgeeft.
        * Verwerk vervolgens de verificatieresultaten.

    title_right: "systeem vereisten"
    content_right: |
        GroupDocs.Signature for .NET worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download de nieuwste versie van GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Svg file
        string filePath = "input.svg";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ondertekenen met Qrcode handtekeningen Live demo"
    content: |
       Voeg nu verschillende elektronische handtekeningen toe aan het Svg-bestand door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifieer andere Qrcode handtekeningen met C#"
    content: |
        "Verificatie van elektronische handtekeningen in verschillende documenten. Controleer de kwaliteit van handtekeningen in de populaire bestandsindelingen, zoals hieronder wordt onthuld."
    format: 
       
       
back_to_top:
    enable: true
---