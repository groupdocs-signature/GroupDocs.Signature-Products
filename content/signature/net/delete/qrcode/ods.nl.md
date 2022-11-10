---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Ods
productName: .NET
lang: nl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Ods for C#

############################# Head ############################
head_title: "Verwijder Qrcode handtekeningen uit Ods bestanden via C#"
head_description: "Het verwijderen van specifieke Qrcode handtekeningen uit ondertekende Ods documenten kan gemakkelijk worden uitgevoerd met korte .NET code."

############################# Header ############################
title: "Verwijder Qrcode handtekeningen die in Ods bestanden zijn geplaatst"
description: "Verwijder verschillende Qrcode handtekeningen uit Ods documenten. Voor het verwijderen van Qrcode-handtekeningen is een eenvoudige C#-code vereist."
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
    title: "Krijg informatie over GroupDocs.Signature for .NET API-functies"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API biedt vele manieren om uw documenten te verwerken met behulp van elektronische handtekeningen. Digitale handtekeningen zoals teksten, afbeeldingen, digitale certificaten, barcodes, QR-codes, stempels of metadata zijn beschikbaar. Klanten hebben de mogelijkheid om digitale handtekeningen toe te voegen, te verwijderen, bij te werken, te verifiëren of te zoeken in PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsformaten. Er is een groot aantal handige functies en instellingen beschikbaar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe Qrcode handtekeningen te verwijderen uit uw Ods document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) biedt een handige functie voor het wissen van Ods documenten van Qrcode handtekeningen met een paar regels code.
        
        * Instantieer eerst het Signature-object dat het pad naar uw document doorgeeft als een constructorparameter.
        * Maak vervolgens een geschikt handtekeningobject en stel de unieke id in.
        * Roep daarna de Delete-methode aan die het handtekeningobject doorgeeft dat moet worden verwijderd.
        * Tot slot de resultaten van de proceswerking.

    title_right: "systeem vereisten"
    content_right: |
        GroupDocs.Signature for .NET worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download de nieuwste versie van GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ods file
        string filePath = "input.ods";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                // set up particular signature id
                QrCodeSignature signatureToDelete = new QrCodeSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ondertekenen met Qrcode handtekeningen Live demo"
    content: |
       Voeg nu verschillende elektronische handtekeningen toe aan het Ods-bestand door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verwijder uw Qrcode handtekeningen met C#"
    content: |
        "Verwijdering van elektronische handtekeningen die aan verschillende documentformaten zijn toegevoegd. Snel handtekeningen verwijderen zonder extra code."
    format: 
       
       
back_to_top:
    enable: true
---