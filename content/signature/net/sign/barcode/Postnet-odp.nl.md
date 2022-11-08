---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Postnet
fileformat: Odp
productName: .NET
lang: nl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Odp for C#

############################# Head ############################
head_title: "eSign Odp document met Postnet Barcode in C#"
head_description: "Maak een Postnet Barcode Signature en plaats deze op het Odp document met .NET met behulp van een paar regels code. Gebruik de GroupDocs Document Signature API voor het ondertekenen van verschillende bestandsindelingen."

############################# Header ############################
title: "Genereer Postnet Barcode handtekening voor Odp document in C#"
description: "Onderteken uw Odp zakelijke documenten met Postnet Barcode. Genereer snel en eenvoudig een barcodehandtekening met een paar regels code om ondertekeningsopties in te stellen."
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
    title: "Over GroupDocs.Signature for .NET Barcode handtekeningen API."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is een snelle en gemakkelijke API voor het beheren van elektronische ondertekening van digitale documenten met behulp van barcodetypes zoals UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 en vele anderen. Klanten kunnen eenvoudig barcodes maken met de vereiste tekst en deze op PDF, Microsoft Office Words-documenten, Microsoft Office Excel-werkmappen, MS PowerPoint-presentaties, Adobe Photoshop-bestanden en verschillende afbeeldingsformaten plaatsen. Barcodes die in documenten zijn geplaatst, kunnen worden bijgewerkt, doorzocht, geverifieerd, verwijderd of bekeken. Bovendien wordt het aanpassen van streepjescodes ondersteund.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappen om Odp te ondertekenen met Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) biedt de mogelijkheid om Odp documenten snel en gemakkelijk te ondertekenen met Barcode handtekeningen.
        
        * Maak een instantie van de Signature-klasse die een Odp-bestand levert dat moet worden ondertekend als pad of geheugenstroom
        * Instantieer SignOptions klasse en stel alle gevraagde gegevens in.
        * Roep de Signature.Sign()-methode op en geef uitvoer Odp-bestand of geheugenstroom

    title_right: " systeem vereisten"
    content_right: |
        GroupDocs.Signature for .NET worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download de nieuwste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Odp file
        string filePath = "input.odp";
        // Set up output file
        string outputFilePath = "output.odp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Postnet,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Odp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Odp documenten ondertekenen met Barcode Live Demo"
    content: |
       Onderteken het Odp-bestand met verschillende handtekeningen op dit moment door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan. Gratis online demo voor u klaar.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Postnet Barcode"
          content: |
            POSTNET (Postal Numeric Encoding Technique) is een barcode-symboliek die door de United States Postal Service wordt gebruikt om te helpen bij het sturen van post.
          characterset: |
             Numerieke cijfers (0-9).
          textcapacity: |
             Maximaal 11 tekens.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAACcAAAAjCAYAAAAXMhMjAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACeSURBVFhH7c7BCkMxEELR/P9Pp1LoRrCXpi4Cbw5kIRKZtS82x52a407Ncae+HrfWer8Pyr+i/3NcQv/nuIT+z3EJ/X/Ocf9mlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2ubnAHHdqjjt18XF7vwDevzbHqsQWPwAAAABJRU5ErkJggg==

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere ondersteunde Barcode handtekeningen voor C#"
    content: |
        "U kunt Odp ook ondertekenen met andere soorten handtekeningen. Zie de lijst hieronder."
    format: 
        
       
back_to_top:
    enable: true
---