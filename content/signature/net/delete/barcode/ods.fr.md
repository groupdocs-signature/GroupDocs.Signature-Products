---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Barcode
fileformat: Ods
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Barcode signature on Ods for C#

############################# Head ############################
head_title: "Supprimez les signatures Barcode des fichiers Ods via C#"
head_description: "La suppression de signatures Barcode spécifiques à partir de documents Ods signés peut être effectuée facilement avec un code .NET court."

############################# Header ############################
title: "Supprimer les signatures Barcode qui sont placées dans les fichiers Ods"
description: "Supprimez diverses signatures Barcode des documents Ods. La suppression des signatures Barcode nécessite un code C# simple."
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
    title: "Obtenir des informations sur les fonctionnalités de l'API GroupDocs.Signature for .NET"
    content: |
        L'API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) propose de nombreuses façons de traiter vos documents à l'aide de signatures électroniques. Des signatures numériques telles que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées sont disponibles. Les clients ont la possibilité d'ajouter, de supprimer, de mettre à jour, de vérifier ou de rechercher des signatures numériques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Un grand nombre de fonctionnalités et de paramètres utiles sont fournis.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment supprimer les signatures Barcode de votre document Ods"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) fournit une fonctionnalité utile pour effacer les documents Ods des signatures Barcode avec quelques lignes de code.
        
        * Tout d'abord, instanciez l'objet Signature passant le chemin d'accès à votre document en tant que paramètre de constructeur.
        * Ensuite, créez un objet de signature approprié et configurez son identifiant unique.
        * Après cela, appelez la méthode Delete en passant l'objet de signature qui doit être supprimé.
        * Enfin, traiter les résultats de l'opération.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Téléchargez la dernière version de GroupDocs.Signature for .NET depuis [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ods file
        string filePath = "input.ods";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "07f83369-318b-41ad-a843-732417b912c2";

                // provide signature features to delete
                // set up particular signature id
                BarcodeSignature signatureToDelete = new BarcodeSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signer avec Barcode signatures Démo en direct"
    content: |
       Ajoutez dès maintenant diverses signatures électroniques au fichier Ods en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Supprimez vos signatures Barcode avec C#"
    content: |
        "Suppression des signatures électroniques qui ont été ajoutées à divers formats de documents. Supprimez les signatures rapidement sans code supplémentaire."
    format: 
       
       
back_to_top:
    enable: true
---