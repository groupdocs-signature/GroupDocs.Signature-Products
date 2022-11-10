---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Csv
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Csv with C#

############################# Head ############################
head_title: "Cerqueu signatures de Metadata al fitxer Csv a C#"
head_description: "Utilitzeu .NET per cercar signatures Metadata als fitxers Csv mitjançant unes poques línies de codi."

############################# Header ############################
title: "Cerqueu signatures Metadata al fitxer Csv"
description: "L'API nativa de .NET permet cercar signatures Metadata als fitxers Csv ja signats. Feu una cerca avançada de signatura electrònica als vostres documents Csv amb unes poques línies de codi."
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
    title_left: "Com cercar signatures de Metadata a Csv"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) facilita que els desenvolupadors de .NET cerquin signatures de Metadata als fitxers Csv des de les seves aplicacions implementant uns quants passos senzills.
        
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
        
        // Set up input Csv file
        string filePath = "input.csv";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Csv document
                List<SpreadsheetMetadataSignature> signatures = signature.Search<SpreadsheetMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (SpreadsheetMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cerqueu Metadata signatures electròniques Demostració en directe"
    content: |
       Cerqueu al document diverses signatures electròniques als fitxers Csv ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cerqueu altres signatures de Metadata amb C#"
    content: |
        "Cerca de signatures electròniques en diversos documents. Cerqueu signatures d'un dels formats de fitxer més populars, tal com es mostra a continuació."
    format: 
           
       
back_to_top:
    enable: true
---