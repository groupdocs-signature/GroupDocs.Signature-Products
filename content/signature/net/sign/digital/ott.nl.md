---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ott
productName: .NET
lang: nl
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ott for C#

############################# Head ############################
head_title: "Digitale elektronische handtekeningen toevoegen aan Ott bestand met C#"
head_description: "Zet de digitale handtekening op het Ott-bestand voor .NET met een paar regels code. Gebruik de GroupDocs Document Signature API om tientallen bestandsindelingen te ondertekenen."

############################# Header ############################
title: "eSign Ott bestanden met Digital handtekeningen in C#"
description: "Hoe een Digital handtekening toe te voegen met een paar regels .NET code"
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
    title: "Over GroupDocs.Signature for .NET API voor digitale handtekeningen"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) is een populaire API om documenten te ondertekenen met de digitale elektronische handtekeningen, met digitale certificaten. Voor de API voor digitale handtekeningen gebruikt de API PFX-certificaatbestanden om documenten te ondertekenen met met een wachtwoord beveiligde privé- en openbare sleutels. De digitale handtekeningen kunnen worden gebruikt om zakelijke documenten te certificeren met een specifieke eSign PDF-pagina, en om volledige Microsoft Office-documenten zoals Words, Excel, Powerpoint-bestanden en Open Office-documenten te certificeren. Klanten kunnen de handtekeningen gemakkelijk manipuleren, zoals bewerken, verwijderen of aanpassen. De API biedt een manier om handtekeningen te zoeken en te verifiëren. Bovendien zijn er veel mogelijkheden voor het aanpassen van handtekeningen.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Stappen om Ott te ondertekenen met Digital in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) biedt de mogelijkheid om Ott documenten snel en gemakkelijk te ondertekenen met Digital handtekeningen.
        
        * Maak een instantie van de Signature-klasse die een Ott-bestand levert dat moet worden ondertekend als pad of geheugenstroom
        * Instantieer SignOptions klasse en stel alle gevraagde gegevens in.
        * Roep de methode Signature.Sign() op en geef uitvoer Ott-bestand of geheugenstroom

    title_right: " systeem vereisten"
    content_right: |
        GroupDocs.Signature for .NET worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.

        * Besturingssystemen: Microsoft Windows, Linux, MacOS
        * Ontwikkelomgevingen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Download de nieuwste GroupDocs.Signature for .NET van [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ott file
        string filePath = "input.ott";
        // Set up output file
        string outputFilePath = "output.ott";
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

                // sign Ott document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ott documenten ondertekenen met Digital Live Demo"
    content: |
       Onderteken het Ott-bestand met verschillende handtekeningen op dit moment door naar de website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) te gaan. Gratis online demo voor u klaar.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere ondersteunde Digital handtekeningen voor C#"
    content: |
        "U kunt Ott ook ondertekenen met andere soorten handtekeningen. Zie de lijst hieronder."
    format: 
       
       
back_to_top:
    enable: true
---