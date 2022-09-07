---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Xltm
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Xltm for C#

############################# Head ############################
head_title: "Vérification des signatures Qrcode pour les fichiers Xltm via C#"
head_description: "Utilisez seulement quelques lignes de code .NET pour vérifier les documents Xltm et leurs signatures Qrcode."

############################# Header ############################
title: "Vérification des signatures Qrcode pour les fichiers Xltm"
description: "L'API pour .NET offre la possibilité de vérifier les signatures Qrcode sur les documents Xltm. La vérification des signatures électroniques dans vos documents Xltm peut être effectuée rapidement et facilement."
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
    title: "Découvrez les nouvelles fonctionnalités de l'API GroupDocs.Signature for .NET"
    content: |
        L'API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) offre un large éventail de façons de traiter de nombreux formats de documents à l'aide de signatures électroniques. De nombreux types de signatures numériques tels que textes, images, certificats numériques, codes-barres, codes QR, tampons ou métadonnées sont pris en charge. Les clients peuvent ajouter, supprimer, modifier, valider ou rechercher des signatures numériques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Un nombre étonnant de fonctionnalités et de paramètres supplémentaires sont disponibles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment valider les signatures Qrcode dans votre document Xltm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inclut des fonctionnalités utiles telles que la vérification des signatures Qrcode placées sur les documents Xltm. Utilisez cette opportunité sans implémenter de code supplémentaire.
        
        * Tout d'abord, instanciez la classe Signature en fournissant comme paramètre de constructeur le chemin d'accès à un document censé être vérifié.
        * Deuxièmement, créez un nouvel objet VerifyOptions et configurez toutes les propriétés requises.
        * Enfin, appelez la méthode Verify de l'objet Signature en passant l'instance VerifyOptions.
        * Traiter ensuite les résultats de la vérification.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Téléchargez la dernière version de GroupDocs.Signature for .NET depuis [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltm file
        string filePath = "input.xltm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signer avec Qrcode signatures Démo en direct"
    content: |
       Ajoutez dès maintenant diverses signatures électroniques au fichier Xltm en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Vérifiez les autres signatures Qrcode à l'aide de C#"
    content: |
        "Vérification des signatures électroniques apposées dans divers documents. Vérifiez la qualité des signatures dans les formats de fichiers populaires comme indiqué ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---