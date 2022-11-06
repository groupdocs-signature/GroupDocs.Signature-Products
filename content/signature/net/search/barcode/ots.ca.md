---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Ots
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Ots with C#

############################# Head ############################
head_title: "Cerqueu signatures de Barcode al fitxer Ots a C#"
head_description: "Utilitzeu .NET per cercar signatures Barcode als fitxers Ots mitjançant unes poques línies de codi."

############################# Header ############################
title: "Cerqueu signatures Barcode al fitxer Ots"
description: "L'API nativa de .NET permet cercar signatures Barcode als fitxers Ots ja signats. Feu una cerca avançada de signatura electrònica als vostres documents Ots amb unes poques línies de codi."
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
    title: "Sobre l'API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) proporciona l'API de .NET per processar documents amb diversos tipus de signatura, com ara textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els usuaris poden afegir, suprimir, actualitzar, verificar o cercar signatures electròniques en PDF, documents MS Word, llibres de treball MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge, amb suport addicional per personalitzar les propietats de les signatures segons sigui necessari.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com cercar signatures de Barcode a Ots"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) facilita que els desenvolupadors de .NET cerquin signatures de Barcode als fitxers Ots des de les seves aplicacions implementant uns quants passos senzills.
        
        * Creeu una nova instància de la classe Signature i passeu la ruta del document font com a paràmetre de constructor.
        * Instancieu l'objecte SearchOptions segons els vostres requisits i especifiqueu les opcions de cerca.
        * Truqueu al mètode de cerca de la instància de classe Signature i passeu-li SearchOptions.
        * Processeu els resultats de la cerca segons les vostres demandes.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for .NET són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Baixeu la darrera versió de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ots file
        string filePath = "input.ots";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                BarcodeSearchOptions options = new BarcodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Barcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Barcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Barcode signatures in Ots document
                List<BarcodeSignature> signatures = signature.Search<BarcodeSignature>(options);

                // process signatures which were found                
                foreach (BarcodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cerqueu Barcode signatures electròniques Demostració en directe"
    content: |
       Cerqueu al document diverses signatures electròniques als fitxers Ots ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cerqueu altres signatures de Barcode amb C#"
    content: |
        "Cerca de signatures electròniques en diversos documents. Cerqueu signatures d'un dels formats de fitxer més populars, tal com es mostra a continuació."
    format: 
           
       
back_to_top:
    enable: true
---