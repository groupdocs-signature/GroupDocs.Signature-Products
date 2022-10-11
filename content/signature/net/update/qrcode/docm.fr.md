---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Qrcode
fileformat: Docm
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Docm for C#

############################# Head ############################
head_title: "Mettre à jour les signatures Qrcode placées dans les fichiers Docm avec C#"
head_description: "Utilisez le code .NET simple et facile à comprendre pour la mise à jour des signatures Qrcode dans les documents signés Docm."

############################# Header ############################
title: "Modifier et mettre à jour les signatures Qrcode placées dans les fichiers Docm"
description: "L'API pour .NET fournit des fonctionnalités pour la mise à jour des signatures Qrcode dans les documents Docm. Mettez à jour les signatures électroniques dans vos documents Docm avec quelques lignes de code C# rapidement et facilement."
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
    title: "En savoir plus sur les fonctionnalités de l'API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) La fonctionnalité de l'API contient une vaste sélection de moyens pour traiter les formats de documents à la demande à l'aide de signatures électroniques. Un large éventail de signatures électroniques telles que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées sont pris en charge. Les clients peuvent ajouter, supprimer, modifier, valider ou rechercher des signatures numériques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. De nombreuses fonctionnalités et paramètres utiles sont disponibles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment changer les signatures Qrcode dans votre document Docm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inclut des fonctionnalités utiles telles que la mise à jour des signatures Qrcode placées dans les documents Docm. Il permet de modifier les fonctionnalités des signatures sans code supplémentaire.
        
        * Pour commencer, créez un objet Signature passant comme chemin de paramètre constructeur à un document qui est censé être mis à jour.
        * Ensuite, instanciez un objet de signature particulier approprié et configurez son identifiant et ses propriétés qui doivent être modifiées.
        * Enfin, appelez la méthode Update de Signature en passant un objet de signature particulier.
        * Traiter les résultats de mise à jour à votre avis.

    title_right: "Configuration requise"
    content_right: |
        GroupDocs.Signature for .NET sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Téléchargez la dernière version de GroupDocs.Signature for .NET depuis [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docm file
        string filePath = "input.docm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to update
                // set up particular signature id
                QrCodeSignature signatureToUpdate = new QrCodeSignature(id)
                {
                    // specify signature width
                    Width = 200,
                    // specify signature height
                    Height = 200,
                    // set left position
                    Left = 120,
                    // set top position
                    Top = 160
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Mise à jour des signatures Qrcode sur les pages du document - Démo en direct"
    content: |
       Modifiez dès maintenant diverses signatures électroniques du document Docm en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Mettre à jour diverses signatures Qrcode via C#"
    content: |
        "Modification des signatures numériques qui sont placées dans divers formats de documents. Mettez à jour les données des signatures sans code supplémentaire."
    format: 
       
       
back_to_top:
    enable: true
---