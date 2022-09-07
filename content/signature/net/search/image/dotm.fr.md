---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Dotm
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Dotm with C#

############################# Head ############################
head_title: "Rechercher les signatures Image dans le fichier Dotm dans C#"
head_description: "Utilisez .NET pour rechercher des signatures Image dans des fichiers Dotm en utilisant quelques lignes de code."

############################# Header ############################
title: "Rechercher les signatures Image dans le fichier Dotm"
description: "L'API native .NET permet de rechercher des signatures Image dans des fichiers Dotm déjà signés. Effectuez une recherche avancée de signature électronique dans vos documents Dotm en utilisant quelques lignes de code."
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
    title: "À propos de l'API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) fournit l'API .NET pour le traitement de documents à l'aide de divers types de signature tels que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées. Les utilisateurs peuvent ajouter, supprimer, mettre à jour, vérifier ou rechercher des signatures électroniques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image, avec une prise en charge supplémentaire pour la personnalisation des propriétés des signatures selon les besoins.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment rechercher des signatures Image dans Dotm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permet aux développeurs de .NET de rechercher plus facilement des signatures Image dans des fichiers Dotm à partir de leurs applications en mettant en œuvre quelques étapes simples.
        
        * Créez une nouvelle instance de la classe Signature et transmettez le chemin du document source en tant que paramètre du constructeur.
        * Instanciez l'objet SearchOptions selon vos besoins et spécifiez les options de recherche.
        * Appelez la méthode Search de l'instance de classe Signature et transmettez-lui SearchOptions.
        * Traitez les résultats de recherche en fonction de vos demandes.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Téléchargez la dernière version de GroupDocs.Signature for .NET depuis [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotm file
        string filePath = "input.dotm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Dotm document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signer avec Image signatures Démo en direct"
    content: |
       Ajoutez dès maintenant diverses signatures électroniques aux fichiers Dotm en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Rechercher d'autres signatures Image à l'aide de C#"
    content: |
        "Recherche de signatures électroniques dans divers documents. Trouvez des signatures à partir de l'un des formats de fichiers populaires, comme indiqué ci-dessous."
    format: 
           
       
back_to_top:
    enable: true
---