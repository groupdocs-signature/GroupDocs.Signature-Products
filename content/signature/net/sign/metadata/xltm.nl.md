---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xltm
productName: .NET
lang: nl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xltm for C#

############################# Head ############################
head_title: "Voeg elektronische handtekeningen met metagegevens toe aan Xltm documenten via C#"
head_description: "Gebruik metadata als verborgen elektronische handtekeningen in uw Xltm-documenten met een paar regels C#-code. Gebruik de GroupDocs Document Signature API om uw zakelijke documenten en bestanden elektronisch te ondertekenen met metadata-informatie."

############################# Header ############################
title: "Metadata elektronische handtekeningen voor Xltm document via .NET zijn eenvoudig en gemakkelijk te gebruiken!"
description: "Onderteken uw Xltm documenten en contracten met verborgen metadata-items. Genereer probleemloos metadata voor PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties en verschillende afbeeldingsformaten."
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
    title: "Over GroupDocs.Signature for .NET API voor handtekeningen met metagegevens"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is een populaire API voor het elektronisch ondertekenen van digitale documenten. Handtekeningen zoals teksten, afbeeldingen, digitale certificaten, barcodes, QR-codes, stempels of metadata zijn beschikbaar. Handtekeningen kunnen worden geplaatst op PDF's, MS Word-documenten, MS Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsformaten. Klanten kunnen hun document ondertekenen en de elektronische handtekeningen die op die documenten zijn geplaatst bijwerken, zoeken, verifiëren, verwijderen of een voorbeeld bekijken. Bovendien zijn er veel mogelijkheden voor het aanpassen van handtekeningen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappen om Xltm te ondertekenen met Metadata in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) biedt de mogelijkheid om Xltm documenten snel en gemakkelijk te ondertekenen met Metadata handtekeningen.
        
        * Maak een instantie van de Signature-klasse die een Xltm-bestand levert dat moet worden ondertekend als pad of geheugenstroom
        * Instantieer SignOptions klasse en stel alle gevraagde gegevens in.
        * Roep de Signature.Sign()-methode op en geef uitvoer Xltm-bestand of geheugenstroom

    title_right: " systeem vereisten"
    content_right: |
        GroupDocs.Signature for .NET worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download de nieuwste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xltm file
        string filePath = "input.xltm";
        // Set up output file
        string outputFilePath = "output.xltm";

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
                
                // sign Xltm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Xltm documenten ondertekenen met Metadata Live Demo"
    content: |
       Onderteken het Xltm-bestand met verschillende handtekeningen op dit moment door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan. Gratis online demo voor u klaar.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere ondersteunde Metadata handtekeningen voor C#"
    content: |
        "U kunt Xltm ook ondertekenen met andere soorten handtekeningen. Zie de lijst hieronder."
    format: 
       
       
back_to_top:
    enable: true
---