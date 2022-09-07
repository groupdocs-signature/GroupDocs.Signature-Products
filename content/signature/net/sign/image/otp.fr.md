---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Otp
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Otp for C#

############################# Head ############################
head_title: "Ajout de signatures Image au fichier Otp avec C#"
head_description: "Mettez Image Signature sur le fichier Otp pour .NET en utilisant quelques lignes de code. Utilisez l'API GroupDocs Document Signature pour signer des dizaines de formats de fichiers."

############################# Header ############################
title: "Signez des fichiers Otp avec des signatures Image en C#"
description: "Comment ajouter Image Signature avec quelques lignes de code .NET"
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
    title: "À propos de l'API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) est une API populaire pour la signature électronique de documents numériques. Des signatures telles que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées sont disponibles. Les signatures peuvent être placées sur des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Les clients peuvent signer leur document et mettre à jour, rechercher, vérifier, supprimer ou prévisualiser les signatures électroniques apposées sur ces documents. De plus, de nombreuses capacités de personnalisation des signatures sont fournies.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Étapes pour signer Otp avec Image dans C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permet de signer rapidement et facilement des documents Otp avec des signatures Image.
        
        * Créez une instance de la classe Signature fournissant le fichier Otp censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Otp ou le flux de mémoire

    title_right: "System Requirements"
    content_right: |
        La signature de documents avec GroupDocs.Signature for .NET peut être effectuée en quelques étapes simples. Nos API sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenez le dernier GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Otp file
        string filePath = "input.otp";
        // Set up output file
        string outputFilePath = "output.otp";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Otp document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Otp avec Image Live Demo"
    content: |
       Signez dès maintenant le fichier Otp avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Image prises en charge pour C#"
    content: |
        "Vous pouvez également signer Otp avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---