---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for C#

############################# Head ############################
head_title: "Ajout de signatures électroniques numériques au fichier Dotx avec C#"
head_description: "Mettez la signature numérique sur le fichier Dotx pour .NET en utilisant quelques lignes de code. Utilisez l'API GroupDocs Document Signature pour signer des dizaines de formats de fichiers."

############################# Header ############################
title: "eSign Dotx fichiers avec Digital signatures en C#"
description: "Comment ajouter la signature Digital avec quelques lignes de code .NET"
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
    title: "À propos de l'API de signatures numériques GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) est une API populaire pour signer des documents avec des signatures électroniques numériques, avec des certificats numériques. Pour les signatures numériques, l'API utilise des fichiers de certificat PFX pour signer un document avec des clés privées et publiques protégées par mot de passe. Les signatures numériques peuvent être utilisées pour certifier des documents commerciaux avec une page particulière eSign PDF, certifier des documents Microsoft Office entiers tels que Words, Excel, des fichiers Powerpoint et des documents Open Office. Les clients peuvent facilement manipuler les signatures comme les modifier, les supprimer ou les ajuster. L'API fournit un moyen de rechercher et de vérifier les signatures. De plus, de nombreuses capacités de personnalisation des signatures sont fournies.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Étapes pour signer Dotx avec Digital dans C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permet de signer rapidement et facilement des documents Dotx avec des signatures Digital.
        
        * Créez une instance de la classe Signature fournissant le fichier Dotx censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Dotx ou le flux de mémoire

    title_right: " Configuration requise"
    content_right: |
        GroupDocs.Signature for .NET sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenez le dernier GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";
        // Set up output file
        string outputFilePath = "output.dotx";
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

                // sign Dotx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Dotx avec Digital Live Demo"
    content: |
       Signez dès maintenant le fichier Dotx avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Digital prises en charge pour C#"
    content: |
        "Vous pouvez également signer Dotx avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---