---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Tiff
productName: .NET
lang: nl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Tiff for C#

############################# Head ############################
head_title: "eSign Tiff document met Interleaved2of5 Barcode in C#"
head_description: "Maak Interleaved2of5 Barcode Signature en plaats deze op Tiff document met .NET met behulp van een paar regels code. Gebruik de GroupDocs Document Signature API voor het ondertekenen van verschillende bestandsindelingen."

############################# Header ############################
title: "Genereer Interleaved2of5 Barcode handtekening voor Tiff document in C#"
description: "Onderteken uw Tiff zakelijke documenten met Interleaved2of5 Barcode. Genereer snel en eenvoudig een barcodehandtekening met een paar regels code om ondertekeningsopties in te stellen."
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
    title_left: "Stappen om Tiff te ondertekenen met Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) biedt de mogelijkheid om Tiff documenten snel en gemakkelijk te ondertekenen met Barcode handtekeningen.
        
        * Maak een instantie van de Signature-klasse die een Tiff-bestand levert dat moet worden ondertekend als pad of geheugenstroom
        * Instantieer SignOptions klasse en stel alle gevraagde gegevens in.
        * Roep de methode Signature.Sign() op en geef uitvoer Tiff-bestand of geheugenstroom

    title_right: " systeem vereisten"
    content_right: |
        GroupDocs.Signature for .NET worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download de nieuwste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Tiff file
        string filePath = "input.tiff";
        // Set up output file
        string outputFilePath = "output.tiff";

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
                
                // sign Tiff document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Tiff documenten ondertekenen met Barcode Live Demo"
    content: |
       Onderteken het Tiff-bestand met verschillende handtekeningen op dit moment door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan. Gratis online demo voor u klaar.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) is een continue twee-breedte barcode symbologie coderende cijfers. Het wordt commercieel gebruikt op 135-film, voor ITF-14-barcodes en op dozen van sommige producten, terwijl de producten binnenin zijn gelabeld met UPC of EAN.
          characterset: |
             Numerieke cijfers (0-9).
          textcapacity: |
             Variabele lengte.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere ondersteunde Barcode handtekeningen voor C#"
    content: |
        "U kunt Tiff ook ondertekenen met andere soorten handtekeningen. Zie de lijst hieronder."
    format: 
        
       
back_to_top:
    enable: true
---