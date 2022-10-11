---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Docm
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Docm for C#

############################# Head ############################
head_title: "Ajouter des signatures électroniques de métadonnées aux documents Docm via C#"
head_description: "Utilisez les métadonnées comme signatures électroniques cachées dans vos documents Docm en utilisant quelques lignes de code C#. Utilisez l'API GroupDocs Document Signature pour signer électroniquement vos documents et fichiers commerciaux avec des informations de métadonnées."

############################# Header ############################
title: "Les signatures électroniques de métadonnées pour le document Docm via .NET sont simples et faciles à utiliser !"
description: "Signez électroniquement vos documents et contrats Docm avec des entrées de métadonnées masquées. Générez des métadonnées pour les fichiers PDF, les documents MS Word, les classeurs MS Excel, les présentations MS PowerPoint et divers formats d'image sans problème et avec un codage supplémentaire."
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
    title: "À propos de l'API de signatures de métadonnées GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) est une API populaire pour la signature électronique de documents numériques. Des signatures telles que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées sont disponibles. Les signatures peuvent être placées sur des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Les clients peuvent signer leur document et mettre à jour, rechercher, vérifier, supprimer ou prévisualiser les signatures électroniques apposées sur ces documents. De plus, de nombreuses capacités de personnalisation des signatures sont fournies.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Étapes pour signer Docm avec Metadata dans C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permet de signer rapidement et facilement des documents Docm avec des signatures Metadata.
        
        * Créez une instance de la classe Signature fournissant le fichier Docm censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Docm ou le flux de mémoire

    title_right: " Configuration requise"
    content_right: |
        GroupDocs.Signature for .NET sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenez le dernier GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Docm file
        string filePath = "input.docm";
        // Set up output file
        string outputFilePath = "output.docm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Docm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Docm avec Metadata Live Demo"
    content: |
       Signez dès maintenant le fichier Docm avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Metadata prises en charge pour C#"
    content: |
        "Vous pouvez également signer Docm avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---