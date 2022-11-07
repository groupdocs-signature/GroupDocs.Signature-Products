---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Xlsx
productName: .NET
lang: nl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xlsx for C#

############################# Head ############################
head_title: "Verwijder Image handtekeningen uit Xlsx bestanden via C#"
head_description: "Het verwijderen van specifieke Image handtekeningen uit ondertekende Xlsx documenten kan gemakkelijk worden uitgevoerd met korte .NET code."

############################# Header ############################
title: "Verwijder Image handtekeningen die in Xlsx bestanden zijn geplaatst"
description: "Verwijder verschillende Image handtekeningen uit Xlsx documenten. Voor het verwijderen van Image-handtekeningen is een eenvoudige C#-code vereist."
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
    title_left: "Hoe Image handtekeningen te verwijderen uit uw Xlsx document"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) biedt een handige functie voor het wissen van Xlsx documenten van Image handtekeningen met een paar regels code.
        
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
                
        // Set up input Xlsx file
        string filePath = "input.xlsx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

                // provide signature features to delete
                // set up particular signature id
                ImageSignature signatureToDelete = new ImageSignature(id);

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
    title: "Ondertekenen met Image handtekeningen Live demo"
    content: |
       Voeg nu verschillende elektronische handtekeningen toe aan het Xlsx-bestand door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verwijder uw Image handtekeningen met C#"
    content: |
        "Verwijdering van elektronische handtekeningen die aan verschillende documentformaten zijn toegevoegd. Snel handtekeningen verwijderen zonder extra code."
    format: 
       
       
back_to_top:
    enable: true
---